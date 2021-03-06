# Special Topics on Clouds and Environment

This repo contains course materials of the course Clouds and Environment 2019Q1 (AtmSci8047 )

## 課程概述
本課程主旨在討論研究「台灣極端空氣汙染事件在不同天氣型態下之特性」，經由對觀測與模擬資料之分析瞭解當前東亞綜觀天氣型態下台灣PM2.5與環境條件、邊界層、雲物理、輻射收支、大尺度環流之關係，討論其中牽涉之物理過程，並推估未來氣候變遷情境下台灣PM2.5高汙染事件的可能改變。 

## 課程目標
學生在本課程中可以了解紊流尺度下流體與其它物理過程與環境之交互作用。 

## 課程要求
學生將輪流負責上述各課題之論文研讀、報告，然後進行全體討論。 

學生將親自動手分析模擬結果（包括雲解析模式或全球模式）與觀測資料（包括遙測與實地觀測），了解「台灣極端空氣汙染事件在不同天氣型態下之特性」與相關的重要物理過程。 

學生須有自行撰寫與修改程式語言基礎，建議能先修大學部之流體力學、熱力學、地球系統概論、計算機語言、數值分析等課程 

## 更新記錄

### 2019.03.08 
- EPA資料清理，範例在[week01_data_preparation 資料夾](https://github.com/tingsyo/course_ce2019/tree/master/data_preparation)。
- 資料清理，相關軟體安裝請參考：[使用 Python 分析與探索氣象資料](https://github.com/tingsyo/course_py4as)。
- 作業：
  - 範例資料：[pm25_2015.csv](https://github.com/tingsyo/course_py4as/blob/master/data/pm25_2015.csv)
  - 嚴重污染的標準：50/100/150 10^-6g/m^3
  - 定義嚴重空污事件的發生

### 2019.03.15
- repo 架構修改：每週新增內容在新資料夾 /weekNN_TOPIC_NAME，資料存放在 /data
- 新增第二週內容： /week02_define_pollution
- 定義「高污染事件」
- cluster analysis 範例

### 2019.03.20
- 新增 EPA 測站經緯度資訊：/data/epa_stations.csv
- 新增第3週內容： /week03_hararchical_clustering_and_similarity

### 2019.04.17
- 修改 week01_data_preparation/epa_reorganize.ipynb，修正資料合併時資料重複複製的 bug
- 新增 week01_data_preparation/epa_preprocessing.ipynb，利用 EPA data 製作 PM2.5 資料
- 新增 data/pm25_2000_2014.csv

### 2019.04.19
- [bug fixed] week01_data_preparation/epa_reorganize.ipynb -> read_epa_file:
  - 如果第一個讀取的觀測項目不存在或缺資料，其他觀測項目在缺的日期時間即使有資料也會被丟棄
  - 修正：先產生完整「日期─時間」清單再開始讀取變項，如果資料有缺會轉成 missing values
- [updated] data/pm25_2000_2014.csv

### 2019.04.21
- [Added] week04_generalized_linear_model/Generalized_Linear_Model.ipynb

### 2019.05.16
- [Added] week05_dimension_reduction/301_pca_using_python.ipynb
- [Added] week05_dimension_reduction/302_pca_using_python_mnist.ipynb
- [Added] week06_model_evaluation/Evaluating Machine Learning Model.ipynb
- [Added] week06_model_evaluation/Example_model_evaluation.ipynb

### 2019.05.27
- [Added] week05_dimension_reduction/PCA_ncep_example.ipynb
- [Updated] week06_model_evaluation/Example_model_evaluation.ipynb -> Example_cross_validation.ipynb
- [Added] week06_model_evaluation/Example_feature_selection.ipynb


