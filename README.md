# OCR身份证识别任务

## 总述
使用 DETR-RESNET-50模型进行文字信息定位，裁剪获取对应图片后使用 trocr-base-handwritten 模型进行文字识别。

## 环境

PyTorch==1.12.1+cuda
transformers==4.36.2
datasets==2.16.1

[数据集](https://huggingface.co/datasets/lansinuote/ocr_id_card_small)
```
from datasets import load_dataset
#解压数据文件
#注意路径要一致
name = 'lansinuote/ocr_id_card_small'
load_dataset(name).save_to_disk('dataset/' + name)
```

[DETR-RESNET-50模型](%3Cspan%3E%3Cdiv%3Ehttps://huggingface.co/facebook/detr-resnet-50%3C/div%3E%3C/span%3E)
 
 [trocr-base-handwritten 模型](%3Cspan%3E%3Cdiv%3Ehttps://huggingface.co/microsoft/trocr-base-handwritten%3C/div%3E%3C/span%3E)

 
