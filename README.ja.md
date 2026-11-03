# AID Studio — AI ドラマ＆モーションコミック制作

[English](README.md) · **日本語** · [扫码加入开源交流群](#コミュニティとフィードバック)

**AID Studio は、AI ショートドラマ、映画、コミック向けのオープンソースの AI モーションコミック制作プラットフォームで、脚本や絵コンテから動画、ボイスオーバーまでのエンドツーエンドのワークフローを備えています。**

オープンソースでセルフホスト可能な AI ドラマ＆モーションコミック制作。脚本や絵コンテから動画、ボイスオーバーまで対応し、映画やコミックの制作もサポートします。

<p align="center">
  <a href="https://www.aidstudio.com.cn/"><strong>オンラインで試す</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="#クイックスタート"><strong>AID をデプロイ</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://gzxxaitdb.feishu.cn/docx/LZ5zdesEgo1z4Mxc7OWc7zTHnJc"><strong>ユーザーチュートリアル</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/gzxx-2025/aid-studio/releases"><strong>リリース</strong></a>
  &nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="SUPPORT.md"><strong>ヘルプ</strong></a>
</p>

<p align="center">
  <a href="#製品プレビュー">
    <img src="references/web/2.png" alt="AID ワークフローキャンバス：脚本、アセット、絵コンテ、動画制作を視覚的に整理" width="100%">
  </a><br>
  <sub>実際のワークフローキャンバスのスクリーンショット · <a href="#製品プレビュー">その他の製品スクリーンショットを見る</a></sub>
</p>

<a id="交流与反馈"></a>

## コミュニティとフィードバック

デプロイ、モデルの設定、カスタマイズ、制作ワークフローとの連携に関する質問は、[ヘルプ](SUPPORT.md) に記載のチャンネルを利用するか、QR コードをスキャンしてコミュニティチャットに参加してください。

**扫码加入 AID 开源交流群（中文交流 / 技术支持入口）**

本群仅仅为开源交流、技术支持群，无广告，无任何隐形消费。

このグループはオープンソースに関する交流と技術サポート専用で、広告や隠れた料金は一切ありません。

<p align="center">
  <img src="https://img.shields.io/badge/交流群说明-%E6%9C%AC%E7%BE%A4%E4%BB%85%E4%BB%85%E4%B8%BA%E5%BC%80%E6%BA%90%E4%BA%A4%E6%B5%81%E3%80%81%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81%E7%BE%A4%EF%BC%8C%E6%97%A0%E5%B9%BF%E5%91%8A%EF%BC%8C%E6%97%A0%E4%BB%BB%E4%BD%95%E9%9A%90%E5%BD%A2%E6%B6%88%E8%B4%B9%E3%80%82-d93025?style=for-the-badge" alt="オープンソースの交流と技術サポートのみ。広告や隠れた料金はありません。本群仅仅为开源交流、技术支持群，无广告，无任何隐形消费。">
</p>

<p align="center">
  <a href="references/community-qr.png">
    <img src="references/community-qr.png" alt="AID オープンソースコミュニティの QR コード — 扫码加入开源交流群" width="220">
  </a><br>
  <sub>扫码进群：如果二维码未直接显示，可点击二维码区域查看原图。<br>QR コードをスキャンしてコミュニティチャットに参加してください。QR コードが表示されない場合は、QR コードの領域をクリックすると元の画像を開けます。</sub>
</p>

<a id="赞助商"></a>

<a id="核心能力"></a>

## 主な機能

- **完全な制作ワークフロー**：脚本、キャラクター、シーン、絵コンテ、画像、動画、ボイスオーバーを 1 つのプロジェクト内で整理できます。
- **複数のモデル**：テキスト、画像、動画、音声のモデルを必要に応じて設定できます。利用できる機能は選択したモデルによって異なります。
- **制御されたモデル呼び出し**：固定のモデルパラメーター、実行時の推論オプション、リクエストのマッピングを明確な優先順位のルールに従って組み合わせます。見積もり前に特定できる設定エラーは、プロバイダーへの送信前に拒否されます。
- **セルフホストと管理**：Docker または systemd でインストールでき、モデル、タスク、ユーザー、アップグレードの管理機能が統合されています。

> ソースコードは MIT License の下で公開されています。AI による生成には、各プロバイダーの API 認証情報が必要です。モデルの呼び出し、サーバー、ストレージには費用が発生する場合があり、生成の品質はモデルと入力アセットに依存します。

[最初のモーションコミックプロジェクト](#最初のモーションコミックプロジェクト) · [AID をデプロイ](#クイックスタート) · [製品のスクリーンショット](#製品プレビュー) · [技術とソースコード](#公開ソースコードの構成) · [ドキュメント](#ドキュメント)

<a id="aid-用来做什么"></a>

## AID の用途

AID は **AI モーションコミックとショートドラマ** に特化しており、映画的なショートフィルムや静止画のコミックにも対応しています。クリエイターは脚本、エピソード、アセット、生成結果を同じプロジェクト内で管理でき、チームや開発者はプラットフォームをセルフホストして独自のモデルを設定できます。

<a id="三大核心创作方向"></a>

## 3 つの主な制作ワークフロー

| ワークフロー | 制作できるもの |
| --- | --- |
| **AI モーションコミック / ショートドラマ** | エピソードの脚本、キャラクターとシーンのアセット、絵コンテ画像、動画クリップ、キャラクターのボイスオーバー、完成動画のプレビュー |
| **AI 映画 / ショートフィルム** | ショットの計画、参照アセットの整理、動画生成、映像と音声の制作 |
| **AI コミック** | ストーリーとキャラクターの構築、連続した絵コンテ画像、静止画コミックのアセット管理 |

ワークフローに沿った制作とワークフローキャンバスは、別々の入り口です。ご自身の制作スタイルに合ったものを選んでください。冒頭のスクリーンショットは、既存のワークフローキャンバスを示しています。

<a id="第一个漫剧项目"></a>

## 最初のモーションコミックプロジェクト

エピソード全体に広げる前に、まず絵コンテのショットを 1 つ完成させましょう：

1. **モデルを準備する**：AID をデプロイした後、管理画面でテキストモデルと画像モデルを設定します。動画やボイスオーバーが必要な場合は、動画モデルと音声モデルを追加します。有効にする前に、それぞれの機能、認証情報、費用を確認してください。
2. **プロジェクトを作成する**：短い脚本を用意してエピソードを作成し、キャラクターとシーンを整理します。
3. **参照アセットを準備する**：使用する権利のあるキャラクターやシーンの画像を生成またはアップロードします。
4. **絵コンテのショットを 1 つ完成させる**：絵コンテの脚本と画像を確認し、設定済みの動画モデルを選んでクリップを生成します。
5. **ボイスオーバーを追加してプレビューする**：必要に応じてボイスオーバーを追加し、映像と音声を確認してから、次のショットに進みます。

静止画のコミックの場合は、動画とボイスオーバーの手順を省略してください。ページごとの説明は [ユーザーチュートリアル](https://gzxxaitdb.feishu.cn/docx/LZ5zdesEgo1z4Mxc7OWc7zTHnJc)、インストールに関する質問は [デプロイガイド](deploy/README.md)、その他の質問は [ヘルプ](SUPPORT.md) をご覧ください。

<a id="功能特性"></a>

## 機能

<details>
<summary>制作ワークフローとプラットフォームの全機能を表示</summary>

**エンドツーエンドの AI 制作**

- 脚本とエピソード：プロジェクト、脚本、エピソードの管理、AI による脚本作成の支援、シーンアセットの抽出
- キャラクター、小道具、シーン：ビジュアルアセットライブラリ、参照画像の管理、キャラクターへの音声の割り当て
- 絵コンテのワークベンチ：絵コンテの脚本生成、絵コンテ画像の生成、ショットグループの分割、動画プロンプトの生成
- 画像生成：テキストからの画像生成、画像からの画像生成、複数画像の融合。参照画像のプレースホルダーを一貫して処理します
- 動画生成：画像からの動画生成、最初と最後のフレームの指定、複数ショットの一括生成。解像度、長さ、アスペクト比はモデルの機能に照らして検証されます
- 音声合成：複数の声による TTS、ボイスライブラリの管理、リップシンク

**プラットフォームの機能**

- マルチプロバイダーのオーケストレーション：テキスト、画像、動画、音声のモデル向けの統一された Provider。モデルの機能、参照画像の数、解像度、長さ、アスペクト比を設定できます
- API ゲートウェイの設定：互換性のあるプロトコル向けにモデルのエンドポイントと認証情報を設定でき、モデルごとに上書きできます
- 統一されたタスクシステム：生成キュー、同時実行のスケジューリング、進捗の更新、リトライ、補償処理、結果の取得
- ビジュアルの一貫性：キャラクター、小道具、シーンのアセットを再利用し、公式/カスタムのスタイルとプロジェクトのスタイルスナップショットを使用し、モデルの機能の範囲内で参照画像を安全に整理します
- 課金：モデル/SKU ベースの課金、残高の凍結と精算、チャージパッケージ、Alipay/WeChat Pay
- ユーザーアカウント：アカウント、SMS、メール、WeChat の QR コードによるログイン、本人確認、紹介インセンティブ
- 管理：モデル、プロバイダー、エージェント、プロンプト、コンテンツ、注文、ユーザー、ストレージ、プラットフォーム設定の一元管理
- 本番運用：Docker と systemd によるデプロイ、内部または外部のミドルウェア、HTTPS、設定のバックアップ、診断、完全なアンインストール
- オンラインアップグレード：独立した `aid-updater` を使い、UI または CLI のどちらからでも更新の確認、リアルタイムの進捗の確認、ロールバックができます

</details>

<a id="快速开始"></a>

## クイックスタート

<a id="生产部署"></a>

### 本番環境へのデプロイ

新しい 64 ビットの Linux サーバーから始めてください。RocketMQ を無効にし、ミドルウェアを同じホストに置く場合、最小要件は **2 CPU コア / 4 GB RAM / 40 GB ディスク** です。その他の容量要件とインストールオプションについては、[デプロイガイド](deploy/README.md) をご覧ください。

以下のコマンドは、インストーラーを `/root/aid-install.sh` に保存します。まず Gitee からダウンロードし、失敗した場合は自動的に GitHub にフォールバックします。スクリプトはダウンロードに成功した場合にのみ実行されます。初回インストール時は、まず設定が生成されます。**初期化とサービスの起動に進む前に、設定を確認して承認してください。**

```bash
cd /root && if command -v curl >/dev/null 2>&1; then curl -fL --retry 3 --connect-timeout 15 -o /root/aid-install.sh https://gitee.com/gzxx-2025/aid-studio/raw/master/deploy/aid.sh || curl -fL --retry 3 --connect-timeout 15 -o /root/aid-install.sh https://raw.githubusercontent.com/gzxx-2025/aid-studio/master/deploy/aid.sh; elif command -v wget >/dev/null 2>&1; then wget -O /root/aid-install.sh https://gitee.com/gzxx-2025/aid-studio/raw/master/deploy/aid.sh || wget -O /root/aid-install.sh https://raw.githubusercontent.com/gzxx-2025/aid-studio/master/deploy/aid.sh; else echo 'Please install curl or wget first'; exit 1; fi && sudo env AID_REMOTE_BOOTSTRAP=1 AID_RELEASE_CHANNEL=auto bash /root/aid-install.sh install
```

インストール後、`sudo aid default` を実行してアクセス URL を確認します。**初回ログイン後、ただちに管理者パスワードを変更してください。** 管理画面で必要なモデルを設定して有効にし、[最初のモーションコミックプロジェクト](#最初のモーションコミックプロジェクト) に進んでください。

<details>
<summary>デプロイオプション、リソース要件、管理コマンドを表示</summary>

`install` は自動判定のエントリーポイントです。AID がデプロイされていない場合はデフォルトで Docker による初回インストールを行い、すでにデプロイされている場合は更新を確認します。デプロイモードを明示的に選ぶこともできます：

```bash
sudo env AID_REMOTE_BOOTSTRAP=1 AID_RELEASE_CHANNEL=auto bash /root/aid-install.sh install-docker
sudo env AID_REMOTE_BOOTSTRAP=1 AID_RELEASE_CHANNEL=auto bash /root/aid-install.sh install-manual
```

`auto` は安定版を優先し、インストール可能な安定版がない場合にのみ、通知を表示したうえで Beta にフォールバックします。安定版チャンネルにとどまるには `stable` を使い、プレリリース版を明示的にテストしたい場合にのみ `beta` を使ってください。

| デプロイモード | 適した用途 | 正となる設定 | ランタイム |
|---------|---------|---------|---------|
| Docker（推奨） | 新しいサーバー、およびミドルウェア/ランタイム環境を分離したい場合 | `/data/aid/config/docker.env` | Docker Compose |
| 手動デプロイ | 既存のホスト、BaoTa パネル、または systemd ベースの運用 | `/data/aid/aid-deploy.conf` | systemd + Nginx |

初回デプロイでは設定が生成され、管理者による確認と承認が必要です。**設定が承認されるまで、インストーラーは統合ソースコードの取得、プログラムのビルド、データベースの初期化、サービスの起動を行いません。** コード、依存関係、イメージには中国からアクセスしやすいソースを優先し、必要に応じて公式のソースにフォールバックします。サーバー、管理画面のフロントエンド、Web フロントエンド、アップデーターは同じバージョンタグからビルドされ、完全なログは `/data/aid/logs/` に書き出されます。互換性のあるバージョンの既存の依存関係は再利用され、不完全なキャッシュ済みのダウンロードは再検証されて再ダウンロードされます。

Docker モードは、内蔵または外部の MySQL 5.7、内蔵または外部の Redis、任意の RocketMQ、任意の HTTPS に対応しています。外部の MySQL を設定すると、内蔵の MySQL サービスは起動しません。Redis のユーザー名、パスワード、データベースのインデックスはすべて空でもかまいません。RocketMQ を無効にした場合、MQ は起動も検証もされません。有効にした場合は、外部の NameServer と ACL を設定できます。手動モードでは、必要に応じて JDK、Git、Maven、Node.js、Go、Nginx、MySQL 5.7、Redis を用意します。外部のミドルウェアは接続性のみがチェックされ、RocketMQ は管理者が自分で用意する必要があります。

HTTPS には、ユーザー向けと管理画面用のドメイン、ポート 443、完全な証明書チェーン、秘密鍵が必要です。証明書のデフォルトの場所は `/data/aid/config/ssl/` です。管理画面の「Project Upgrade Configuration → Runtime Configuration」で、証明書のアップロード、ドメインの設定、DNS・証明書・HTTPS の個別テストを行うこともできます。`HTTP_PORT=443` を設定するだけでは、TLS は自動的には有効になりません。

デプロイ後は、どちらのインストールモードでも同じ管理コマンドを使います：

| コマンド | 用途 |
|------|------|
| `sudo aid` | 対話式の管理メニューを開く |
| `sudo aid default` | パブリック/プライベートネットワークのユーザー向けおよび管理画面の URL と、初期アカウント情報を表示する |
| `sudo aid status` | サービス、ミドルウェア、アップデーターの状態を確認する |
| `sudo aid logs` | 実行時のログを表示する |
| `sudo aid config` | 現在のデプロイ設定を編集し、案内に従って適用する |
| `sudo aid restart` | 設定を再読み込みしてサービスを再起動する |
| `sudo aid update` | 現在のチャンネルの更新を確認して適用する |
| `sudo aid progress` | アップグレード、アップデーターの更新、ロールバックの進捗をリアルタイムで表示する |
| `sudo aid rollback` | 公式にロールバックが許可されている過去のバージョンを選択する |
| `sudo aid backup` | デプロイのバックアップを作成する |
| `sudo aid mysql` | 現在の MySQL の接続情報を表示する |
| `sudo aid uninstall --keep` | データと設定を残したままプログラムをアンインストールする |
| `sudo aid uninstall --purge` | 2 回目の確認の後、AID のデータを完全に削除する |

**サーバーのリソース要件**（インストーラーが自動的にチェックします。最小要件を下回る場合は、現在のリソースを表示して `y/n` で確認を求めます）：

| デプロイ | 最小 | 推奨 |
|---------|---------|---------|
| ローカルの Docker フルスタック（RocketMQ 無効） | 2 コア、4 GB RAM / 40 GB ディスク | 4 コア、8 GB RAM / 100 GB 以上のディスク |
| ローカルの Docker フルスタック（RocketMQ 有効） | 4 コア、4 GB RAM / 40 GB ディスク | 6 コア、12 GB RAM / 100 GB 以上のディスク |
| ローカルの手動デプロイ（ミドルウェアを同じホストに配置） | 2 コア、4 GB RAM / 40 GB ディスク | 4 コア、8 GB RAM / 100 GB 以上のディスク |
| ローカルの手動デプロイ（RocketMQ 有効） | 4 コア、4 GB RAM / 40 GB ディスク | 6 コア、12 GB RAM / 100 GB 以上のディスク |

RocketMQ を有効にした場合の 4 コア/4 GB という最小要件は、ローカルでのセットアップと機能検証のみを想定しており、JVM/MQ の設定を縮小する必要があります。メッセージ量が多い場合や MQ ベースのディスパッチを行う場合は、6 コア/12 GB 以上を推奨します。チューニングについては、[デプロイガイド](deploy/README.md) の「Configuration Requirements」をご覧ください。メディアファイルには OSS/COS のオブジェクトストレージを強く推奨します。ローカルディスクはフォールバックとしてのみ使われます。


</details>

<details>
<summary>ローカル開発と管理画面へのアクセス方法を表示</summary>

<a id="本地开发"></a>

### ローカル開発

要件：JDK 17 以上、Maven 3.6 以上、Docker（ミドルウェア用）。

```bash
# 1. Start the development environment (MySQL + Redis; automatically imports the initialization scripts in sql/)
cd deploy/docker
docker compose -f docker-compose.middleware.yml up -d
# To include RocketMQ for integration testing, use:
# docker compose -f docker-compose.middleware.yml --profile mq up -d

# 2. Build and start the backend (development defaults match the environment above; no configuration changes are needed)
cd ../..
mvn clean package -DskipTests
java -jar aid-admin/target/aid-admin.jar
```

`http://localhost:8080` にアクセスしてサービスを確認します。データベースの初期化により、管理者アカウント `admin / admin123` が作成されます。初回ログイン後、ただちにパスワードを変更してください。

バックエンドのすべての環境設定は、環境変数で上書きできます：`DB_*`、`REDIS_*`、`TOKEN_SECRET`（**本番環境では強力なランダム値が必須です**）、`AID_PROFILE`、`ROCKETMQ_ENABLED`（RocketMQ をデプロイしていない場合は `false` に設定すると、MQ の接続を完全に無効にしてローカルのタスクモードを使います）、`ROCKETMQ_NAMESERVER`。

<a id="默认访问与后台访问码"></a>

### デフォルトの URL と管理画面のアクセスコード

本番環境へのデプロイ後、デフォルトの URL は次のとおりです（実際のポートとランダムなアクセスコードは `sudo aid default` の出力を参照してください）：

| エントリーポイント | デフォルトの URL | 備考 |
|------|---------|------|
| ユーザー向けフロントエンド | `http://SERVER_IP/` | デフォルトはポート 80。`HTTP_PORT` で変更できます |
| 管理画面のフロントエンド | `http://SERVER_IP:8089/<RANDOM_ACCESS_CODE>` | デフォルトはポート 8089。初回デプロイ時に 12 文字のランダムなアクセスコードが生成され、完全な URL が出力されます |
| バックエンド API | `http://SERVER_IP:8080/` | デフォルトはポート 8080。通常は Nginx のリバースプロキシ経由でアクセスします |

データベースの初期化により、管理者アカウント `admin / admin123` が作成されます。初回デプロイでは、公開されている固定のエントリーパスは使用されず、インストーラーが 12 文字のランダムなアクセスコードを生成します。初回ログイン後、ただちに管理者パスワードを変更してください。アクセスコードは「Global Business Configuration → Login and Authentication → Admin Login Entry」で再生成できます。`sudo aid default` が表示するのは初期アカウント情報のみで、すでに変更された管理者パスワードを照会したりリセットしたりすることはありません。

ランダムな管理画面のエントリーを有効にしている場合は、ログイン URL を次のように組み立てます：

```text
http://SERVER_IP:8089/<ACCESS_CODE>
```

例（デプロイ後に出力された実際のアクセスコードを使ってください）：

```text
http://localhost:8089/Ab12Cd34Ef56
```

ドメインと HTTPS を設定している場合も、同じように管理サイトのルートパスにアクセスコードを付け加えます：

```text
https://admin.example.com/Ab12Cd34Ef56
```

デプロイ後、インストーラーは現在データベースに保存されている管理画面の完全なログイン URL を出力します。アクセスコードを忘れた場合は、`aid_config` テーブルで `category = 'admin_entry'` かつ `config_name = 'access_code'` のレコードを照会するか、ログイン後に再生成して保存してください。


</details>

<a id="配置-ai-厂商"></a>

### AI プロバイダーの設定

公開リポジトリには、管理画面のフロントエンドとユーザー向けの制作フロントエンドのソースコードが、それぞれ [`frontend/admin`](https://github.com/gzxx-2025/aid-studio/tree/main/frontend/admin) と [`frontend/web`](https://github.com/gzxx-2025/aid-studio/tree/main/frontend/web) に含まれています。起動後、管理画面の「AI Model Configuration」でプロバイダーの認証情報、モデルの機能、課金ルールを設定し、モデルを有効にします。動画やボイスオーバーのワークフローには、対応する動画モデルと音声モデルも必要です。

<a id="产品预览"></a>

## 製品プレビュー

> README の画像はリポジトリからの相対パスを使用しており、Gitee と GitHub の両方で直接表示されます。ページの読み込みが遅い場合は、ブラウザーが画像のキャッシュを終えるまでお待ちください。

<a id="用户端创作工作台"></a>

### ユーザー向け制作ワークベンチ

プロジェクトの作成、脚本の執筆、ワークフローキャンバス、キャラクター/シーンのアセット管理から、絵コンテの生成、動画、ボイスオーバー、完成動画のプレビューまで、ユーザー向けフロントエンドは AI モーションコミック、AI 映画、AI コミックのための一貫したワークフローを提供します。

<p align="center">
  <img src="references/web/0.png" alt="AID のユーザーログインと事例ギャラリー" width="92%">
</p>

| 制作の入り口 | マイ作品 |
|-------------|---------|
| <img src="references/web/1.png" alt="AID の AI コンテンツ制作の入り口" width="100%"> | <img src="references/web/14.png" alt="ユーザー向けフロントエンド：マイ作品" width="100%"> |

| プロジェクトの設定とスタイルの選択 | ワークフローに沿った脚本の執筆 |
|-------------------|---------------|
| <img src="references/web/15.png" alt="プロジェクトの設定とスタイルの選択" width="100%"> | <img src="references/web/3.png" alt="ワークフローに沿った脚本の執筆" width="100%"> |

| ワークフローキャンバス | シーンとアセットの管理 |
|---------|---------------|
| <img src="references/web/2.png" alt="プロジェクトのワークフローキャンバス" width="100%"> | <img src="references/web/4.png" alt="シーンとアセットの管理" width="100%"> |

| 画像の編集と参照アセット | 生成モデルの設定 |
|-------------------|-------------|
| <img src="references/web/5.png" alt="画像の編集と参照アセット" width="100%"> | <img src="references/web/6.png" alt="生成モデルの設定" width="100%"> |

| 絵コンテのデザイン | 絵コンテ動画の管理 |
|---------|-------------|
| <img src="references/web/7.png" alt="絵コンテのデザインと参照画像" width="100%"> | <img src="references/web/8.png" alt="絵コンテ動画の管理" width="100%"> |

| 複数のパラメーターによる動画生成 | 音声と映像の同期 |
|----------------|-------------|
| <img src="references/web/9.png" alt="複数のパラメーターによる動画生成" width="100%"> | <img src="references/web/10.png" alt="音声と映像の同期の管理" width="100%"> |

| ボイスオーバーの編集 | ボイスオーバーのキャラクター選択 |
|---------|-------------|
| <img src="references/web/11.png" alt="ボイスオーバーの編集とプレビュー" width="100%"> | <img src="references/web/12.png" alt="ボイスオーバーのキャラクター選択" width="100%"> |

<p align="center">
  <img src="references/web/13.png" alt="動画のタイムラインと完成動画のプレビュー" width="92%">
</p>

<a id="管理端运营后台"></a>

### 管理ダッシュボード

管理画面のフロントエンドは、プラットフォームの概要、ユーザーと作品の管理、AI モデルとプロバイダーの設定、タスクの監視、支払いと課金、システムのアップグレードなどの管理機能をカバーしています。

<p align="center">
  <img src="references/manager/0.png" alt="AID 管理画面のログイン入り口" width="92%">
</p>

| データの概要 | 生成タスクの監視 |
|---------|-------------|
| <img src="references/manager/1.png" alt="管理画面のデータの概要" width="100%"> | <img src="references/manager/2.png" alt="生成タスクの監視" width="100%"> |

| ユーザー管理 | コンテンツ詳細の審査 |
|---------|-------------|
| <img src="references/manager/3.png" alt="ユーザー管理" width="100%"> | <img src="references/manager/4.png" alt="コンテンツ詳細の審査" width="100%"> |

| AI モデルの設定 | AI ワークフローのオーケストレーション |
|------------|-------------|
| <img src="references/manager/5.png" alt="AI モデルの設定" width="100%"> | <img src="references/manager/6.png" alt="モデルプール、エージェント、戦略マトリクスのオーケストレーション" width="100%"> |

| オンラインアップグレードとリリースノート | オンラインユーザーの監視 |
|-------------------|-------------|
| <img src="references/manager/7.png" alt="オンラインアップグレードとリリースノート" width="100%"> | <img src="references/manager/8.png" alt="オンラインユーザーの監視" width="100%"> |

<p align="center">
  <img src="references/manager/9.png" alt="サービス、キャッシュ、実行時リソースの監視" width="92%">
</p>

<a id="公开源码目录"></a>

## 公開ソースコードの構成

公開されている `aid-studio` リポジトリは、AID の統合ソースコードとデプロイ用リリースのエントリーポイントです。バックエンド、管理画面のフロントエンド、ユーザー向けの制作フロントエンド、バージョンマニフェスト、デプロイスクリプト、差分 SQL、独立したアップデーターが含まれています。3 つのアプリケーションコンポーネントはすべて同じバージョンタグを共有します。

統合された公開ソースは [Gitee aid-studio](https://gitee.com/gzxx-2025/aid-studio) と [GitHub aid-studio](https://github.com/gzxx-2025/aid-studio) で公開されており、両プラットフォームでコミットとタグは同一です。

| パス | 内容 |
|------|------|
| `/` | Java バックエンド、初期化 SQL、デプロイスクリプト、アップデーター |
| `frontend/admin/` | 管理画面のフロントエンド（React） |
| `frontend/web/` | ユーザー向けの制作フロントエンド |

`v1.0.1` 以降、新しいバージョンではこのリポジトリの対応するバージョンタグを使用します。過去のバージョンを取得または移行する前に、該当するリリースノートを確認してください。アップグレード、バックアップ、利用可能なロールバックの範囲については、[デプロイガイド](deploy/README.md) をご覧ください。

<a id="官方资产包"></a>

## 公式アセットバンドル

AID の初期化データは、初回デプロイ後のプラットフォームの初期表示と制作例のために、公式のメディアリソースを参照しています。これには、キャラクター、シーン、小道具、ライティング、ショットサイズ/焦点距離、ポーズ、表情、エフェクト、絵コンテの例、エージェントとプロバイダーのアイコン、ボイスのアバターと MP3 サンプル、ホームページの画像、デモ動画が含まれます。この大容量のアセットバンドルは、ソースコードとは別に配布されています。公開コードホスティングの帯域を消費したり、デプロイする人の OSS/COS ストレージに誤って書き込んだりしないよう、GitHub/Gitee の Releases やワンコマンドのデプロイでは自動的にダウンロードされません。

- バンドルには、`aid_init` 初期化データベースが実際に参照している公式ファイルのみが含まれます。ユーザーが生成したコンテンツ、アカウント、キー、ログ、その他の業務データは含まれません。
- データベースが使用する元のオブジェクトキーは `files/aid/...` 以下に保持されています。初期化 SQL を一括で書き換えることなく、1 回の操作でバンドルをローカルストレージ、Alibaba Cloud OSS、Tencent Cloud COS にインポートできます。
- 各ファイルはバンドル内の `manifest.json` と `asset-checksums.txt` に記載されており、パス、サイズ、SHA-256 による整合性チェックが可能です。
- ダウンロードのエントリーポイントとバージョンごとのチェックサムは、[公式サイト](https://www.aidstudio.com.cn/) とリリースのお知らせで公開されています。アプリケーションのバージョンに合った `aid-official-assets_<VERSION>.tar.gz` を選んでください。インポートのコマンドはバンドル内の `README.md` に記載されています。

<a id="系统架构"></a>

## システムアーキテクチャ

<details>
<summary>システムアーキテクチャと技術スタックを表示</summary>

<p>
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
  <img src="https://img.shields.io/badge/Java-17-orange.svg" alt="Java">
  <img src="https://img.shields.io/badge/Spring%20Boot-3.5-brightgreen.svg" alt="Spring Boot">
  <img src="https://img.shields.io/badge/MySQL-5.7-4479A1.svg" alt="MySQL">
  <img src="https://img.shields.io/badge/MyBatis--Plus-3.5-red.svg" alt="MyBatis-Plus">
  <a href="https://github.com/gzxx-2025/aid-studio/actions/workflows/backend-build.yml"><img src="https://github.com/gzxx-2025/aid-studio/actions/workflows/backend-build.yml/badge.svg?branch=main" alt="Backend build"></a>
  <a href="https://github.com/gzxx-2025/aid-studio/actions/workflows/admin-build.yml"><img src="https://github.com/gzxx-2025/aid-studio/actions/workflows/admin-build.yml/badge.svg?branch=main" alt="Admin build"></a>
  <a href="https://github.com/gzxx-2025/aid-studio/actions/workflows/web-build.yml"><img src="https://github.com/gzxx-2025/aid-studio/actions/workflows/web-build.yml/badge.svg?branch=main" alt="Web build"></a>
</p>

```text
aid-studio (Maven multi-module monolith)
├── aid-admin        Spring Boot entry point and configuration
├── aid-common       Shared components (security/cache/storage/payments/SMS adapters)
├── aid-business     Web layer
│   ├── business-framework   Web framework, data sources, filters and AOP
│   ├── business-system      Admin APIs (/system /aid /aidconfig)
│   ├── business-main        User APIs (/auth /api/user /recharge)
│   ├── business-quartz      Scheduled tasks
│   └── business-generator   Code generation
├── aid-interface    Domain layer
│   ├── interface-core       Core interfaces
│   ├── interface-system     Entities, Mappers and system services
│   └── interface-main       Business services (media/storyboards/billing/upgrades, etc.)
├── aid-consumer     MQ consumers
├── deploy/updater   Standalone updater (Go)
└── frontend
    ├── admin        Admin frontend (React)
    └── web          User creation frontend
```

呼び出しの流れ：`Controller → Service → Mapper → MySQL`。メディアの生成は、統一されたオーケストレーション層を通じて各プロバイダーの実装にルーティングされます。

<a id="技术栈"></a>

## 技術スタック

| カテゴリ | 技術 | バージョン |
|------|------|------|
| 言語 | Java | 17 |
| フレームワーク | Spring Boot | 3.5.x |
| ORM | MyBatis-Plus | 3.5.x |
| データベース | MySQL | 5.7 |
| キャッシュ | Redis + Redisson | 3.x |
| メッセージキュー | RocketMQ | 4.x/5.x |
| スケジュールタスク | Quartz | 2.5.x |
| オブジェクトストレージ | Alibaba Cloud OSS / Tencent Cloud COS | - |
| API ドキュメント | SpringDoc OpenAPI | 2.8.x |
| アップデーター | Go | 1.22 |

</details>

<a id="文档导航"></a>

## ドキュメント

| ドキュメント | 説明 |
|------|------|
| [デプロイガイド](deploy/README.md) | Docker / systemd によるデプロイ、設定、HTTPS、ミドルウェア、アップグレード、ロールバック、アンインストール |
| [英語版の概要](README.md) | 英語での概要、インストール、最初のプロジェクト、メンテナンス |
| [コントリビューションガイド](CONTRIBUTING.md) | 問題の報告、変更の範囲、開発時の検証、PR の提出 |
| [公開 Provider 接続ガイド](doc/公开Provider接入指南.md) | テキスト/画像/動画/音声の Provider のエントリーポイント、機能の宣言、統一されたタスクと課金、公式プロトコルの検証、提出前のチェック（[English](doc/public-provider-integration.md)） |
| [ヘルプ](SUPPORT.md) | 使い方、デプロイ、モデルの設定に関する質問のサポートチャンネル |
| [セキュリティの報告](SECURITY.md) | 機密情報を公開せずに脆弱性を非公開で報告する |
| [行動規範](CODE_OF_CONDUCT.md) | コミュニティでのコミュニケーションと協力のガイドライン |
| Swagger API ドキュメント | 起動後に `http://localhost:8080/swagger-ui.html` にアクセスします（本番環境ではデフォルトで無効） |

<a id="在线升级"></a>

## オンラインアップグレード

管理画面の「System Management → Project Upgrade Configuration」と CLI は、同じ独立したアップデーターを使用します。このページには、現在のバージョン、オンラインのバージョン、二か国語のリリースノート、アップデーターの状態、利用可能なロールバックのバージョン、黒いリアルタイムのターミナルが表示されます。タスクの実行中は、重複した送信がブロックされます。4 コア/4 GB RAM を下回る場合は、アップグレードを確定する前に高リスクの警告が表示されます。

アップグレードの処理では、まずアップデーターのバージョンを確認し、古いアップデーターは続行する前にアップグレードする必要があります。次に、署名付きのマニフェストと統合リポジトリのバージョンタグを検証し、設定とデータベースをバックアップし、3 つのアプリケーションコンポーネントすべてをローカルでビルドし、差分 SQL を適用し、プログラムを置き換えてヘルスチェックを行います。新しい設定項目は存在しない場合にのみ追加され、既存の値は保持され、同じディレクトリにバックアップが作成されます。失敗した場合は、定められた安全な範囲内でプログラムと設定が自動的に復元されます。アップグレード中は、UI または `sudo aid progress` で同じリアルタイムのログを確認できます。`q` を押すと、バックグラウンドのタスクを中断せずにビューアーを終了できます。

更新では 3 つのコンポーネントすべてをコンパイルし、データベースをバックアップし、ヘルスチェックを実行するため、一時的に CPU、メモリ、ディスク I/O を大量に消費する場合があります。本番環境では、まずホスト外にバックアップを作成し、トラフィックの少ない時間帯に更新を実行してください。Beta 版は、まずテスト環境で試してください。アップグレード、SQL、ロールバックの完全なルールについては、[デプロイガイド](deploy/README.md) をご覧ください。

<a id="参与贡献"></a>

## コントリビュート

中国語または英語での Issue と Pull Request を歓迎します。[コントリビューションガイド](CONTRIBUTING.md)、[公開 Provider 接続ガイド](doc/公开Provider接入指南.md)、[行動規範](CODE_OF_CONDUCT.md) を読んだうえで、問題の再現、ドキュメントの改善、バグの修正、公開モデルプロトコルへの対応など、ご自身に合った貢献の方法を選んでください。

- [問題を報告する / 改善を提案する](https://github.com/gzxx-2025/aid-studio/issues/new/choose)
- [good first issue を探す](https://github.com/gzxx-2025/aid-studio/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22good%20first%20issue%22)
- [セキュリティの問題を報告する](SECURITY.md)

AID が役に立ったら、リポジトリにスターを付けていただけると嬉しいです。公開する権利のある制作例や、デプロイの経験を共有していただくことも歓迎します。

<a id="donate"></a>

## 赞赏支持 / 寄付

如果 AID Studio 对你有帮助，欢迎自愿赞赏，支持项目持续维护与改进。

AID Studio が役に立ったら、プロジェクトの継続的なメンテナンスと改善を支えるために、任意での寄付をご検討ください。

<p align="center">
  <a href="references/wechat-donation.jpg">
    <img src="references/wechat-donation.jpg" alt="微信赞赏码 / WeChat の寄付用コード" width="320">
  </a><br>
  <sub>微信扫码赞赏 · WeChat でスキャンして寄付<br>点击图片查看原图 / 画像をクリックすると原寸で表示されます</sub>
</p>

<a id="开源协议"></a>

## ライセンス

このプロジェクトは [MIT License](LICENSE) の下でオープンソースとして公開されています。著作権は 光子讯息(杭州)科技有限公司 (Guangzi Xunxi (Hangzhou) Technology Co., Ltd.) に帰属します。第三者の帰属表示については [NOTICE](NOTICE) をご覧ください。元の著作権表示とライセンス表示は保持されています。

<a id="鸣谢"></a>

## 謝辞

管理画面のフレームワークの一部は [RuoYi-Vue](https://gitee.com/y_project/RuoYi-Vue)（MIT License）に基づいています。元のプロジェクトに深く感謝します。

| コミュニティ | 謝辞 |
|------|------|
| <a href="https://linux.do/"><img src="https://cdn3.ldstatic.com/original/4X/c/c/d/ccd8c210609d498cbeb3d5201d4c259348447562.png" alt="Linux.do" width="64"></a> | 中国語での技術的な議論とオープンソースのエコシステムを支えている [Linux.do](https://linux.do/) コミュニティに感謝します。 |
