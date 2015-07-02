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

# 余談

## 便利なコマンド
```
ishii-no-MacBook-Air:Library don$ /usr/libexec/java_home -V
Matching Java Virtual Machines (3):
    1.8.0_45, x86_64:	"Java SE 8"	/Library/Java/JavaVirtualMachines/jdk1.8.0_45.jdk/Contents/Home
    1.6.0_65-b14-466.1, x86_64:	"Java SE 6"	/System/Library/Java/JavaVirtualMachines/1.6.0.jdk/Contents/Home
    1.6.0_65-b14-466.1, i386:	"Java SE 6"	/System/Library/Java/JavaVirtualMachines/1.6.0.jdk/Contents/Home

/Library/Java/JavaVirtualMachines/jdk1.8.0_45.jdk/Contents/Home
```
