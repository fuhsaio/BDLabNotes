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

## Model Selection (連結資料未放)
> 選擇適當的模型，需要估計 generalization error 來判斷

### 1. Using Validation Set
> Divide training data into two parts 
* Training set
* Validation Set

### 2. Incorporating Model Complexity
* [Estimating the Complexity of Decision Trees]()  
* [Minimum Description Length (MDL)]()

### 3. Estimating Statistical Bounds
* [Statistical Bounds]()

</br>

## Model Selection for Decision Trees
### [Pre-Pruning (Early Stopping Rule)]()
### [Post-pruning]()

