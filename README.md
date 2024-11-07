__目標__：建構並比較不同機器學習模型，以預測台股市場的交易訊號。

__做法__：

- 數據蒐集及整理：使用 FinMind API 蒐集台股歷史收盤資料，計算移動平均線
（MA）、KD指標等技術因子作為特徵。

- 模型建立與優化：
將技術指標作為特徵因子，策略多空作為目標變數，利用 scikit-learn 構建
多種機器學習模型。
使用箱形圖篩選最佳模型，並應用 GridSearchCV 進行參數調優。

- 結果分析：通過報酬率、因子重要度、混淆矩陣（confusion_matrix）等指標
評估模型表現。

__成就__：
最終模型達到 93% 的準確率
提升對關鍵因子的洞察力，並有效捕捉市場交易訊號。
