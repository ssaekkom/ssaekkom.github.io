---
layout: post
title:  "Oracle에서 table, column 목록 조회"
date:   2018-08-21
author: Sewon Lee
categories: Oracle
tags:	Oracle table column
cover:  "/assets/instacode.png"
---

## 1. 테이블 목록조회  
SELECT *  
FROM ALL_ALL_TABLES;  

SELECT *  
FROM DBA_TABLES;  

SELECT *  
FROM ALL_OBJECTS  
WHERE OBJECT_TYPE = 'TABLE';    


-- 접속한 계정의 테이블 목록보기    
SELECT *  
FROM TABS;  

SELECT *  
FROM USER_OBJECTS   
WHERE OBJECT_TYPE = 'TABLE';  

SELECT *  
FROM USER_TABLES;  


-- 테이블 코멘트 보기  
SELECT *  
FROM ALL_TAB_COMMENTS  
WHERE TABLE_NAME = '테이블명';  

SELECT *  
FROM USER_TAB_COMMENTS;  


## 2. 컬럼 목록조회  
SELECT *  
FROM COLS  
WHERE TABLE_NAME = '테이블명'  
;  

SELECT *  
FROM ALL_TAB_COLUMNS  
WHERE TABLE_NAME = '테이블명';  

SELECT *  
FROM USER_TAB_COLUMNS;  

-- 컬럼 코멘트 보기  
SELECT *  
FROM USER_COL_COMMENTS;  


## 3. 인덱스 목록조회  
ALL_INDEXES      
ALL_IND_COLUMNS  
ALL_CONSTRAINTS  
DBA_INDEXES  
USER_INDEXES  
....   

