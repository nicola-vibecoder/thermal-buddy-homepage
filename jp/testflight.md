---
layout: default
title: ベータテスト（TestFlight）
published: false
---

{% include site-banner-lang.html %}

# Thermal Buddy iOS — ベータテスト — TestFlight

<p class="page-meta">Thermal Buddy をより良くするために、ご協力ありがとうございます。</p>

---

## ハイカーからハイカーへ

あの感覚、わかりますか？

深夜2時、テントの中で天井を見つめている。持ってきた服を全部重ね着しているのに、それでも寒い。またレイヤリングを間違えた。

あるいは山行の前日。ギアを広げながら考える。「去年の10月、似たようなルートを歩いたとき……テントの中で寒かったっけ？あのプリマロフトは持ってきてたっけ？十分だったっけ？」——でも、まったく思い出せない。

Thermal Buddy を作ったのは、そういう経験が積み重なったからです。

何度も同じ失敗をくり返した末に、記録をつけ始めました。気温、着ていたもの、実際の体感。シーンごとに。数ヶ月分のデータが溜まったとき、検索して「このコンディションで何が機能したか？」を振り返ることがいかに役立つかを実感しました。そして次の山行が、少しだけ良くなりました。その次も。

このベータは、アプリが一般公開される前に実際に使ってみる機会です。あなたはただのテスターではありません。ギアにこだわり、それをちゃんと記録しようとしている人です。だからこそ、あなたのフィードバックには特別な価値があります。

ぜひ、率直な意見を聞かせてください。

— Eiji

<a href="mailto:eiji@thermalbuddy.app" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;"><svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="flex-shrink:0;"><rect x="2" y="4" width="20" height="16" rx="2"/><polyline points="2,4 12,13 22,4"/></svg><span>eiji@thermalbuddy.app</span></a>

<a href="https://www.instagram.com/ultralight_for_espresso/" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;"><svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="flex-shrink:0;"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg><span>@ultralight_for_espresso</span></a>

---

## TestFlight でベータに参加する

<p class="cta-actions"><a href="https://testflight.apple.com/join/q2s2cH73" class="github-issue-button" style="font-size:18px;padding:14px 30px;">TestFlight で開く</a></p>

> **ベータ期間中は課金されません。** TestFlight 経由でのPremium購入はAppleのサンドボックス環境で処理されるため、実際の支払いは一切発生しません。
>
> **ベータの期間について。** 数週間を予定しています。終了時はTestFlightアプリから自動的に通知が届くので、ご安心ください。

---

## 特に聞きたいフィードバック

次の2つのシナリオを意識しながらテストしてみてください。

### 1. 山行後にログを記録する

帰ってきた直後、テント場やトレイルヘッドで。何を着ていたかを記録します。

- **Active シーン：** 歩いていたとき・走っていたとき・登っていたときの装備。
- **Rest・Sleep シーン：** 休憩や就寝時に何を追加したか、または入れ替えたか。特に夜のテント内。

*暑かった？寒かった？ちょうど良かった？* 記憶が新鮮なうちに記録してみてください。

**聞きたいこと：**
- Sleep シーンを追加する操作は直感的でしたか？わかりにくい部分はありましたか？
- ギアカテゴリは、自分の装備の整理方法と合っていましたか？
- 記録したかったのに、フィールドがなかった情報はありましたか？

### 2. 次の山行を計画する

数週間後、次のルートの準備をしている場面です。Search を開いて「5〜10℃の Sleep シーンで何を着ていたか？」と調べてみてください。

結果を見て、期待通りでしたか？自分の履歴が装備選びの参考になりましたか？

**聞きたいこと：**
- 検索結果を見て、装備の判断に自信が持てましたか？それとも迷いが残りましたか？
- アプリに答えてほしいけど、今は答えられない計画の問いはありましたか？
- 「あ、これ持っていかなきゃ」または「これは要らないな」と思えた過去のログはありましたか？

「こうだったらもっと使いやすいのに」と感じた瞬間——それが一番聞きたいことです。

---

## デベロッパーメニュー（テスト用ツール）

アプリ内に、サンプルデータを素早く読み込むための隠しツールがあります。テスター向けの機能です。

### ロック解除の方法

1. アプリを開き、**設定**（最後のタブ、歯車アイコン）に移動します。
2. 設定画面の一番下にある **About** セクションまでスクロールします。
3. **Build** の行を**素早く5回タップ**します。
4. ハプティクスのフィードバックが来て、**Data** セクションが About の上に表示されます。

再びロックするには、同じく Build を5回タップしてください。

### サンプルデータの読み込み

**Data** セクションには、2つのボタンがあります。

| ボタン | 内容 |
|--------|------|
| **Load App Store Data (EN)** | Search 機能を紹介するために設計された英語のサンプルログ一式。アプリを探索する際の出発点として最適です。 |
| **Load App Store Data (JA)** | 同じく Search 機能を紹介するために設計された日本語のサンプルログ一式。アプリを探索する際の出発点として最適です。 |

ボタンをタップして確認すると、サンプルログがすぐにログブックに追加されます。

### ⚠️ 注意：「全てのログを削除」はすべて消えます

**全てのログを削除** ボタンは、サンプルデータだけでなく、**自分で記録したすべてのログを含む、デバイス上の全ログを削除します**。この操作は取り消せません。

サンプルデータだけを削除したい場合は、ログブックで対象の記録を個別に削除してください（カードを左にスワイプすると削除ボタンが出ます）。

---

## 質問がある場合

[よくある質問 (FAQ)](faq.md) に、アプリの使い方が詳しく載っています。

バグを見つけた場合や機能のリクエストは、[GitHub Issues](https://github.com/nicola-vibecoder/thermal-buddy/issues) からお願いします。確実にトラッキングできる一番早い方法です。

---
{{ site.copyright }}
