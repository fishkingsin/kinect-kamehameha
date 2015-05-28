# Working Configurations #

@en This is the list of the hardware/software configurations where this program is reported to work (or not to work). **Please use comment to let me know of your configurations.**

  * The GPU (supposedly) needs to support OpenGL 2.x & programmable shaders & GL\_ARB\_vertex\_array\_object extension. If the program ends saying "This GPU does not support shaders", install the latest graphic driver for your GPU and try again.
  * For Kinect SDK version
    * Works with Kinect SDK V1.0.
  * For OpenNI version
    * As to the best knowledge today, the recommended version combination of OpenNI, NITE, and SensorKinect is shown in the [OpenNI\_Downloads](OpenNI_Downloads.md) page. This recommendation may become obsolete, so check the OpenNI site for the up-to-date information.
    * This program does not work if you installed Microsoft's official KinectSDK. This issue generally happens for any Kinect Hacks created by OpenNI+NITE+SensorKinect. You can workaround this issue by the following steps. (Sorry this is a kind of tricky.) The behavior is not exactly the same as the original, but it "a sort of" works.
      1. Download the workaround module from the following URL and extract the archive somewhere: http://code.google.com/p/kinect-mssdk-openni-bridge/
      1. Install the module as to README. Though README explains how to modify data/OpenNIConfig.xml, it is not necessary.

@ja 動作報告(または動作しなかった報告)のあった構成です。**あなたの構成をコメントで教えてください。**

  * (おそらく)OpenGL 2.x、プログラマブルシェーダ、およびGL\_ARB\_vertex\_array\_objectをサポートしたGPUでないと動作しません。もしプログラムが "This GPU does not support shaders" と言って終了するようならグラフィックドライバを最新のものに更新して再び試してみてください。
  * Kinect SDK版について
    * Kinect SDK V1.0と問題なく動作します。
  * OpenNI版について
    * 現在知る限り、OpenNI、NITE、SensorKinectの推奨バージョンを[OpenNI\_Downloads](OpenNI_Downloads.md)ページに記述してあります。これらのバージョンは時代遅れになることもありますので、OpenNIのサイトで最新情報をチェックするようにしてください。
    * Microsoft公式KinectSDKをインストールすると動かなくなるという問題があります。これは本プログラムに限らず、OpenNI+NITE+SensorKinectを使って作られたKinect Hack一般で発生する問題です。この問題は次の手順で回避することができます(ややこしい手順ですみません)。オリジナルと完全に同じ動きにはならないものの一応動く状態にはなります。
      1. 次のURLから回避用モジュールをダウンロードし、どこかに展開する: http://code.google.com/p/kinect-mssdk-openni-bridge/
      1. READMEにしたがってインストールする。READMEにはOpenNIConfig.xmlの書き換え方が書いてありますが、これは不要です。

## Work ##

### Platform ###

| **CPU**        | **GPU**           | **OS**                | **Reported by** | **Remark** |
|:---------------|:------------------|:----------------------|:----------------|:-----------|
| Core i7 2600   | GeForce GTX 285   | Win 7 Pro 64          | tomoto          |            |
| Core i7 2600   | GeForce GTX 285   | Win XP Pro 32         | tomoto          |            |
| Core2Duo E6750 2.66GHz | GeForce 8600GT    | Win 7 Pro             | hidden.xv       |            |
| Core2Duo 2.0GHz | GeForce 9400M     | Win 7 Pro on MacBook BootCamp | hidden.xv       |            |
| AMD64x2 3200+  | GeForce 9500GT    | Win 7 Pro             | rg7strin        |            |
| Core i7 2600   | GeForce GTX 285   | Ubuntu 12.10 on VMware Player 5.0.1  | tomoto          |            |

### Kinect SDK ###

| **Kinect SDK** | **Remark** | **Reported by** |
|:---------------|:-----------|:----------------|
| 1.6            |            | tomoto          |
| 1.5            |            | tomoto          |
| 1.0            |            | tomoto          |

### OpenNI & Kinect Drivers ###

| **OpenNI** | **NITE** | **Kinect Driver** | **Remark** |  **Reported by** |
|:-----------|:---------|:------------------|:-----------|:-----------------|
| 1.5.2.23   | 1.5.2.21 | kinect-mssdk-openni-bridge 1.5.0.0 for 1.5.2.23 + Kinect SDK V1.5|            | tomoto           |
| 1.5.2.23   | 1.5.2.21 | SensorKinect by avin2 5.0.3.4 |            | tomoto           |
| 1.3.4.3    | 1.4.2.4  | SensorKinect by avin2 5.0.3.4 | ZigFu's all-in-one package | tomoto           |
| stable 1.3.3.6 | stable 1.4.2.4 | SensorKinect by avin2 5.0.3.4 |            | tomoto           |
| unstable 1.1.0.41 | unstable v1.3.1.5  | SensorKinect by avin2 5.0.1 | Obsolete   | tomoto           |
| alpha 1.0.0.23 | 1.3.0.17 | SensorKinect by avin2 5.0.0 | Obsolete   | tomoto           |
| stable 2.0.0.29 Beta | stable 2.0.0.29 Beta | Tomoto's mod      |            | tomoto           |


## Not Work ##