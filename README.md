generated from [slime-hatena/launch-umamusume-from-steam](https://github.com/slime-hatena/launch-umamusume-from-steam)

# launchOnSteam
非Steamゲーを無理やりSteamで起動して「プレイ中」を維持するスクリプト。  
自分用ですが使えそうなら持っていってください。

> [!TIP]
> 使用する場合はコピペ、もしくはzipでダウンロードしてください！。
> どうしてもgitを使用する場合はチェックアウト先をコミット単位にして、バージョンを固定してください。
> 私がスクリプトを気ままに更新する可能性があるので、追従すると急に動かなくなります。

## 免責事項

このスクリプトを実行時に起きた損害等には責任を負いかねます。  
また使用した結果、ゲーム内でBANされる可能性も否定できません。自己責任でご利用ください。

**以下は以前のスクリプトの説明のままです、そのうち書き換えます**

## 使い方

### 1. Steamに非Steamゲームを登録する

Steamクライアントの左下から追加します。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/7b55c12d-1e98-fb14-f47c-222b532732c1.png)

開いた画面のなかから1つチェックを入れて追加します。  
すべての設定を変更するため、何を選んでも大丈夫です。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/5ce395a6-df58-f116-998e-1d4991697a75.png)

### 2. ゲームの設定を編集する

追加したゲームを右クリックし、プロパティを開きます。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/94493773-aa9b-3240-d07b-e4e713261f32.png)

以下のように設定してください。  
なお、こちらの[Setting generator](https://slime-hatena.github.io/launch-umamusume-from-steam/)を使用することで簡単に設定を生成できます。

|   |   |
|---|---|
| タイトル | `ウマ娘 プリティーダービー` |
| リンク先（画像ではTARGET） | `"C:\WINDOWS\System32\WindowsPowerShell\v1.0\powershell.exe"` |
| 作業フォルダー（画像ではSTART IN） | `"<<あなたがウマ娘をインストールしたディレクトリ>>"` |
| 起動オプション | `-windowstyle hidden -NoProfile -ExecutionPolicy Bypass -Command "& \"<<あなたがダウンロードしたスクリプトを配置したディレクトリ>>\bin\start.ps1\""` |

`<<---->>` はあなたの環境情報で置き換えてください。すべて絶対パスで指定する必要があります。  
コピペや置き換え時に、文字を消しすぎてしまわないよう気をつけてください。  
アイコンなどは適当に拾ってきて設定します。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/3baa8277-bc8e-8e59-9aa5-b31223cbaec5.png)

### 完成

ゲームを起動するとDMMGAMESランチャーとウマ娘が起動するはずです。

### 3. 見た目を良くする（任意）

このままだと見た目が悪いので変更します。
必要な画像は3種です。

- 背景（画像1枚目）
- ロゴ（画像1枚目）
- カバー（画像2枚目）


![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/78e9a9bb-5ea1-28aa-9205-008470f0860e.png)

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/88b70d7f-b245-246e-881b-bba385795960.png)

背景部分で右クリックをするとカスタム背景やロゴが指定できます。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/d3f88cba-e172-b44a-a61b-eb1e5aab8934.png)


同様にライブラリのコレクションカバーも右クリックで指定できます。

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/e574ba65-ee71-f889-48e3-2210aa0f37d9.png)

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/00d1da41-bb5b-e1e8-5ae2-cfc621a4bd37.png)


見た目が良くなるのでぜひ設定しておきましょう！

![image](https://github.com/slime-hatena/launch-umamusume-from-steam/blob/images/1973eb80-fac4-d4bd-b2c6-e40480356980.png)
