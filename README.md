# OCR-IDcard
OCR识别身份证任务
使用 DETR-RESNET-50模型进行文字信息定位，裁剪获取对应图片后使用 trocr-base-handwritten 模型进行文字识别。
 DETR-RESNET-50模型
 https://huggingface.co/facebook/detr-resnet-50
 trocr-base-handwritten 模型
 https://huggingface.co/microsoft/trocr-base-handwritten

 目前已更新文字定位代码，后续更新文字识别，测试训练部分的代码
