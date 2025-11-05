---
title: "歩数の取得（Health Connect 連携）"
summary: "Android 13以降はHealth Connectが標準。連携の前提、許可、端末別の注意点を解説。"
slug: "steps"
weight: 20
tags: ["使い方","Health Connect","歩数"]
draft: false
# 旧URLからのリダイレクト（ここは実際の旧パスに合わせて）
aliases: ["/posts/steps-health-connect/", "/steps-health-connect/"]
---

## 1. 連携の前提
- Android 9 以上推奨。Android 13 以降は **Health Connect** が標準/ストア提供。
- Google Play 開発者サービス（GMS）が無い端末（例: 一部HUAWEI）は連携不可の場合があります。
- すでに Google Fit を使っている場合も **Health Connect** を経由する形で利用できます。

## 2. Health Connect を入れる
1. Google Play で **Health Connect** をインストール（Android 14 以降は設定内に統合されている場合あり）
2. 位置: *設定 → アプリ → Health Connect* または *Play ストア → Health Connect*

## 3. 権限を付与する
1. ステップくじを開き、ホームの案内から **歩数連携** をタップ  
2. Health Connect が開いたら、以下の権限を **許可**  
   - **歩数（Steps）**  
   - **アクティビティ** / **運動**（Activity / Exercise）  
   - 期間は *過去のデータを含む* を推奨  
3. アプリに戻り、**「歩数を取得」** をタップ → 1000歩ごとのゲージが埋まるか確認

## 4. よくある質問
### Q. 歩数が0のまま / 反映が遅い
- Health Connect の権限が **ON** か確認  
- 端末の **省電力/電池の最適化** でアプリが制限されていないか  
- 端末再起動 → Health Connect → ステップくじの順で再起動  
- 歩数は端末の**センサー/OS**に依存します。古い端末やスマートウォッチ側の設定で差が出る場合あり

### Q. 片方の端末では増えるが、もう片方で増えない
- 1アカウントで複数端末を使う場合、**最新の端末からの記録のみ採用**されることがあります  
- 同時利用は避け、**メイン端末を1つに**絞るのが確実

### Q. Google Fit を使いたい
- Health Connect を入れた上で Google Fit と接続すると、Fit → Health Connect → ステップくじ の順にデータが流れます  
- 反映に数分かかることがあります
