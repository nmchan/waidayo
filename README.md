![waidayo_logo](waidayo_logo_v3_pr.png)


# [使い方はwikiのほうが詳しいよ！](https://github.com/nmchan/waidayo/wiki)

# はじめに
- waidayoはVRMに対応した3D VTuber向けのフェイシャルモーションキャプチャシステムです。
- iPhoneで表情をキャプチャし、PCへモーションを転送することができます。
- 本アプリケーションは個人法人を問わず無償で商用利用していただくことが可能です
- わからないことや要望があれば作者のdiscord、waidayo(face2vmc) チャンネルで質問しよう！
    - https://discord.com/invite/GrZWt6U

# 必要なもの
- A12 Bionic以降のチップが搭載されたiPhone/iPad（SE2でも動くよ！！！）
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
    - 使用するVRMファイルの使用許諾についてよく確認し、自己責任でご利用ください
- iTunesを使ってiPhoneへVRMファイルを転送する
    - https://support.apple.com/ja-jp/HT201301
- Cドライブ直下（またはプログラムと同じフォルダ）へ用意したVRMファイルを置く
    - Macの場合はDocument直下のみ
- iPhone版アプリとPC版アプリを起動する
    - 自動で接続されるよ！
    
- 補足）アンチエイリアス処理の設定を変更できるよ
     - キーボード上部の数字キー(0,2,4,8)を押すと切り替わります
    
# 今後のアップデート予定
- モデルリスト（AppStore審査暫定対応のため簡易的な表示になっています）
    - 現在の実装：アプリ起動時にdefault.vrmを検出した場合は優先表示
    - アップデート予定：内蔵アバターの選択機能削除
- エモート機能
- idleポーズ変更（現在は肩下げのみ）

# リリース履歴
- 1.0.9 2020/10/05
    - iOS14環境で他の端末への自動接続機能が使用できない不具合を修正
    
- 1.0.8 2020/09/28
    - VRoid Hub経由のモデルデータが正常に読み込めない不具合を修正
    
- 1.0.6 2020/09/22
    - 対応Blendshapeの追加（口：いーの表情）

- 1.0.5 2020/07/05
    - アバターの口、舌の挙動を修正
    - 設定画面を更新（タブ追加）

- 1.0.4 2020/06/16
    - アバターの口の挙動を修正
    - 暗号化アバター（SEDSS）の転送機能

- 1.0.3 2020/06/11
    - デフォルトアバターの挙動を修正
    - デバイス探索機能を追加
- 1.0.2 2020/06/03
    - メニューボタン非表示機能
       - default.vrmを転送済みの時のみ有効化
       - 同じ場所にメニューボタンがあるので勘で押してください
    - 一部モデルで長時間利用時に腕が回転してしまう不具合を解消
    - 画面回転に対応
    - Head Offsetが正しく反映されない問題の修正
        - （設定項目を削除、後日リセットボタンを新設）
    - 一部のモデルで顔が暗くなってしまう問題を解決
    - 背景を黒にするダークモードを追加
- 1.0.1 2020/05/23
    - 認識外へ出た際の挙動を修正（アバターを完全に停止）
    - MirroringON時にBLINK_L/Rが反転しない
    - iPad版でサードパーティライセンス表示が見切れる
    - アイトラッキングオフ時の挙動修正
- 1.0.0 2020/05/20
    - 初版

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
        
# 注意事項
- waidayoではVRMの作成に利用するUniVRMはVersion0.53の利用を推奨しています
    - 0.55などでは表情や目の動きがおかしくなることがあります。 
- iPhone版とPC版で同じボーン構造、ブレンドシェイプ情報を持つモデルデータを使う必要があります
    - ＝PC側はどれだけ魔改造してもOK（HDRP対応やVRM標準外シェーダーの適用など）
- VRMファイルをインポートした場合、常に最優先で表示されます。
    - アプリ内蔵アバター、VRoid Hub連携機能でロードしたアバターは再起動時に保持されません。
- waidayoを有償頒布ソフトの機能として利用する場合は個別に相談お願いいたします。
        
# 作者について
- Twitter https://twitter.com/nmch1222
- YouTube https://www.youtube.com/c/nmch1222
- FANBOX https://nmch1222.fanbox.cc/
- 干芋 https://www.amazon.jp/hz/wishlist/ls/2YH7VGKBX5U3C?ref_=wl_share
    - waidayoの開発はみなさまの反応が原動力です
    - もしよければ作者SNSの登録やFANBOX、干芋などご支援いただけますと嬉しいです
    
