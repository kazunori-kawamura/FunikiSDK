# FUN'IKI SDK
By using the FUN'IKI Ambient Glasses SDK (Software Development Kit), it is possible to link the app you developed with the <FUN'IKI Ambient Glasses> and control how the glasses glow and play sounds. In addition, software development that utilizes data from the various sensors is possible.  

The SDK is free of charge and developed apps can be published freely, so try making a fun, original app.  

In addition, although functionality is limited compared to the SDK, it is possible to simply control the <FUN'IKI Ambient Glasses> using MIDI and OSC.  

# 雰囲気メガネSDK
雰囲気メガネSDK（ソフトウェア開発キット）を用いれば、ご自分で開発したアプリと〈雰囲気メガネ〉を連携させて、思いのままにメガネを光らせ、音を鳴らすことができます。また、各種センサーのデータを活用したソフトウェアの開発も可能です。SDKは無償であり、開発したアプリは自由に公開できます。ぜひ独創的で楽しいアプリを作ってください。なお、SDKより機能が限られますが、MIDIやOSCを用いて簡単に〈雰囲気メガネ〉をコントロールすることもできます。


#開発環境
Xcode 7.2以上

##インストール
### Cocoapods
雰囲気メガネSDKはCocoapodsに対応しています。[CocoaPods](http://cocoapods.org).
Podfileに以下の記述を追加して下さい。
```
pod 'Funiki', :git => 'https://github.com/FUNIKImegane/FunikiSDK.git'
```

#雰囲気メガネSDK 1.0.1で使用できる機能
-LED、ブザー  
   LEDの色と、その色に変わる遷移時間を指定して、光りをコントロールすることができます。  
   同時にブザーの音の高さ、音の強さ、持続時間を指定して鳴らすことができます。  
   
-加速度、角速度センサ  
   加速度と角速度の情報を取得できます。取得できる間隔は接続状況によって変化します。  
   
-プッシュ・ボタン  
   プッシュ・ボタンで発生したイベント（シングル・プッシュ、ダブル・プッシュ）を取得できます。  
   
-バッテリー残量  
   バッテリー残量を3段階で取得できます。  
   

#既知の不具合
・UVセンサ、照度センサは問題が確認されたため、このバージョンのSDKでは公開を見送らせていただきます。


SDKで利用出来るクラス、メソッドなどは、MAFunikiManager.h のコメントを参照してください。

#ファイルの構成
- FunikiSDK
SDK(FunikiSDK.a)とヘッダ・ファイル、簡単にLEDを制御するプログラム(Funiki.h, Funiki.m)
- FunikiSDKExample
SDKの内容を網羅したサンプル・コード(Objective-C)
- FunikiSDKExampleSwift
SDKの内容を網羅したサンプル・コード(Swift)
- FunikiSDKEasyExample
簡単にLEDを制御するサンプル・コード(Objective-C)
- FunikiSDKEasyExampleSwift
簡単にLEDを制御するサンプル・コード(Swift)
- Documents
SDKの使用方法

雰囲気メガネSDKを既存のプロジェクトで使用するには、Documents/ 内のHTMLファイルを参照してください。   



