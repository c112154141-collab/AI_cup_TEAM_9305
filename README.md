# AI_cup_TEAM_9305
NKUST_EE_ML_期末報告&amp;AI_cup_競賽報告
本專案使用 Ultralytics YOLO (yolo 9m)於 Google Colab 上進行模型訓練與推論。  
train.ipynb 包含資料解壓縮、資料分割與模型訓練流程，資料以病人為單位切割，比例為 5:4:1（train/val/test）。  
訓練完成後，於 train 程式最後直接進行 test set評估。  
模型評估指標包含 Precision、Recall、mAP@0.5、mAP@0.5:0.95 及 IoU。  
predict.ipynb 用於載入訓練完成之模型（best.pt），  
對競賽資料進行推論並輸出參賽所需的預測 txt 檔案。  
整體流程參考 AI CUP 範例，但已調整訓練參數與資料切割方式。
