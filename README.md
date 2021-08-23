# IIR新生訓練python_HW
## 執行方式
* Google Drive Colab Notebook
* 檔案下載：

    https://drive.google.com/file/d/1H1KOMeOd5E1wFBDAPlbslKT1rnVvJeX-/view?usp=sharing
## 處理方式
* #### read sales_train.csv:
1. 讀取所有資料，並判斷此資料月份
   data[:][0][3:] : 所有資料之月份(包含年份)
2. 將每月資料之item_price進行加總
3. 為月銷售額依照年份構建折線圖
4. 將不同店家之各項商品銷售額進行加總，在為其構建直方圖:
   df.groupby(['shop_id']).sum()

## 圖表分析
### 1.月銷售額 (折線圖)
* 分析每一年在不同月份間之銷售額成長趨勢
![](https://i.imgur.com/lrrX5m9.png)

### 2.每家店家之總銷售額 (直方圖)
* 分析哪些店家面臨銷售額短缺之問題
![](https://i.imgur.com/8ulfrXD.png)


