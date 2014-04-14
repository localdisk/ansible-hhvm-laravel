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
[Ansible のインストール](http://docs.ansible.com/intro_installation.html) を参考にしてください。
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
