# 資料 Data
資料與其屬性的集合
> 屬性是指物件的特性，其值可能會隨時間變動

### 屬性值
可用 數值 或 符號 表示
### 屬性和屬性值的區別
相同屬性 對應 不同屬性值
> 長度 → 公尺、公分...  

不同屬性 對應 相同屬性值
> 年齡、身高 → 以整數(數值)表示

## 屬性型態
|   |類別|運算方式|範例|
|---|:-:|:------:|---|
|**名目 Nominal**  | 定性 | = ≠| 員工編號、眼睛顏色、郵遞區號 |
|**順序 Ordinal**  | 定性 | = ≠ > <| 成績、金屬硬度 |
|**區間 Interval** | 定量   | = ≠ > < </br> + -| 日期、華氏攝氏溫度 |
|**比例 Ratio**    | 定量   | = ≠ > < </br> + - × ÷| 長度、重量、價格|

詳細資料參考 ： [連結](https://medium.com/marketingdatascience/%E5%B0%BA%E5%BA%A6%E7%9A%84%E9%A1%9E%E5%9E%8B-%E5%90%8D%E7%9B%AE%E5%B0%BA%E5%BA%A6-%E9%A0%86%E5%BA%8F%E5%B0%BA%E5%BA%A6-%E5%8D%80%E9%96%93%E5%B0%BA%E5%BA%A6-%E6%AF%94%E4%BE%8B%E5%B0%BA%E5%BA%A6-d567f93b5104)

### 離散性屬性 Discrete
> 屬性為 有限 或 可數  
> e.g. 郵遞區號  
> 二元屬性 是 離散性屬性
### 連續性屬性 Continuous
> e.g. 氣溫

## 對資料探勘具重大影響的資料特性
+ **維度 Dimension** - 資料集的維度 就是指物件的屬性，維度越高越難分析
+ **稀疏度 Sparsity** - 非對稱資料，該資料可能只有 1% 不為 0 ( 只有非 0 需要運算 )，但也節省時間與儲存空間
+ **解析度 Resolution** - 不同解析度對特性會有影響，用 公里、公尺 為單位查看地圖，公里的地貌相對平坦 (解析度太大，特性可能消失)

## 資料品質的問題
+ **雜訊 Noise**
+ **遺漏值 Missing**
+ **離群值 Outliers** - 分析時忽略不計
+ **重複性資料 Duplicate** - 需資料清理 data cleaning

</br></br></br>

# 相似度和距離 Similarity and Distance (待補充 未完成)
### 鄰近度 proximity
> 表示兩個物件的 相似 與 不相似度
### 相似度 Similarity
> 數值越大，物件越像  
> 值介於 0 - 1
### 不相似度 Dissimilarity
> 數值 ( 距離 ) 越大，物件差異越大  
> 最小的相異度 時常是 0  
> 值介於 0 - ∞ (對象不同)  

---
### 歐基里德 距離
> 求兩點直線距離
* n 維度個數 ( 屬性 )  
* x<sub>k</sub>、y<sub>k</sub>，指其第 k 個屬性

<img src="https://user-images.githubusercontent.com/86312099/123497641-3d16ac80-d661-11eb-8045-28d3cc24b960.png">

---

### Minkowski 距離
> 由歐幾里德距離衍生
+ r 參數
  + r = 1，[漢明距離](https://zh.wikipedia.org/wiki/%E6%B1%89%E6%98%8E%E8%B7%9D%E7%A6%BB)、[曼哈頓距離](https://zh.wikipedia.org/wiki/%E6%9B%BC%E5%93%88%E9%A0%93%E8%B7%9D%E9%9B%A2)
  + r = 2，歐幾里德距離
  + r = ∞，[切比雪夫距離](https://zh.wikipedia.org/wiki/%E5%88%87%E6%AF%94%E9%9B%AA%E5%A4%AB%E8%B7%9D%E7%A6%BB)     
+ n 維度個數 ( 屬性 ) 
+ x<sub>k</sub>、y<sub>k</sub>，指其第 k 個屬性

<img src="https://user-images.githubusercontent.com/86312099/123498642-de9efd80-d663-11eb-8aa1-b078d3a3d054.png">

> 切比雪夫距離 ( r = ∞ )  
> <img src="https://user-images.githubusercontent.com/86312099/123499494-d5b12a80-d669-11eb-9f86-2b3d475518a6.png">

</br>

---
### Mahalanobis 距離(待補充)
---

## Metric 度量(指標)
> 當距離滿足以下條件，則稱為 metric

歐基里德距離 為例 :
+ 正向性
  + d( x , y ) ≧ 0，對所有 x、y 而言
  + d( x , y ) ＝ 0，當 x = y
+ 對稱性
  + d( x , y ) = d( y , x )，對所有 x、y 而言
+ 三角不等式
  + d( x , z ) ≦ d( x , y ) + d( y , z )，對所有 x、y、z 而言
  
