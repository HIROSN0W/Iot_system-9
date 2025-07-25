# Iot_system-9

鈴鹿高専では、構内の部屋の貸し出し情報をDX化し、Webアプリを通じて学生や教員が部屋の使用状況を確認したり、利用申請を行ったりできるようにすることを目的としています [cite: 3, 4, 9]。

このシステムは、以下の顧客と作業者を想定しています。
* **顧客**: 学生、教員
* **作業者**: 学生課、守衛

主な機能は以下の通りです。
* 各部屋の使用状況の見える化。
* 顧客がいつでもどこでも会議の予定を立てたり、部屋の利用申請を行ったりできる。
* 学生が部屋の申請をしやすくなる 。
* 守衛窓口対応が不要になり、ダブルブッキングが防止される。

集めるデータとしては、各部屋の予約状況と部屋の利用申請が挙げられます。

データの送受信方法は以下の通りです。
* 顧客はスマートフォンなどのデバイスから部屋の利用申請を行う。
* 作業者は申請の許可/却下を行う。

部屋管理アプリはWebアプリとして提供され、SNCT-STUDENTSに接続している場合のみ使用可能です（セキュリティのため）。 UIは、すべての部屋を俯瞰でき、時刻の空き状況はカレンダーアプリで表示されます。

部屋管理のフローは以下の通りです。
1.  学生が予約する。
2.  学生課が申請を受け取る。
3.  学生課が承諾する。
4.  学生課が鍵管理アプリからワンタイムパスワードを取得する。
5.  学生課が学生にパスワードを渡す。

鍵管理アプリは既存のアプリ（例: セサミスマートロック）を使用し、学生課のみが使用します。

このシステム導入による具体的な成果として、エアコンや電気の無駄遣い防止、鍵の管理のデジタル化による学生課の業務負担軽減、場所の有効活用、部屋を借りる時間の短縮が期待されています。