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
> 暴力破解 - Computationally prohibitive
> 列出所有可能規則  
> 計算每個規則 support、confidence  
> 修剪掉小於 threshold 的規則

### Computational Complexity
> 計算複雜度 = 3<sup>d</sup> - 2<sup>d + 1</sup> + 1  
> [範例](https://user-images.githubusercontent.com/86312099/126541407-7577f424-c9db-43a8-8280-845425ab8a70.png)  








