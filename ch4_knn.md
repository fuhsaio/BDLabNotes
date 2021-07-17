# KNN ( k-nearest neighbors )
> k-近鄰演算法  
> k是一個用戶定義的常數。一個沒有類別標籤的向量（查詢或測試點）  
> 測試資料 將被歸類為最接近該點的 k個樣本點中最頻繁使用的一類。

### Rote-learner
> 記住整個訓練集資料，完全匹配某訓練資料值才分類。  
> Rote 是基於實例分類器 ( Instance Based Classifiers ) 最原始的分類方法  
> 鄰近點分類 ( KNN ) 則是 基於實例分類器 的另外一種方法


### Nearest neighbor
> 使用 k 個最近點（最近鄰）進行分類

<img src="https://user-images.githubusercontent.com/86312099/125598012-706fe7f0-b3ad-44b1-808d-cc279bf53193.png" width="500px">

## 運作模式
> The set of labeled records - Supervised ( 監督式學習 )

+ 計算每點之間的距離
  + Euclidean distance...
+ k 值決定鄰近點數目、並投票
  + vote weight = 1/d<sup>2</sup>
+ 投票結果決定預測類別

<br>

### knn feature & efficiency
> 相關特性及方法 - [簡報連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_knn_issue.pdf)

### Voronoi Diagram
> 1 nearest-neighbor  
> 每個鄰近的點的中垂線，形成 [Voronoi Diagram](http://web.ntnu.edu.tw/~algo/Neighbor.html)

### Scaling issues
> 屬性值需要 比例縮放( Scaled )，避免計算距離 受單一屬性影響過大

---
### 參考文章
**knn 簡介** - [連結](https://pyecontech.com/2020/04/19/knn/)  
**knn & k-mean 差異** - [連結](https://medium.com/chung-yi/ml%E5%85%A5%E9%96%80-%E4%BA%8C%E5%8D%81%E4%B8%80-knn%E8%88%87k-means%E5%B7%AE%E7%95%B0-7dc6ad0227fc)  
**knn python-sklearn** - [連結](https://ithelp.ithome.com.tw/articles/10197110)
