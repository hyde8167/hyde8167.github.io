---
title: "Projects"
permalink: /projects/
author_profile: true
---

## Kaggle / コンペティション

### 第４回 空戦AIチャレンジ 2025/11
- 内容：航空戦シミュレーション環境上での agent 行動最適化
- 121位/1680チーム
<img width="1137" height="90" alt="image" src="https://github.com/user-attachments/assets/428007a0-c984-44c1-8493-e1ad04f60b65" />
- 技術スタック：
  - Agentモデル / 報酬モデル
- コメント：
　- 報酬モデルの考え方が非常に参考になりました
  - Private Kaggleのデータセット、コンペ作成に時間を使い過ぎて途中リタイア状態になってしまいました
  - 行動ログの可視化・統計量分析、報酬モデル、Agent作成

### 第1回 国土交通省 地理空間情報データチャレンジ 2024/11
- 内容：不動産の賃料を予測するモデルの構築
- 42位/452チーム
<img width="1176" height="98" alt="image" src="https://github.com/user-attachments/assets/15aba831-269a-44d5-8520-1b66d7b999ed" />
- 技術スタック：
  - LightGBM / XGBoost / catboost　/ensemble
- コメント：
　- データ量とデータの汚れにかなり苦戦
  - 一番スコアに聞いたのが欠損処理、異常値処理でした
  - lightGBM,catboost,xgboost,ensemble


### CMI Detect Behavior with Sensor Data（ジェスチャ分類）

- 内容：センサーデータを用いた行動認識タスク
- 技術スタック：
  - LightGBM / XGBoost / PyTorch
  - CPU/GPU 両対応パイプライン
  - 特徴量エンジニアリング（統計量・時系列分割）
- 成果：
  - Associate レベルを超えるベースライン改善
- コメント：
　- 参加しただけの状態
  - 一番スコアに聞いたのが欠損処理、異常値処理でした

---

## イベント・コンペ開催

### FakeNewsの検出チャレンジ [Kaggle/Private]
- 内容：ニュース記事とフェイク記事（GPT 生成含む）の二値分類データセットを作成、有志コンペ開催
- 技術スタック：
  - Python（pandas, scikit-learn, LightGBM）
  - NLP 前処理・要約・翻訳パイプライン
- 主な特徴量：
  - タイトル・本文の長さ、句読点・感嘆符の数
  - 投稿者ごとのフォロワー統計（log・国別正規化）
  - 投稿時間帯・休日フラグ など
- 成果：
  - PR-AUC / AUC を指標としたベースラインモデル構築
  - 特徴重要度・SHAP による説明可能性の確保

---

## イベント等

### AI Quest [2021]
- 内容：PBL（Project-Based Learning)形式での経済産業省主催の教育プログラム
- 修了/第1タームプレゼン課題優秀賞/第2タームプレゼン課題優秀賞
- 技術スタック：
  - 機械学習基礎
- 工夫点：
  - 学習済みモデルの重み読み込み / 外部エージェント連携
  - 行動ログの可視化・統計量分析

---

## AWS アーキテクチャ設計

### Dify / Webアプリの AWS ホスティング

- 内容：Dify 等の Web アプリを AWS 上で安定稼働させる構成
- 構成例：
  - VPC + Public / Private Subnet
  - ALB or CloudFront + EC2
  - NAT Gateway / Bastion host
- 成果：
  - コスト・可用性・運用容易性のバランスを取った構成案
  - PPT 資料としての図版・説明資料を作成
