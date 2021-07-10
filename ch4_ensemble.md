# Ensemble 集成
> 以系統化的方式將好幾個監督式學習的模型結合，目的是產生一個更強大的模型

<br>

## Types of Ensemble Methods
+ **Manipulate data distribution**
  + bagging
  + boosting
  
+ **Manipulate input features**
  + random forests
  
+ **Manipulate class labels**
  + error-correcting
  + output coding

## Bagging
> bootstrap aggregating 自助聚合
+ 從 trainning data 中隨機抽取(取後放回)，依每輪抽取的樣本 訓練多個分類器  
  每個分類器權重一致做 Majority vote(多數決)
+ 此抽樣的方法在統計上稱為 bootstrap  
+ 原始資料若有 noisy，可以降低不穩定性

示例 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/Bagging.pdf)

## Boosting
> 透過關注先前錯誤分類的紀錄，自適應改善 訓練集分布的 迭代過程 (iterative)

+ 與 Bagging 不同的是:
  + Boosting 每回合的分類器是有關連的
  + 每筆資料的權重 不相同，在每回合結束後 改變 
+ 將分類錯誤的資料 權重加大，使分類器學習其特性 降低錯誤率
+ 專注於 分類錯誤的資料，因此對 noisy 很敏感，若訓練資料中 noisy 過多  
  後期分類器會集中在 noisy，反而降低 最終分類效果
  
示例 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/Boosting.pdf)

## AdaBoost
> 一種改進的Boosting分類算法。提高前幾個分類器分類錯誤樣本的權重  
> 使用加權投票機制 取代 平均投票機制

原理及示例 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/AdaBoost.pdf)

<br>

---

### 參考文章 - [連結](https://chih-sheng-huang821.medium.com/%E6%A9%9F%E5%99%A8%E5%AD%B8%E7%BF%92-ensemble-learning%E4%B9%8Bbagging-boosting%E5%92%8Cadaboost-af031229ebc3)
### 參考文章 - [連結](http://violin-tao.blogspot.com/2018/01/ml-ensemble.html)


