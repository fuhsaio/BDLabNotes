# Rule-Based Classifier
> 透過建立 " if ... then ..." 規則進行分類  
> 規則 : anteceden ( 前因 ) => consequent ( 後果 )

<br>

## Rule Coverage and Accuracy
 
<img src="https://user-images.githubusercontent.com/86312099/125877617-193e2be2-852d-41bd-bdff-795c5be2edce.png" width="300"> 

### Coverage of a rule
> 符合 antecedent of a rule 的資料比例

### Accuracy of a rule
> 符合 antecedent and consequent 的資料比例



<br>

## Characteristics of Rule Sets
### Strategy 1
+ **Mutually exclusive rules**
  > 規則彼此獨立  
  > 每筆紀錄 最多包含一個規則

+ **Exhaustive rules**
  > 詳盡所有特徵值組合的規則  
  > 每筆紀錄 至少包含一個規則

### Strategy 2
+ **Rules are not mutually exclusive**
  > 觸發超過一個規則  
  > Solution : Ordered rule set、Unordered rule set – use voting schemes

+ **Rules are not exhaustive**
  > 沒有觸發規則  
  > Solution : Use a default class

<br>

### Ordered Rule Set
> 規則 按照優先級排序 - [範例](https://user-images.githubusercontent.com/86312099/125884828-45d5e3cc-6449-45ed-ab50-86b89de9da31.png)

### Rule Ordering Schemes
> Rule-based ordering (規則排序)、Class-based ordering (分類排序) - [範例](https://user-images.githubusercontent.com/86312099/125885635-169e3b6d-4998-47be-9a7f-f320acf9c493.png)






