jig.jp サマーインターンシップ2024 選考課題
函館高専
ケビン　ウオング


１．実装した機能やデザインの説明
実装した機能としてはまず正常のしりとりゲームとして最後の文字と入力した言葉の最初の文字をチェックする機能を作りました。
また、リセットボタンでゲームをはじめからやり直す機能を作りました。
最後に前に使った言葉のリストを表示できる機能もを追加しました。これで前に出てきた言葉を使ったらゲームが終了となります。


２．アプリの動作確認の方法（WebサイトのURLや、セットアップを含めたアプリケーションの実行手順等）
まずはヒント通りpreviousWordをwordHistoriesのArray of Stringsに書き替え、使ったことばをarrayに追加します。
入力したことばの exception　をチェックします：
    １．最後の文字が「ん」であった場合は alert　を表示してゲームが終了となります
    ２．入力した言葉がarrayにあるかどうかを確認し、あった場合は alert　を表示してゲームが終了となります
    ３．最後の言葉の最後の文字と入力した言葉の最初の文字に合わせ、一致である場合はその言葉をarrayに入れ、ゲームを続けます。

exception 1また２に捕まったら自動的に　http://localhost:8000/end.html　のページにredirectします。ここでは、end.htmlを表示ます。
リセットのボタンを押したらまた　http://localhost:8000/index.html　のメインページに戻ります。



３．参考にしたWebサイト
https://developer.mozilla.org/en-US/
https://www.w3schools.com/js/
https://zenn.dev/kawaxumax/articles/0044a0e30536e2
https://dmitripavlutin.com/javascript-fetch-async-await/
https://note.com/jigjp_engineer