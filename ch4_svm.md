# Support Vector Machines ( SVM )
> 在超平面上找出資料的 最佳分隔線

<img src="https://user-images.githubusercontent.com/86312099/126025917-f6fefc48-bd1a-422d-8b71-0cc87b23a052.png" width="550">

<br>

## Linear SVM
> 線性平面 - [範例](https://user-images.githubusercontent.com/86312099/126026024-82835e07-4d77-41fd-8c06-1ad807fc50b0.png)

<img src="https://user-images.githubusercontent.com/86312099/126025976-c7c19d1c-477d-4469-a085-b06bc340e70c.png" width="450">

<br>

## Linear separation problem
> 有些資料點會進入 margin 區域 - [圖例](https://user-images.githubusercontent.com/86312099/126026222-4fdfaa77-77ba-49f5-9ff5-51b45a4eb611.png)  
> 使用 slack variables 擴大判斷範圍，其值越大容忍範圍越大

<img src="https://user-images.githubusercontent.com/86312099/126026120-eae09346-ff4c-4d23-b970-2652c4aeac48.png" width="450">

<br>

## Nonlinear SVM
> 非線性  
> 原本資料分隔邊界為 非線性 - [圖例](https://user-images.githubusercontent.com/86312099/126026377-020143e9-6060-41cc-93da-1783dbd9ab9c.png)  
> 將資料轉換至更高維度 得出線性的資料分隔邊界

<img src="https://user-images.githubusercontent.com/86312099/126026508-11a05d41-8a31-4712-9275-e0f1ededfe69.png" width="550">

<img src="https://user-images.githubusercontent.com/86312099/126026488-77d0a848-6530-49a5-8cf9-6cc670e83f34.png" width="550">

## Nonlinear SVM Issues
> high dimensional  
> What type of mapping function ϕ should be used  
> Most computations involve dot product  Φ( x<sub>i</sub> ) ● Φ( x<sub>j</sub> )

## Kernel Trick
>  Φ( x<sub>i</sub> ) ● Φ( x<sub>j</sub> ) = k ( x<sub>i</sub> , x<sub>j</sub> )
>  K(xi, xj) is a kernel function ( )




<br>

---
### 參考文章
**SVM 簡介** - [連結](https://chih-sheng-huang821.medium.com/%E6%A9%9F%E5%99%A8%E5%AD%B8%E7%BF%92-%E6%94%AF%E6%92%90%E5%90%91%E9%87%8F%E6%A9%9F-support-vector-machine-svm-%E8%A9%B3%E7%B4%B0%E6%8E%A8%E5%B0%8E-c320098a3d2e)










