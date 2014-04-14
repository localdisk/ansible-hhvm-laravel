## ansible-hhvm-laravel


Vagrant + Ansible for PHP Server.

HHVM のお勉強のために作りました。[Laravel](http://laravel.com) を入れているのは趣味です。

## 内容

- Ubuntu 12.04 64bit
- Nginx
- HHVM
- Composer
- Redis
- MySQL
- and Laravel

## インストール

### 1. [VirtualBox](https://www.virtualbox.org/) をインストール
最新版を入れれば大丈夫。
### 2. [Vagrant](http://www.vagrantup.com/) をインストール
最新版を入れれば大丈夫。
### 3. [Ansible](http://www.ansible.com/home) をインストール
[足りないインフラ力をAnsibleでまかなう](http://localdisk.hatenablog.com/entry/2014/01/19/%E8%B6%B3%E3%82%8A%E3%81%AA%E3%81%84%E3%82%A4%E3%83%B3%E3%83%95%E3%83%A9%E5%8A%9B%E3%82%92Ansible%E3%81%A7%E3%81%BE%E3%81%8B%E3%81%AA%E3%81%86(%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB)に書きました。
Windows ユーザーは諦めましょう。
### 4. git clone
```
$ git clone https://github.com/localdisk/ansible-hhvm-laravel.git
```
### 5. vagrant up
```
$ cd ansible-hhvm-laravel
$ vagrant up
```
### 6. 確認
http://192.168.33.10/ にアクセスすると Laravel の初期画面が表示されます。
現在 Permission まわりに不具合があります。エラーが発生したら
```
$ chmod -R 777 laravel/app/storage
```
してください。

おかしいところがあったら Pull Request お願いします。
