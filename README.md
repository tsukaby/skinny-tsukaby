## Skinnyのpackage:standaloneについて

### 成功パターン

`./skinny run`してlocalhost:8080を見る。  
index.htmのHTMLちゃんと見える。
imも見える。

### 失敗パターン

standalonパッケージングする。  
javaコマンド叩く前に適当なディレクトリにcdする。Desktopとか。（cur dirが違う）
そして`java -jar [適切なパス]`

index.htmは見えるけど、imが見えない。assets/imgが解決できない模様。
