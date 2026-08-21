# VISUAL_QA_TASK

## 目标

重新验收当前被标记为 `READY_FOR_QA` 的全部商品。禁止把“已有两张场景图”直接等同于成功。

本轮只做视觉 QA 和证据交接：不生成新场景图、不上传商品平台、不修改线上商品。

## 必须先读取

- `docs/CURRENT_RULES.md`
- `docs/QA_ACCEPTANCE_RULES.md`
- `manifests/xhs_scene_manifest.csv`
- `reports/LATEST_REPORT.md`

## 验收范围

对 Manifest 中所有当前 `READY_FOR_QA` 商品逐个检查，预计 78 个；以实际 CSV 状态为准，不允许只抽样。

每个商品必须同时定位：

1. 原作品高清图/完整原始参考。
2. 最终场景图 1。
3. 最终场景图 2。

若任一证据无法确定，标记 `QA_NEEDS_MANUAL`，不要猜。

## 每张场景图检查内容

### 1. 作品完整性

- 矩形作品四边是否完整。
- 圆形作品完整圆周是否完整。
- 是否缺角、缺边、裁掉原作有效画面。
- 是否被框、卡纸、家具、植物、灯具等遮挡有效画面。

### 2. 原作内容一致性

逐项对照原图：

- 主体和细节是否丢失。
- 是否新增原作不存在的元素。
- 是否出现重绘、替换、镜像、旋转、错误补全。
- 主要色块、线条、肌理、文字、人物、动物、建筑等结构是否保持。

不能只看“整体像不像”。尤其要检查原图四个边缘、角落和细节密集区域。

### 3. 画框/卡纸/装裱

- 原有画框是否保留。
- 原有卡纸/留白是否保留。
- 原本无框的是否误加固定框。
- 原本有框的是否被变成裸画芯。
- 外框颜色、厚度、比例是否明显错误。

### 4. 比例与透视

- 是否有横向拉伸、纵向压缩、弯曲、异常梯形。
- 对斜视场景，先提取作品四角并做透视校正，再把校正后的作品区域与原图比较。
- 不允许仅根据场景里未校正的矩形长宽比下结论。

### 5. 尺寸感

依据 Manifest 的真实尺寸判断场景尺度是否明显错误。只判断明显失真，不要求毫米级反推。

## 推荐技术流程

可以写 Python/OpenCV 辅助，但任何自动分数都不能替代人工检查：

1. 定位场景里的作品区域。
2. 提取四角/轮廓。
3. 透视校正成正视图。
4. 与原图统一方向和比例。
5. 计算特征匹配/结构相似度作为提示。
6. 对差异区域生成可视化或放大裁片。
7. 最终由视觉证据判定，不允许仅凭 SSIM、pHash、特征点数量自动通过。

## 必须输出的证据

创建：

- `manifests/xhs_scene_qa.csv`
- `reports/VISUAL_QA_REPORT.md`
- `previews/qa_batches/`

建议每张 QA batch 最多放 4 个商品，保证细节可读。每个商品面板至少包含：

- 商品序号、作品名、艺术家、真实尺寸、装裱信息。
- 原作品参考图。
- 场景图 1。
- 场景图 1 的透视校正作品裁片。
- 场景图 2。
- 场景图 2 的透视校正作品裁片。
- 两张场景分别的 QA 状态和原因。

对任何失败或不确定商品，另外生成单商品高清证据：

`previews/qa_failures/Pxxx_作品名_QA.jpg`

## QA CSV 字段

至少包含：

- 商品序号
- 商品ID
- 艺术家
- 作品名
- artwork_lookup_key
- original_reference
- scene_1_reference
- scene_1_qa_status
- scene_1_qa_reason
- scene_2_reference
- scene_2_qa_status
- scene_2_qa_reason
- product_qa_status
- qa_evidence_path

`artwork_lookup_key` 建议为 `艺术家-作品名`。不要提交 token、cookie、API key。

## 最终状态

只允许：

- `QA_PASS`
- `QA_FAIL_CROP`
- `QA_FAIL_CONTENT`
- `QA_FAIL_FRAME`
- `QA_FAIL_SCALE`
- `QA_FAIL_PERSPECTIVE`
- `QA_NEEDS_MANUAL`

同一个商品只要两张最终场景里任意一张失败，该商品就不能 `QA_PASS`。

## 报告要求

报告必须写清：

- 实际验收商品数。
- `QA_PASS` 数。
- 每种失败类型数量。
- `QA_NEEDS_MANUAL` 数。
- 发现的具体问题商品编号和简要原因。
- 统计必须互斥并能加总到本轮验收商品总数。

## 结束条件

完成后：

1. 更新 `tasks/CURRENT_TASK.md` 记录本轮实际工作。
2. 把 `tasks/NEXT_TASK.md` 改为 `WAITING_FOR_CHATGPT_VISUAL_QA`。
3. 提交并 push 到 `fix/visual-qa-handoff-20260821` 分支。
4. 不要合并到 `main`，等待 ChatGPT 再次逐图验收。
