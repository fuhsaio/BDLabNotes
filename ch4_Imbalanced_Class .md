# Class Imbalance Problem
> 類別分布太過集中，大多紀錄都屬同個類別  
> imbalanced class 難以被評估模型準確性

### Imbalance Class case
+ Credit card fraud
+ Intrusion detection
+ Defective products in manufacturing assembly line

<br>

## Confusion Matrix
> 混淆矩陣  
> 用 預測類別、實際類別 做矩陣組合表示

<table>
  <tr>
    <td></td>
    <td>Predict Y</td>
    <td>Predict N</td>
  </tr>
  <tr>
  <tr>
    <td>Actual Y</td>
    <td>a ( TP )</td>
    <td>b ( FN )</td>
  </tr>
  <tr>
    <td>Actual N </td>
    <td>c ( FP )</td>
    <td>d ( TN )</td>
  </tr>
</table>

示例 - [連結]()

### Accuracy
> Accuracy 是找出 True Positive (TP) 和 True Negative (TN) 的情況  
> A = ( TP + TN ) / ( TP + TN + FP + FN )

### Problem with Accuracy
> 若正向資料(TP)很少 - (信用卡盜刷偵測，盜刷紀錄少)  
> 但 TN 很多，即使準確率(accuracy)高，也無法達到預測目標  
> 因此需要其它指標判斷

<br>

## Alternative Measures
> Precision（準確率）、 Recall（召回率）、 F Measure


