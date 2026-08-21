# Visual QA Report｜READY_FOR_QA 全量重验

- 实际验收商品数：78。
- 本轮仅做原作品→场景图视觉 QA 和证据交接；未生成新场景图、未上传商品、未修改线上商品。
- 证据 PDF：`reports/VISUAL_QA_EVIDENCE.pdf`，共 39 页，覆盖全部验收商品。

## 互斥统计

| 状态 | 商品数 |
|---|---:|
| QA_PASS | 61 |
| QA_FAIL_CROP | 3 |
| QA_FAIL_CONTENT | 0 |
| QA_FAIL_FRAME | 0 |
| QA_FAIL_SCALE | 0 |
| QA_FAIL_PERSPECTIVE | 0 |
| QA_NEEDS_MANUAL | 14 |

合计：78，应等于本轮验收商品数 78。

## 非 QA_PASS 商品

- P004｜风入蓝｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P004_风入蓝_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜匹配框覆盖墙面而非真实作品四角；虽能看到作品，当前证据不能逐边完成透视校正
  - 场景2：QA_NEEDS_MANUAL｜匹配框覆盖木墙/背景而非真实作品四角；虽能看到作品，当前证据不能逐边完成透视校正
- P010｜春天的歌｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P010_春天的歌_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜匹配框覆盖墙面和柜体而非真实作品四角；当前证据不足以逐边核验画芯
  - 场景2：QA_NEEDS_MANUAL｜匹配框覆盖木墙/柜体而非真实作品四角；当前证据不足以逐边核验画芯
- P011｜静海｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P011_静海_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜匹配框覆盖墙面和柜体而非真实作品四角；当前证据不足以逐边核验画芯
  - 场景2：QA_NEEDS_MANUAL｜匹配框覆盖木墙/柜体而非真实作品四角；当前证据不足以逐边核验画芯
- P012｜春径｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P012_春径_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜匹配框覆盖墙面和柜体而非真实作品四角；当前证据不足以逐边核验画芯
  - 场景2：QA_NEEDS_MANUAL｜匹配框覆盖木墙/柜体而非真实作品四角；当前证据不足以逐边核验画芯
- P013｜塔尔寺的盛夏｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P013_塔尔寺的盛夏_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜匹配框覆盖墙面/桌面背景而非真实作品四角；当前证据不足以逐边核验画芯
  - 场景2：QA_NEEDS_MANUAL｜匹配框覆盖木墙/柜体而非真实作品四角；当前证据不足以逐边核验画芯
- P022｜水果系列2-《桃韵》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P022_水果系列2-《桃韵》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部桃子圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部桃子圆形，原作外缘内容消失
- P023｜水果系列2-《蓝实》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P023_水果系列2-《蓝实》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部蓝实圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部蓝实圆形，原作外缘内容消失
- P024｜水果系列2-《柠黄》｜QA_FAIL_CROP｜证据：`previews/qa_batches/P024_水果系列2-《柠黄》_QA.jpg`
  - 场景1：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景1只保留内部柠黄圆形，原作外缘内容消失
  - 场景2：QA_FAIL_CROP｜原图可见圆形作品外圈的蓝白条纹边缘，场景2只保留内部柠黄圆形，原作外缘内容消失
- P026｜水果系列2-《圆果.红》｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P026_水果系列2-《圆果.红》_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜圆形作品外缘/背衬与场景边界关系无法仅凭当前匹配框可靠确认，不能猜测完整性
  - 场景2：QA_NEEDS_MANUAL｜圆形作品外缘/背衬与场景边界关系无法仅凭当前匹配框可靠确认，不能猜测完整性
- P040｜轻灵系列—咪｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P040_轻灵系列—咪_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜命中四边覆盖墙面和家具背景，未能可靠定位真实作品边界；不能据此判断完整性/装裱
  - 场景2：QA_NEEDS_MANUAL｜无法可靠定位真实作品四角，不能完成完整性/装裱核验
- P046｜赤原三骏｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P046_赤原三骏_QA.jpg`
  - 场景1：QA_PASS｜原图与场景作品区域已生成透视校正裁片；逐项检查边缘、主体、主要色块、装裱和透视，未见明确不一致
  - 场景2：QA_NEEDS_MANUAL｜场景2作品区域无法可靠定位，不能检查四边、四角和内容
- P057｜肌理画｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P057_肌理画_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜作品在场景1中尺寸过小，当前证据不足以逐项检查边缘、内容和装裱
  - 场景2：QA_NEEDS_MANUAL｜作品在场景2中尺寸过小，当前证据不足以逐项检查边缘、内容和装裱
- P059｜桦林秋韵｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P059_桦林秋韵_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜场景1作品过小，无法可靠定位四角
  - 场景2：QA_PASS｜原图与场景作品区域匹配并已生成透视校正裁片；逐项检查未见明确缺边、内容替换、装裱冲突或明显比例失真
- P062｜叶中花·春野花信｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P062_叶中花·春野花信_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜场景1作品过小，无法可靠定位四角
  - 场景2：QA_NEEDS_MANUAL｜自动命中落在墙面/家具边缘而非作品四角，无法确认
- P063｜叶中花·花漫｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P063_叶中花·花漫_QA.jpg`
  - 场景1：QA_NEEDS_MANUAL｜作品过小，无法可靠定位四角
  - 场景2：QA_NEEDS_MANUAL｜作品过小，无法可靠定位四角
- P077｜权利游戏之来财｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P077_权利游戏之来财_QA.jpg`
  - 场景1：QA_PASS｜原图与场景作品区域匹配并已生成透视校正裁片；逐项检查未见明确缺边、内容替换、装裱冲突或明显比例失真
  - 场景2：QA_NEEDS_MANUAL｜场景2为近景/细节式图，无法确认完整作品边缘和场景关系
- P084｜野兽派猫居手记 7（2026）｜QA_NEEDS_MANUAL｜证据：`previews/qa_batches/P084_野兽派猫居手记 7（2026）_QA.jpg`
  - 场景1：QA_PASS｜原图与场景作品区域匹配并已生成透视校正裁片；逐项检查未见明确缺边、内容替换、装裱冲突或明显比例失真
  - 场景2：QA_NEEDS_MANUAL｜场景2为近景/细节式图，无法确认完整作品边缘和场景关系

## 证据说明

每个商品证据板同时展示原作品、场景 1、场景 1 透视校正裁片、场景 2、场景 2 透视校正裁片。自动定位分数仅用于辅助；无法可靠定位的项目按 `QA_NEEDS_MANUAL` 处理。
