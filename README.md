# manipulator  
 FileMakerのデータをJavascriptで操作するためのアドオンです。
このアドオンはデータとそれを処理するための計算式を受け取り、その結果をFileMakerに返します。  

（ご注意）  
このアドオンはFileMakerデータをJavascriptで処理した場合の操作感を体感していただくためにつくったものであり、稼働中ファイルへの組み込みを想定したものではありません。
無限ループを発生させてしまうような計算式を指定してしまった場合や、処理データが極めて膨大なものであった場合はFileMaker側にコントロールが返ってこず、やむなく強制終了が必要になってしまう事態もありえます。実験用ファイルとして扱っていただき、大事なファイルと同時には開かないようにしてください。    

(動作要件)  
FileMaker ver19.1.2~(Mac or Win)
  
(使い方)   
Manipulatorフォルダ：　アドオン本体。ホームフォルダ下の以下の場所にこのフォルダごと配置してください。
* Library/Application Support/FileMaker/Extensions /AddonModules folder (on macOS).
* AppData\Local\FileMaker\Extensions\AddonModules (on Windows).

JS-Drill: デモファイル。manipulatorインストール済み。まずはこちらのファイルでmanipulator
の動作をご確認ください。

manipulator_howto.mp4: how-to movie
  
(Windowsにおける注意)  
WindowにおいてWebViewerのエンジンは現状IE11をベースにしたものです。その結果、以下のような制限が発生します。  
1. アロー関数、MapなどES6によって導入された新技術が使用できない。
2. d3の最新バージョンであるv6が使えない。  
JS-Drillで使用している計算式においても上記に該当する場合はSyntax Errorが返されます。　　

(D3について)  
Macにおいてはv6、Winにおいてはv5がCDN経由でロードされます。


---------------------------------------------------------------------------------------------------------



This add-on allows you to manipulate FileMaker data with Javascript.
This add-on takes the data and the formulas used to process it and returns the results to FileMaker.
  
(note)  
This add-on was created to give you a feel for Javascript processing of FileMaker data, and was not designed to be embedded in a working file.
If you specify a formula that creates an infinite loop or if the amount of data to be processed is extremely large, FileMaker will not receive control and may be forced to terminate the file. Please treat the file as an experimental file and do not open it with the important file at the same time.
  
 (Requirement)  
FileMaker version 19.1.2~(Mac or Win).
  
(How to use)  
Manipulator folder: The main body of the add-on. Please put it in the following location under the Home folder.  
* Library/Application Support/FileMaker/Extensions /AddonModules folder (on macOS).
* AppData\Local\FileMaker\Extensions\AddonModules (on Windows).
  
JS-Drill: Demo file. the manipulator is already installed. First of all, check it before you install this in your file.
  
manipulator_howto.mp4: how-to movie

  
(Note on Windows)  
The WebViewer engine in Windows is currently based on IE11. As a result, the following limitations occur  
1. new technologies introduced by ES6, such as arrow functions and Map, cannot be used.  
2. the latest version of d3 (ver6) cannot be used.  
If any of the formulas used in JS-Drill correspond to the above, a syntax error will be returned.　　

(About D3)  
On Mac, v6 is loaded via CDN and on Win, v5 is loaded via CDN.
