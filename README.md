![waidayo_logo](waidayo_logo.png)
# はじめに
- waidayoはVRMに対応した3D VTuber向けのフェイシャルモーションキャプチャシステムです。
- iPhoneで表情をキャプチャし、PCへモーションを転送することができます。
- 本アプリケーションは個人法人を問わず無償で商用利用していただくことが可能です
- わからないことや要望があれば作者のdiscord、waidayo(face2vmc) チャンネルで質問しよう！
    - https://discord.com/invite/GrZWt6U

# 必要なもの
- 顔認証機能のついたiPhone/iPad
- iPhoneからの情報を受信するPC（WindowsまたはMac）
- iPhoneとパソコンは同じネットワークに接続されている必要があります

# waidayoをおすすめする理由
- 無料
- VMC Protocolへの対応（表情のみを送信してVMCと合成することも可能）
- 特殊ブレンドシェイプに対応（舌、ほっぺ、眉など）
- iPhone側で表情を認識するため配信用PCの負荷軽減
- 自分自身のアバターを見ながら配信が可能

# 機能
- アバターの変更
    - iPhoneへ直接データを転送する方法とVRoid Hubからデータをダウンロードする２つの方法があります。
- 表情と顔の向きをPCへ送信する：waidayoモード
    - waidayoとwaidayo for PCだけで配信することができます。
- 表情のみをPCへ送信する：Face2VMCモード
    - バーチャルモーションキャプチャーと連携することができます。

# 使い方（手持ちのVRMファイルを利用）
- iPhone版アプリをダウンロードする
    - ![waidayo_qr](waidayo_qr.png)
    - https://apps.apple.com/jp/app/waidayo/id1513166077
    
- waidayo for PC (Windows/Mac版アプリ)をダウンロードする
    - https://nmch1222.booth.pm/items/1779185

- VRMファイルを用意して"default.vrm"とリネームしておく
- iTunesを使ってiPhoneへVRMファイルを転送する
    - https://support.apple.com/ja-jp/HT201301
- Cドライブ直下へ用意したVRMファイルを置く
    - Macの場合はDocument直下
- iPhone版アプリへPCのIPアドレスを登録する
    - 設定＞Send Motion IP Addressから変更できるよ！

# 使い方（バーチャルモーションキャプチャーと連携する）
- iPhone版waidayoの設定画面で「Face Only(With VMC)」を選択
- PC版waidayoの画面を閉じて、ばもきゃを起動（ばもきゃは先行リリース品（FANBOXで300円以上の支援）が必要）
    - https://akira.fanbox.cc/
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
    
- 舌を出す、ほっぺぷくーは別の表情のトリガーとして使うことも可能です
    - 例）BlendshapeProxyの"PUKUU"に「＞＜」や「白目」を登録する

# 注意事項
- waidayoではVRMの作成に利用するUniVRMはVersion0.53の利用を推奨しています
- iPhone版とPC版で同じボーン構造、ブレンドシェイプ情報を持つモデルデータを使う必要があります
    - ＝PC側はどれだけ魔改造しても良い（HDRP対応やVRM標準外シェーダーの適用など）
- VRMファイルをインポートした場合、常に最優先で表示されます。
    - アプリ内蔵アバター、VRoid Hub連携機能でロードしたアバターは再起動時に保持されません。

# おすすめのスマホ固定具
- waidayoモード
    - 同時に充電できるようにスリットが開いているスタンドがおすすめです
    - https://www.amazon.co.jp/dp/B07YZ9F1WV/ref=cm_sw_r_tw_dp_U_x_.ujXEb7EH5BG9

- Face2VMCモード
    - ネックホルダー型のものがおすすめです
    - https://www.amazon.co.jp/dp/B07MLQ7XSR/ref=cm_sw_r_tw_dp_U_x_7ItWEbXKR67ZR
    
# 今後のアップデート予定
- モデルリスト（AppStore審査暫定対応のため簡易的な表示になっています）
    - 現在の実装：アプリ起動時にdefault.vrmを検出した場合は優先表示
    - アップデート予定：複数のVRMに対応
- エモート機能
- idleポーズ変更（現在は肩下げのみ）
- 【修正済み　次回リリース】認識外へ出た際の挙動
- 【修正済み　次回リリース】MirroringON時にBLINK_L/Rが反転しない
- 【修正済み　次回リリース】iPad版でサードパーティライセンス表示が見切れる
- 【修正済み　次回リリース】アイトラッキングオフ時の挙動修正
- Head Offsetが正しく反映されない問題の修正（設定項目を削除、後日リセットボタンを新設）
- 基準点リセットボタンを追加

# トラブルシューティング
- 目がプルプルする等うまく動かない、停止しない
    - Eye TrackingはON、Eye Traking Offset を0にする
    - https://twitter.com/nmch1222/status/1262977166657990659
- 髪の毛が緑色なんだけどwaidayo for PCの背景色を変えられるようにしてほしい
    - EVMC4Uで独自の配信環境を作成することができます
    - https://twitter.com/Seg_Faul/status/1263002762410770433

# 謝辞
- iPhone版アプリに標準搭載のアバターはこよりちゃん制作のフィリナちゃんを使用させて頂いています（使用許諾済み）
    - 気に入ったら買ってね https://nagatorokoyori.booth.pm/items/1577042
    - こよりちゃん https://twitter.com/Nagatoro_Koyori
- iPhone版アプリに標準搭載の切替用アバターはVRoidサンプルモデルのViviちゃんを使用させて頂いています（CC0）
    - Vivi紹介ページ https://vroid.pixiv.help/hc/ja/articles/360014900273-%E3%83%93%E3%83%93-Vivi
- iPhone版アプリのリリースにあたり協力いただいた方々
    - あきらさん https://twitter.com/sh_akira
        - ばもきゃ側のFace2VMCモード対応、アプリリリース作業
    - せぐふぉさん https://twitter.com/Seg_Faul
        - 通信処理の大半
        
# 作者について
- Twitter https://twitter.com/nmch1222
- YouTube https://www.youtube.com/c/nmch1222
- FANBOX https://nmch1222.fanbox.cc/
    
