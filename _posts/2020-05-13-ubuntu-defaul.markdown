# 우분투(20.) 설치후 세팅순서


## 1. root 계정 활성화

```
 sudo passwd root
New password: 
Retype new password: 
passwd: password updated successfully

```


## 2. 미러변경

``` 
`sudo vi /etc/apt/sources.list`
```

확인해보면 기본적으로

http://kr.archive.ubuntu.com/


ubuntu/

위 주소로 되어있다

vi 에서 치환으로 

```
%s/kr.archive.ubuntu.com/ftp.daumkakao.com
```

변경
 

## 3. Apache 설치

```
sudo apt install -y apache2 apache2-utils
```

```
systemctl status apache2$$$
```




아파치 서비스 시작

``` 
sudo systemctl start apache2 
```

[TOC]





