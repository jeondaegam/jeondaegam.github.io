---
emoji: ๐ฟ  
title: JPA๊ฐ ๋ญ์ผ?  
date: '2022-05-23 14:30'  
author: ์ฌ๋ฆ  
tags: jpa  
categories: ECT
---

## Persistence
๋ฐ์ดํฐ๋ฅผ ์์ฑํ ํ๋ก๊ทธ๋จ์ด ์ข๋ฃ๋๋๋ผ๋ ์ฌ๋ผ์ง์ง ์๋ ๋ฐ์ดํฐ์ ํน์ฑ  
=์์์ฑ

## jdbc์ ๊ฐ๋
๋ง์น ๋ด๊ฐ ์ด๋ฆ ๋ชจ๋ฅด๋ ๋๋ผ์ ๊ฐ์๋ ๊ธ๊ณผ ์์ ์บ๋ผ ์ ์๋ ํ๊ฒฝ์ ๋ง๋๋ ๊ฒ์ผ๋ก ๋น์ ํ  ์ ์๋ค.  
  
<img width="50%" src="https://user-images.githubusercontent.com/83997369/169747664-1f2c4f38-ef27-4e30-95b4-116266cc10ea.jpg"/>
  

## ๊ธฐ์กด์ jdbc๋?  
Connection ๊ฐ์ฒด๋ฅผ ์๋์ผ๋ก ๊ด๋ฆฌํ๋ค.  
server, username, pass ๋ฑ์ ๋ฐํ์ผ๋ก DriverManager.getConnection์ ํตํด connection์ ์ค์ ํ๋ ๊ฒ์ด ๊ทธ ์์ด๋ค.  
sql๋ฌธ์ ์์ฑํ๋ค.  
prepareStatement๋ก sql์ ์ ๋ฌํ๋ค.

## JPA์ ์ฅ์ ?
1. java application ๋ด์์ sql๋ฌธ์ ์ง์  ์์ฑํ  ๊ฒฝ์ฐ๊ฐ ์ ์ด์ง๋ค.
2. sql ๊ตฌ์กฐ๋ฅผ java application ๋ด์์ ์ ์ฉํ์ง ์์๋ ๋๋ค.

## jdbc์ jpa์ ๊ตฌ์กฐ ๋น๊ต
<img width="70%" src="https://user-images.githubusercontent.com/83997369/169747997-79371278-1056-48f7-b405-5a76ceb5649c.jpg"/>


### ์ฐธ๊ณ 
์ฐ์ํTech: [์ฌ๋ ์ JPA์ JDBC](https://youtu.be/Ppqc3qN75EE)
