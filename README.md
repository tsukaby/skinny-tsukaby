## Skinnyのpackage:standaloneについて

### 成功パターン1

`./skinny run`してlocalhost:8080を見る。  
HTMLちゃんと見える。

### 成功パターン2

`./skinny package:standalone`して`java -jar standalone-build/target/scala-2.11/skinny-blank-app-standalone-assembly-0.1.0-SNAPSHOT.jar`する。  
HTMLちゃんと見える。

### 失敗パターン

途中までは成功パターン2と同じ。  
javaコマンド叩く前に適当なディレクトリにcdする。Desktopとか。（さっきとcur dirが違う）
そして`java -jar [適切なパス]`

404

current dirのsrc/main/webapp以下にファイルがある前提の動きになってしまっている・・・？(jarを解凍しても良くわからない状況でした・・・タスケテ）

