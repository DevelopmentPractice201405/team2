#追加課題
###sawamura
####演習問題ブランチ名
* 5章:5-6-1, 5-6-2, 5-6-3
* 7章:7-6-1,

#TMUX導入
tmuxインストール
```コマンド
$ sudo apt-get install tmux
```
※ubuntuのバージョンが古い場合は、下記のようなエラーが表示されます。
```
＄ sudo apt-get install tmux  
…　中略　…  
Err http://jp.archive.ubuntu.com /……  
  404  Not Found  
…  
```
サポートが終了したため、パッケージファイルの置き場所のサイトが
old-releases.ubuntu.com に変わったせいです。
/etc/apt/sources.list の中の URL を old-releases.ubuntu.com に変更します。

次のコマンドで、一括でインストール元を変更できます。
（実行前に /etc/apt/sources.list をどこかにコピーして変更前の内容を退避しておくと良いでしょう）
```
$ sudo sed -i -e 's|//.*ubuntu.com/|//old-releases.ubuntu.com/|' /etc/apt/sources.list
```
以下のコマンドを実行して、エラーが出なければOK です。
```
$ sudo apt-get update
```


tmuxインストール
```コマンド
$ sudo apt-get install tmux
```


tmux起動
```
$ tmux
```
画面の最下行に緑色の線が表示されます。
