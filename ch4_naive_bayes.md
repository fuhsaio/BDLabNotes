# Bayes Classifier 
> 貝氏分類器 基於機率模型，假設每個特徵間互相獨立

<br>

## 條件機率、貝氏定理
> 範例 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_Bayes_Theorem.pdf)
<img src="https://user-images.githubusercontent.com/86312099/125765293-046f093f-8953-4359-b7ad-e21cd55accd4.png" width="400">

<br>

## Bayes Theorem for Classification
> 特徵值( X1, X2,…, Xd )、目標( 預測類別 Y )  
> 貝氏定理 計算每個類別機率 P( Y | X1, X2,…, Xd )  
> 類別機率最大者 即為預測類別  

範例 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_Bayes_eg.pdf)  

### Conditional Independence
> 兩事件 A 和 B 在給定的另一事件 C 發生時條件獨立  
> P ( A ⋂ B | Y ) = P( A | Y ) × P( B | Y ) 

<br>

## Estimate Probabilities from Data
> 連續型數值資料 需要經過處理才能計算 概率分布

### Continuous attributes
+ **Discretization** - Partition the range into bins (桶)
+ **Probability density estimation** - [機率密度函數](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_Bayes_continous_probability.pdf)

<br>

### Issues with Naïve Bayes Classifier
> 若其中一個概率值為 0，整個表達式變為 0  
> 除了簡單分數，需要其他 估計條件概率的方式

問題及替代方式 - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_Bayes_issue.pdf)


### Naïve Bayes (Summary)
+ 可以處理不相關的屬性
+ 可以處理雜訊資料的問題
+ 在模式建立以及分類的時候忽略掉遺漏值
+ 關聯度高的屬性可能會因為沒有滿足條件獨立的假設，而使得誤判率提高
  + 使用其他技術，例如貝葉斯信念網絡 (BBN)


