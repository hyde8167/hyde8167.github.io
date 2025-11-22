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
- コメント：
　- 報酬モデルの考え方が非常に参考になりました
  - Private Kaggleのデータセット、コンペ作成に時間を使い過ぎて途中リタイア状態になってしまいました
  - 行動ログの可視化・統計量分析、報酬モデル、Agent作成


### CMI Detect Behavior with Sensor Data（ジェスチャ分類）

- 内容：センサーデータを用いた行動認識タスク
- 技術スタック：
  - LightGBM / XGBoost / PyTorch
  - CPU/GPU 両対応パイプライン
- 工夫点：
  - 特徴量エンジニアリング（統計量・時系列分割）
  - クロスバリデーション設計としきい値最適化
- 成果：
  - Associate レベルを超えるベースライン改善　など

---

## FakeNews データセット / モデル開発

### FakeNews v11 データセット構築

- 内容：ニュース記事とフェイク記事（GPT 生成含む）の二値分類データセット
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

## 強化学習（RL） / シミュレーション

### Air Combat RL（R7Contest + HandyRL）

- 内容：航空戦シミュレーション環境上での agent 行動最適化
- 技術スタック：
  - HandyRL + Ray による分散学習
  - カスタム環境・報酬設計
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
