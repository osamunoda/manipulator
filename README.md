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
