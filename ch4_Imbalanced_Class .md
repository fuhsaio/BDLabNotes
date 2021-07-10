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

**範例** - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_Accuracy.pdf)

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

#### Precision(p)
> a / ( a + c )
#### Recall(r) 
> a / ( a + b )
#### F-measure(F) 
> 2rp / ( r + p ) = 2a / ( 2a + b + c )

<br>

**範例** - [連結](https://github.com/fuhsaio/BDLabNotes/blob/main/src/ch4_AlternativeMeasures.pdf)

<br>

## ROC ( Receiver Operating Characteristic )
> 是一個顯示真陽性比率（TPR）、及偽陽性比率（FPR）兩個值之間相互取捨的圖形

+ **( TPR , FPR )**
  + ( 0 , 0 ) - 表示 模式預測每個資料為 負類別
  + ( 1 , 1 ) - 表示 模式預測每個資料為 正類別
  + ( 1 , 0 ) - 表示 理想模式 ( ideal )

### 繪製 ROC曲線
> 使用分類器輸出的 連續型 ( continuous-valued ) output 並排序  
> 依序將 資料值作 閥值。 大於閥值 - 視為陽性 、 小於閥值 - 視為陰性  
> 比較 真實類別 計算 ( TPR , FPR ) 值  
> 將每輪得到的 ( TPR , FPR ) 值繪製即為 ROC 曲線 

簡報範例 - [連結]()  


<br>

---
### 參考文章
**Confusion Matrix 指標** - [連結](https://www.ycc.idv.tw/confusion-matrix.html)  
**ROC曲線繪製** - [連結](https://zhuanlan.zhihu.com/p/147919317)



