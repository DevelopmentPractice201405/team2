#追加課題
##sawamura
##taba

#担当者：安村、山内
herokuURL
https://enigmatic-bastion-9064.herokuapp.com/


#screenの導入 
###担当者：タバ

##インストール方法  
↓↓↓インストールのコマンドはこれです。↓↓↓  
```コマンド
$ sudo apt-get install screen
```
※ubuntuのバージョンが古い場合は、下記のようなエラーが表示されます。
```
＄ sudo apt-get install screen  
…　中略　…  
Err http://jp.archive.ubuntu.com /……  
  404  Not Found  
…  
```

サポート期間が終了したバージョンのUbuntuは  
http://old-releases.ubuntu.com  
に保存されているので、 /etc/apt/source.list　を編集する必要があります。  

source.listファイルはroot権限でないと編集できないため、次のコマンドを実行します。  
```
$ sudo su -  
```
これで source.list を編集することができます。

root権限に入ることができたら、エディタで /etc/apt/source.list 開いて

jp.archive.ubuntu.com  
を  
old-releases.ubuntu.com  
に置き換えます。

これでインストールできます。
