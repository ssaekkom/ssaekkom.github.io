---
layout: post
title:  "Linux에서 Oracle 실행 하기"
date:   2018-08-14
author: Sewon Lee
categories: Linux
tags:	Linux Oracle 
cover:  "/assets/instacode.png"
---

## Linux에서 Oracle 실행
최초 오라클 계정으로 접속한다.  
$ su - oracle  
$ sqlplus /nolog  
   SQL> conn /as sysdba  
   SQL> startup  


기본적으로 오라클이 실행된다. 그후 리스너를 실행시키자.  

$ lsnrctl start     -> 리스너 실행  
$ lsnrctl status    -> 리스너 상태  
$ lsnrctl stop      -> 리스너 정지  
