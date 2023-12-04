# 圍棋棋力模仿與棋風辨識競賽
隊伍：TEAM_3752

## 文件目錄

```
├── README.md
├── requirements.txt
├── 棋力模仿
│   ├── Dan_Kyu_feature10.ipynb
│   ├── Dan_Kyu_feature18.ipynb
│   ├── Dan_organize_data.ipynb
│   ├── esemble_add.ipynb
│   ├── inception_attention_feature10.ipynb
│   ├── Kyu_organize_data.ipynb
│   └── uptodown_model_feature18.ipynb
├── 棋風辨識
│   ├── PS_feature10_v3.ipynb
│   └── PS_model.ipynb
```

## 執行環境

Python環境
```
Python 3.10.12
```

安裝套件
```
pip install -r requirements.txt
```

## 執行

### 棋力模仿

#### 資料前處理

- **Dan_organize_data.ipynb**: 將初段的CSV檔案轉換至SGF檔案
- **Kyu_organize_data.ipynb**: 將十級的CSV檔案轉換至SGF檔案

#### 特徵工程
- **Dan_Kyu_feature10.ipynb**: 把棋力模仿的棋譜資料做成特徵10的資料集
- **Dan_Kyu_feature18.ipynb**: 把棋力模仿的棋譜資料做成特徵18的資料集

#### 模型預測
- **inception_attention_model.ipynb**: 模型1
- **updown_model.ipynb**: 模型2
- **esemble_add.ipynb**: 對模型1與模型2的結果做集成學習，並輸出預測值

### 棋風辨識

#### 資料前處理與特徵工程
- **PS_feature10_v3.ipynb**: 將棋風辨識的CSV檔案轉換至SGF檔案並做成特徵10的資料集

#### 模型預測
- **PS_model.ipynb**: 棋風模型