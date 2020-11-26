---
layout: post
title:  "Hp스위치 콘솔접속"
categories: net
tags: hp,l2,web,hpe,switch
author: hopeone
description: 기본설정 
comments: true
---

###### . 로컬 사용자 계정 생성 및 서비스 타입 및 레벨 설정 (telnet)
```



<5500-EI>
%Apr  2 09:08:26:096 2000 5500-EI SHELL/5/LOGIN:- 1 - Console(aux0) in unit1 login
<5500-EI>
<5500-EI>sys	
<5500-EI>system-view  
System View: return to User View with Ctrl+Z.
[5500-EI]local-user admin
New local user added.

[5500-EI-luser-admin]password simple 패스워드!@#
 The system password control is set to enable.  Please change your password to minimum length of 10 characters.


[5500-EI-luser-admin]service-type terminal level 3


[5500-EI-luser-admin]quit          

[5500-EI]user-interface vty 0 4
[5500-EI-ui-vty0-4]aut	
[5500-EI-ui-vty0-4]authentication-mode sch	
[5500-EI-ui-vty0-4]authentication-mode scheme 
[5500-EI-ui-vty0-4]quit





	
[5500-EI-ui-aux0]authentication-mode scheme 
[5500-EI-ui-aux0]quit
[5500-EI]quit
<5500-EI>quit





Username:admin
Password:
The system password control is set to enable.  Please change your password to minimum length of 10 characters.
Password:****
Confirm:****
 The system password control is set to enable.  Please change your password to minimum length of 10 characters.
Password:*********
Confirm:*********
 The system password control is set to enable.  Please change your password to minimum length of 10 characters.
Password:***********
Confirm:***********
Updating user password, please wait..........
<5500-EI>
%Apr  2 09:15:21:492 2000 5500-EI SHELL/5/LOGIN:- 1 - admin(aux0) in unit1 login
<5500-EI>
<5500-EI>sy	
<5500-EI>system-view 






Username:admin
Password:
<5500-EI>
%Apr  2 09:15:34:534 2000 5500-EI SHELL/5/LOGIN:- 1 - admin(aux0) in unit1 login
<5500-EI>sys	
<5500-EI>system-view 
System View: return to User View with Ctrl+Z.
[5500-EI]
```

