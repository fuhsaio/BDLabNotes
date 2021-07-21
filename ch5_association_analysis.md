## 該單元直接看簡報示例

# Association_analysis
> 透過 co-occurrence 關聯、而不是 causality ( 因果關係 ) 

<br>

## Frequent Itemset
> [範例](https://user-images.githubusercontent.com/86312099/126426071-7a91f56c-6b4d-4edb-b387-a8005adc0e1a.png)

**Itemset** - A collection of one or more items  
**Support count (σ)** - Frequency of occurrence of an itemset  
**Support** - Fraction of transactions that contain an itemset  
**Frequent Itemset** - An itemset whose support is greater than or equal to a min-sup threshold

<br>

## Association Rule
> [範例](https://user-images.githubusercontent.com/86312099/126539177-f3e8abbd-f384-4f7b-ac31-dc475976f1f1.png)  
> An implication expression of the form X → Y, where X and Y are itemsets

### Rule Evaluation Metrics

+ **Support**
  > 支持度 - σ( X ∪ Y ) / N
 
+ **Confidence**
  > 信賴度 - σ( X ∪ Y ) / σ( X )


## Association Rule Mining Task
> 關聯規則探勘目標  
> support ≥ minsup threshold  
> confidence ≥ minconf threshold

<br>

## Brute-force approach
> 窮舉法 - Computationally prohibitive
> 列出所有可能規則  
> 計算每個規則 support、confidence  
> 修剪掉小於 threshold 的規則

### Computational Complexity
> 包含d項目的資料集 萃取出的規則數量 = 3<sup>d</sup> - 2<sup>d + 1</sup> + 1  
> 此為 窮舉所有可能，有很多不必要的計算
> [範例](https://user-images.githubusercontent.com/86312099/126541407-7577f424-c9db-43a8-8280-845425ab8a70.png)  

<br>

### Mining Association Rules
> 關聯規則探勘演算法 將問題切割成以下兩步驟 - (高頻項目產生 依然需要高度計算)

+ **高頻項目集產生 Frequent Itemset Generation**
  > 尋找滿足 support > minsup 的 itemset

+ **規則產生 Rule Generation**
  > 從前一步驟找到的 Frequent Itemset，萃取出具有 high confidence 的規則 (強規則)








