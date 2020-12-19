
Window Powershell (x86)ではなく64版を使う

Permission denied

PS C:\Users\Redpeaks>  ssh -i C:\MySshkey\MyLinux_key.pem azureuse@52.165.146.44
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
Permissions for 'C:\\MySshkey\\MyLinux_key.pem' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.
Load key "C:\\MySshkey\\MyLinux_key.pem": bad permissions
azureuse@52.165.146.44: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).

MyLinux_key.pemの権限を設定
Administrator以外削除


C:\Users\Redpeaks\.ssh
MyLinux_key.pem
を置く

https://azureworkshops.github.io/Docker-on-CentOS/Courseware/Install_Docker.html

sudo yum update -y
yumというパッケージ管理ツールでの最新状態に設定する。

Dockerをインストールする
sudo yum install -y yum-utils device-mapper-persistent-data lvm2
sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
