=========================================================================
          Epson ePOS SDK for iOS Version 2.3.0

          Copyright Seiko Epson Corporation 2015-2016 All rights reserved.
=========================================================================

1.本ソフトウェアについて

Epson ePOS SDK for iOS は、EPSON TMプリンターおよびEPSON TMインテリジェン
トプリンターに印刷するためのiOSアプリケーションを開発する開発者向けSDKです。
Epson ePOS SDK で提供するAPIを使用してアプリケーションを開発します。Epson 
ePOS SDK には、Androidデバイス向けの Epson ePOS SDK for Android も用意され
ています。
詳細は Epson ePOS SDK for iOS ユーザーズマニュアル を参照ください。

対応iOSバージョン
  iOS 6.0 - 6.1.6
  iOS 7.0 - 7.1.2
  iOS 8.0 - 8.0.2
  iOS 8.2 - 8.4.1
  iOS 9.0 - 9.2.1

対応iOS端末
  iPhone ( 4S / 5 / 5c / 5s / 6 / 6 Plus / 6s / 6s Plus )
  iPod touch ( 第5世代 / 第6世代 )
  iPad2 / iPad ( 第3世代 / 第4世代 )
  iPad Pro ( 12.9-inch / 9.7-inch )
  iPad Air / iPad Air 2
  iPad mini / iPad mini 2 (iPad mini with Retina display) / iPad mini 3
  / iPad mini 4

サポートTMプリンター
  EPSON TM-T20（海外モデルのみ）
  EPSON TM-T20II
  EPSON TM-T60（海外モデルのみ）
  EPSON TM-T70
  EPSON TM-T70II
  EPSON TM-T81II（海外モデルのみ）
  EPSON TM-T82（海外モデルのみ）
  EPSON TM-T82II（海外モデルのみ）
  EPSON TM-T88V
  EPSON TM-T88VI（海外モデルのみ）
  EPSON TM-T90II
  EPSON TM-P20
  EPSON TM-P60（海外モデルのみ）
  EPSON TM-P60II
  EPSON TM-P80（海外モデルのみ）
  EPSON TM-U220 シリーズ（海外モデルのみ）
  EPSON TM-U330 シリーズ（海外モデルのみ）
  EPSON TM-m10
  EPSON TM-m30

サポートTMインテリジェントプリンター
  EPSON TM-T20II-i
  EPSON TM-T70-i
  EPSON TM-T82II-i（海外モデルのみ）
  EPSON TM-T83II-i（海外モデルのみ）
  EPSON TM-T88V-i
  EPSON TM-U220-i（海外モデルのみ）
  EPSON TM-T70II-DT
  EPSON TM-T88V-DT
  EPSON TM-H6000IV-DT（海外モデルのみ）

サポートネットワークプリンター
  EPSON TM-L90
  EPSON TM-T88IV
  EPSON TM-T90
  EPSON TM-T90KP

サポートインターフェイス
  TMプリンター
    有線LAN
    無線LAN
    Bluetooth
  TMインテリジェントプリンター
    有線LAN
  ネットワークプリンター
    有線LAN
    無線LAN

2.提供ファイル

・ePOS2.h
  クラス定義、エラー値／デバイスタイプの定数定義を含むヘッダーファイルです。

・ePOSEasySelect.h
  簡単にプリンターを選択するためのヘッダーファイルです。

・libepos2.a
  機能実行用ライブラリーです。（ARMv7, ARMv7s, ARM64, i386, x86_64 に対応）

・libeposeasyselect.a
  簡単にプリンターを選択するためのライブラリーです。
  （ARMv7, ARMv7s, ARM64, i386, x86_64 に対応）

・ePOS_SDK_Sample_iOS.zip
  サンプルプログラムファイルです。

・EULA.ja.txt
  SOFTWARE LICENSE AGREEMENT が記載されています。

・EULA.en.txt
  SOFTWARE LICENSE AGREEMENT（英語版）が記載されています。

・ePOS_SDK_iOS_um_ja_revx.pdf
  ユーザーズマニュアルです。

・ePOS_SDK_iOS_um_en_revx.pdf
  ユーザーズマニュアル（英語版）です。

・ePOS_SDK_iOS_Migration_Guide_ja_revx.pdf
  マイグレーションガイドです。

・ePOS_SDK_iOS_Migration_Guide_en_revx.pdf
  マイグレーションガイド（英語版）です。

・README.ja.txt
  本書です。

・README.en.txt
  本書（英語版）です。

3.その他留意点

・使用方法、使用上の注意、等の詳細は、ユーザーズマニュアルを参照し、
  ご使用ください。

・iOS9.xでTCP/IP接続を使用する場合、ネットワークのルーターに
  デフォルトゲートウェイを設定してください。

4.制限事項

・以下のTMインテリジェントプリンターでは検索機能(Discoveryクラス)
  をサポートしていません。

    TM-DT シリーズ (TM-DT ソフトウェア Ver. 3.01 以前)
    TM-i  シリーズ

5.バージョン履歴

  Version 2.3.0
    ・対応iOSバージョンからiOS9.3.xを削除
    ・サポートTMプリンターを追加
      ・TM-T60（海外モデルのみ）
    ・不具合修正
      ・TM-インテリジェントプリンターに対してdisconnect APIを実行した場合、関数が返答しないことがある現象を修正

  Version 2.2.0
    ・対応iOSバージョンを追加
      ・iOS 9.3.2
    ・対応iOS端末を追加
      ・iPad Pro ( 9.7-inch )
    ・App Storeの以下の要件に対応
      ・App Storeに申請されるすべてのアプリケーションは、IPv6のネットワークを
        サポートしている必要があります。

  Version 2.1.0
    ・サポートTMプリンターを追加
      ・TM-T88VI（海外モデルのみ）
    ・対応iOSバージョンを追加
      ・iOS 9.1 - 9.3.1
    ・対応iOS端末を追加
      ・iPad Pro ( 12.9-inch )
    ・Epos2LogクラスにSDKのバージョンを取得するためのgetSdkVersion APIを追加
    ・Bitcodeに対応
    ・Swift向けにePOS2_Printer_Swiftサンプルを追加
    ・不具合修正
      ・印刷中にOFFLINEが発生した場合、OFFLINE要因を取り除くと残りのデータが
        印刷される現象を修正
      ・TM-P20/TM-P60II/TM-m10/TM-m30/TM-T90IIで印刷中に電源OFFした場合、プリ
        ンターステータスの接続状態が"接続中"になる現象を修正
      ・disconnect API実行時に、切断イベントが発生しない現象を修正
      ・addFeedPosition APIで、正しく紙送りが行われない現象を修正

  Version 2.0.0
    ・新規リリース

