![waidayo_logo](waidayo_logo.png)
# はじめに
- 顔認証機能のついたiPhone/iPadが必要です
- iPhoneとパソコンは同じネットワークに接続されている必要があります
- わからなかったらdiscordの waidayo(face2vmc) チャンネルで質問しよう！
https://discord.com/invite/GrZWt6U

# 使い方
- iPhone版アプリをダウンロードする
    - Apple App Storeからダウンロードしてね
    - リンク
    
- Windows/Mac版アプリをダウンロードする
    - https://nmch1222.booth.pm/items/1779185

- VRMファイルを用意して"default.vrm"とリネームしておく
- iTunesを使ってiPhoneへVRMファイルを転送する
    - https://support.apple.com/ja-jp/HT201301
- PCのCドライブ直下へ用意したVRMファイルを置く
    - Macの場合はDocument直下
- iPhone版アプリへPCのIPアドレスを登録する
    - 設定＞OSC Sending IP Addressから変更できるよ！

# バーチャルモーションキャプチャーに表情データのみを送る（Face2VMCモード）
- iPhone版waidayoの設定画面で「Face Only(With VMC)」を選択
- PC版waidayoの画面を閉じて、ばもきゃを起動（ばもきゃは先行リリース品（支援）の必要あり）
- ファイヤーウォールの通信確認画面が出た場合は「許可」を押下
- ばもきゃのコントロールパネルにて「詳細設定」を押し詳細設定画面を開く
- 設定画面が出たら「外部からのモーション受信を有効にする」にチェックを入れて「適用」ボタンを押す。
    - （Port番号はデフォルトで入っている「39540」でOK）


# フェイシャルキャプチャ対象となるBlendshapeProxyを増やす
- waidayoではVRM規格で定義されているBlendshapeに加えて以下が利用可能です
    - EYEBROW_ANGRY　おこり眉（Syncモード）
    - EYEBROW_ANGRY_L　おこり眉L（Separateモード）
    - EYEBROW_ANGRY_R　おこり眉R（Separateモード）
    - EYEBROW_SORROW　しょんぼり眉（Syncモード）
    - EYEBROW_SORROW_L　しょんぼり眉L（Separateモード）
    - EYEBROW_SORROW_R　しょんぼり眉R（Separateモード）
    - TONGUE_OUT　舌を出す
    - PUKUU　ほっぺぷくー

# 注意事項
- waidayoではVRMの作成に利用するUniVRMはVersion0.53の利用を推奨しています

# 補足
- 本アプリケーションは法人個人を問わず商用利用していただくことが可能です
