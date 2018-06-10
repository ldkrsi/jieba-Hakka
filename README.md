# jieba-Hakka
[![DOI](https://zenodo.org/badge/136745050.svg)](https://zenodo.org/badge/latestdoi/136745050)

以 jieba 的演算法替換其詞庫及 HMM 機率表所製作的客家語斷詞程式

## Requirement

- Python3

## Usage

將 jieba 資料夾放在你程式的資料夾底下

```python
import jieba

seg_list = jieba.cut("原來你就係狗仔个阿哥") 
print("|".join(seg_list))
# 原來|你|就|係|狗仔|个|阿哥
```

## 資料來源

### 語料來源

- 苗栗、東勢、新屋、楊梅、龍潭、花蓮客語故事集
- 客家笑科、徐老師講古
- 共257,718字、189,497個詞、12,668個不重複單詞

### 斷詞標準

- 詞的定義採與中研院資所之中文線上斷系統所公佈的[精簡詞類](http://ckipsvr.iis.sinica.edu.tw/cat.htm)相同標準
- 用字修訂及拼音轉文字以[教育部臺灣客家語常用詞辭典](http://hakka.dict.edu.tw/hakkadict/index.htm)為標準

## Acknowledgement

感謝國立政治大學語言所**賴惠玲**教授提供資源及機會來完成這支程式；也感謝賴惠玲教授主持的計畫底下的助理人員（圖書資訊與檔案學研究所**王勻芊**同學，語言學研究所**胡雪瀅**、**蔡宛玲**、**紀立昕**同學，英國語文學系**譚雅庭**、**陳怡如**、**洪培綸**同學，等10人）耗費大量心力建立訓練資料。
