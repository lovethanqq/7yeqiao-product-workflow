# Visual QA Report｜READY_FOR_QA 全量重验

- 实际验收商品数：78。
- 本轮仅做原作品→场景图视觉 QA 和证据交接；未生成新场景图、未上传商品、未修改线上商品。
- 证据 PDF：`reports/VISUAL_QA_EVIDENCE.pdf`，共 39 页，覆盖全部验收商品。

## 互斥统计

| 状态 | 商品数 |
|---|---:|
| QA_PASS | 60 |
| QA_FAIL_CROP | 8 |
| QA_FAIL_CONTENT | 0 |
| QA_FAIL_FRAME | 8 |
| QA_FAIL_SCALE | 0 |
| QA_FAIL_PERSPECTIVE | 0 |
| QA_NEEDS_MANUAL | 2 |

合计：78，应等于本轮验收商品数 78。

## 非 QA_PASS 商品

- P004｜风入蓝｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P004_风入蓝_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原参考作品为无框/未固定该黑色细框状态，当前场景出现明显黑色细框，装裱与原作品不一致
  - 场景2：QA_FAIL_FRAME｜原参考作品为无框/未固定该黑色细框状态，当前场景出现明显黑色细框，装裱与原作品不一致
- P010｜春天的歌｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P010_春天的歌_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原图为木色外框及原有内衬关系，当前场景替换成明显不同的黑色细框，装裱被改变
  - 场景2：QA_FAIL_FRAME｜原图为木色外框及原有内衬关系，当前场景替换成明显不同的黑色细框，装裱被改变
- P011｜静海｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P011_静海_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原作品装裱与当前场景装裱明显不一致，场景改变了原有画框关系
  - 场景2：QA_FAIL_FRAME｜原作品装裱与当前场景装裱明显不一致，场景改变了原有画框关系
- P012｜春径｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P012_春径_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原作品装裱被当前场景图替换/改变，未保留原有装裱关系
  - 场景2：QA_FAIL_FRAME｜原作品装裱被当前场景图替换/改变，未保留原有装裱关系
- P013｜塔尔寺的盛夏｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P013_塔尔寺的盛夏_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原木框及内衬关系与当前场景不一致，场景装裱被改变
  - 场景2：QA_FAIL_FRAME｜原木框及内衬关系与当前场景不一致，场景装裱被改变
- P022｜水果系列2-《桃韵》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P022_水果系列2-《桃韵》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部桃子圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部桃子圆形，原作外缘内容消失
- P023｜水果系列2-《蓝实》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P023_水果系列2-《蓝实》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部蓝实圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部蓝实圆形，原作外缘内容消失
- P024｜水果系列2-《柠黄》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P024_水果系列2-《柠黄》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部柠黄圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部柠黄圆形，原作外缘内容消失
- P025｜水果系列2-《青梨》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P025_水果系列2-《青梨》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜自动提取结果仅保留内部主体区域/近似圆形区域；原作品完整外轮廓或边缘信息未被完整保留；因此不能判定为完整一致
  - 场景2：QA_FAIL_CROP｜自动提取结果仅保留内部主体区域/近似圆形区域；原作品完整外轮廓或边缘信息未被完整保留；因此不能判定为完整一致
- P026｜水果系列2-《圆果.红》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P026_水果系列2-《圆果.红》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图外围仍存在完整作品外缘/背衬/条纹结构，当前场景只保留内部红色果实主体区域，原作品外围内容被裁掉
  - 场景2：QA_FAIL_CROP｜原图外围仍存在完整作品外缘/背衬/条纹结构，当前场景只保留内部红色果实主体区域，原作品外围内容被裁掉
- P040｜轻灵系列—咪｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P040_轻灵系列—咪_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原作品没有当前场景中新增的木框，场景出现额外画框
  - 场景2：QA_FAIL_FRAME｜原作品没有当前场景中新增的木框，场景出现额外画框
- P046｜赤原三骏｜QA_FAIL_CROP｜证据：`previews/qa_batches/P046_赤原三骏_QA.jpg`
  - 场景1：QA_PASS｜ChatGPT 人工复核：场景1保留 QA_PASS；本轮明确问题仅适用于场景2的局部近景/裁片
  - 场景2：QA_FAIL_CROP｜场景2属于作品局部近景/裁片，不是完整作品场景图，完整作品四边和完整画面未保留
- P057｜肌理画｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P057_肌理画_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜高清原始场景中作品区域仅约百余像素，分辨率不足以逐项确认四边、四角、蓝色肌理和暗部纹理是否完整一致；不能猜测
  - 场景2：QA_NEEDS_MANUAL｜高清原始场景中作品区域仅约百余像素，分辨率不足以逐项确认四边、四角、蓝色肌理和暗部纹理是否完整一致；不能猜测
- P059｜桦林秋韵｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P059_桦林秋韵_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜高清原始场景中作品区域仅约百余像素，分辨率不足以逐项确认树干数量、红色树木位置、黄色树冠及上下左右边缘；不能猜测
  - 场景2：QA_PASS｜原图与场景作品区域匹配并已生成透视校正裁片；逐项检查未见明确缺边、内容替换、装裱冲突或明显比例失真
- P062｜叶中花·春野花信｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P062_叶中花·春野花信_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原图装裱为黑色厚外框+金色内框，当前场景未保留原装裱
  - 场景2：QA_FAIL_FRAME｜原图装裱为黑色厚外框+金色内框，当前场景未保留原装裱
- P063｜叶中花·花漫｜QA_FAIL_FRAME｜证据：`previews/qa_batches/P063_叶中花·花漫_QA.jpg`
  - 场景1：QA_FAIL_FRAME｜原图装裱为黑色厚外框+金色内框，当前场景未保留原装裱
  - 场景2：QA_FAIL_FRAME｜原图装裱为黑色厚外框+金色内框，当前场景未保留原装裱
- P077｜权利游戏之来财｜QA_FAIL_CROP｜证据：`previews/qa_batches/P077_权利游戏之来财_QA.jpg`
  - 场景1：QA_PASS｜ChatGPT 人工复核：场景1保留 QA_PASS；本轮明确问题仅适用于场景2的局部特写
  - 场景2：QA_FAIL_CROP｜场景2明显为局部特写，完整作品边界与画面内容没有保留
- P084｜野兽派猫居手记 7（2026）｜QA_FAIL_CROP｜证据：`previews/qa_batches/P084_野兽派猫居手记 7（2026）_QA.jpg`
  - 场景1：QA_PASS｜ChatGPT 人工复核：场景1保留 QA_PASS；本轮明确问题仅适用于场景2的大量裁切
  - 场景2：QA_FAIL_CROP｜场景2明显裁掉大量原作品区域，仅保留局部画面

## 证据说明

每个商品证据板同时展示原作品、场景 1、场景 1 透视校正裁片、场景 2、场景 2 透视校正裁片。自动定位分数仅用于辅助；无法可靠定位的项目按 `QA_NEEDS_MANUAL` 处理。

## 最终人工复核补充证据

本轮补充证据：`reports/VISUAL_QA_FINAL_MANUAL_REVIEW.pdf`；P057/P059 使用 `previews/manual_final/` 原始像素对照图。
