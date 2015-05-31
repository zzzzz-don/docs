# TomcatをMacにインストール

* インストール
```
ishii-no-MacBook-Air:~ don$ sudo mv ~/Downloads/apache-tomcat-8.0.23 /usr/local/
ishii-no-MacBook-Air:~ don$ sudo ln -s /usr/local/apache-tomcat-8.0.23 /Library/Tomcat
ishii-no-MacBook-Air:~ don$ sudo chown -R don /Library/Tomcat
ishii-no-MacBook-Air:~ don$ sudo chmod +x /Library/Tomcat/bin/*.sh
```

* tomcatを起動
```
$ /Library/Tomcat/bin/startup.sh
```

* ブラウザで確認  
http://localhost:8080/

* tomcatを停止
```
$ /Library/Tomcat/bin/shutdown.sh
```
