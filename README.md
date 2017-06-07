# Big-Data-Analytics-Homework2

每次Tune結果和程式的那裡作修改，都在程式碼裡用markdown做說明!

1. 請針對各個參數逐一進行分析，建議先固定某個參數，並逐步選擇最佳評估參數
	- XGBoost
		以下為Tune完後，各個最佳的參數
		- learning_rate =0.05
        - n_estimators=280
        - max_depth=5
        - min_child_weight=3
        - gamma=0
        - subsample=0.7
        - colsample_bytree=0.6,
        - reg_alpha=1e-7
        用merror來評分，test-merror-mean最低分數0.003222
	- Gradient Boosting
		以下為Tune完後，各個最佳的參數
		- learning_rate=0.005
		- n_estimators=3600
		- max_depth=5
		- min_samples_split=200
		- min_samples_leaf=70
		- subsample=0.9, random_state=10
		- max_features=310
		用accuracy來評分，CV Score最高分數0.9982778
2. 請留意binary與multi-class classification在評估上的差異 (Precision/Recall僅適合binary)
	因為資料集是multi-class，所以XGBoost、Gradient Boosting在程式的調整上都只有跑multi-class

