# Overfitting 過度擬合
> 過度學習訓練資料，變得無法順利去預測或分辨 不是在訓練資料內的其他資料

### Training、Test errors 訓練、測試誤差
### Generalization errors 泛化誤差
  > 真實情況下模型的誤差

</br>

### 未擬合 underfitting
* model 太過簡單
* 訓練集 資料不具代表性、規模太小
* 分類節點(node)增加，錯誤率反而提高
### 過擬合 overfitting
* model 太過複雜
* 訓練集 錯誤率降低、但測試集 錯誤率提高
* 多重比較規則 Multiple Comparison Procedure

</br>

## Model Selection
> 選擇適當的模型，需要估計 generalization error 來判斷

### 1. Using Validation Set
> Divide training data into two parts 
* Training set
* Validation Set

### 2. Incorporating Model Complexity
* [Estimating the Complexity of Decision Trees](https://github.com/fuhsaio/BDLabNotes/blob/main/src/Estimating%20the%20Complexity%20of%20Decision%20Trees.pdf)  
* [Minimum Description Length (MDL)](https://github.com/fuhsaio/BDLabNotes/blob/main/src/Minimum%20Description%20Length%20(MDL).pdf)

### 3. Estimating Statistical Bounds
* [Statistical Bounds](https://github.com/fuhsaio/BDLabNotes/blob/main/src/Statistical%20Bounds.pdf)

</br>

## Model Selection for Decision Trees
> [參考影片解說](https://www.youtube.com/watch?v=u4kbPtiVVB8)
### Pre-Pruning
> 可用在發展決策樹的過程中，一方面可完全學習訓練資料，一方面可避免在過度學習的情形下先停止學習

### Post-pruning
> 其決策樹可以任意發展，待決策樹建立完成後，再將不必要或多餘的分支修剪掉

</br>

## Model Evaluation
> 模型評估

### holdout
> 將原始資料分成訓練集和測試集，分類膜是由訓練集形成，測試集評估

### subsampling
> 重複 holdout，調整訓練與測試集比例 改善分類效果的估計

### cross-validation
> 交叉驗證
> 將資料分成 不相交的兩個區塊，一個作訓練集、一個作測試集。
> 完成後兩個資料角色再互換

