# Classification
</br>

+ **Base Classifiers**
  + Decision Tree based Methods
  + Rule-based Methods
  + Nearest-neighbor
  + Neural Networks
  + Deep Learning
  + Naïve Bayes and Bayesian Belief Networks
  + Support Vector Machines
+ **Ensemble Classifiers**
  + Boosting
  + Bagging
  + Random Forests

</br>

# Decision Tree 決策樹

</br>

## Example
<img src ="https://user-images.githubusercontent.com/86312099/123761692-a6621e00-d8f4-11eb-8487-5809dfd9ce2a.png">

> 相同的資料集 可能找到 一個以上符合規則的決策樹。如下圖
<img src ="https://user-images.githubusercontent.com/86312099/123761698-a8c47800-d8f4-11eb-90d0-139f819bc5f6.png">

</br>

## Induction Algorithms 歸納演算法
* **Hunt’s Algorithm** ( one of the earliest )
* **CART**
* **ID3, C4.5**
* **SLIQ,SPRINT**

### Hunt’s Algorithm

> 用遞廻的方式不斷地將訓練資料分割至後繼的子集合中

### 遞迴 方式
Step1 : Dt 的所有資料都屬於 相同類別 ，那麼 t 為一葉節點(Yt)  
Step2 : Dt 包含一個類別以上的資料，會再選取一個屬性測試條件，將資料分至更小集合
> Dt 為節點 t 相關的訓練資料  
> Y = {y1,y2...yn} 為 類別標記

</br>

## Methods for Expressing Test Conditions
> 屬性測試條件的表示方法

+ **屬性類型 attribute types**
  + Binary
  + Nominal
  + Ordinal
  + Continuous
+ **拆分數量 number of ways to split**
  + Binary split
    > 2-way split，分成 兩個子集，若為 ordinal type 拆分後會保留順序性
  + Multi-way split
    > 拆分成 n 個子集 ( n > 2 ) 

