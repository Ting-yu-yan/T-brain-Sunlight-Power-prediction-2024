# T-brain-Sunlight-Power-prediction-2024
This repository is used to store the related files and code used for this competition 

## 環境設定

- **Python**: 3.10.12
- **Torch**: 2.5.1
- **NumPy**: 1.26.4
- **Pandas**: 2.2.2
- **Matplotlib**: 3.8.0
- **Scikit-learn**: 1.5.2
- **XGBoost**: 2.1.3
- **CatBoost**: 1.2.7

## Src 說明與參數設定

在資料夾 src 中有兩個 ipynb 檔案，分別是**演算法1**與**演算法2**，基本上只要安裝以上的環境就可以直接從頭到尾運行整個腳本，
其腳本已經包含資料的匯入、資料前處理、模型建立與預測值的生成。
唯一需要注意的是在**演算法1**跟**演算法2**中我們需要給定訓練資料 (Training data) 以及測試資料 (Testing data)的檔案路徑以及最後產生預測值之後要存放的位置 :

**url_training_data** = r"/content/drive/MyDrive/Colab Notebooks/Data science competition/T-brain 2024 Sun light Power predition/Training data"

**url_testing_data** = '/content/drive/MyDrive/Colab Notebooks/Data science competition/T-brain 2024 Sun light Power predition/Testing data'

**url_output** = '/content/drive/MyDrive/Colab Notebooks/Data science competition/T-brain 2024 Sun light Power predition/Testing data/'

讀者可以根據自己實際的情形修改檔案的位置，而我們的 training data 跟 testing data 都可以在該 github 的 repository 中取得。

## Score table

| 演算法       | 描述                          | Private leader board   |
|------------|-------------------------------|---------|
| 演算法1    | 一次考量所有 Site 的資料，並且建立 LSTM + XGBoost + CatBoost 的預測模型    | 638932.89  |
| 演算法2    | 一次只考量一個 Site 的資料，並且建立 LSTM + XGBoost + CatBoost 的預測模型     |  1066292.98 |
