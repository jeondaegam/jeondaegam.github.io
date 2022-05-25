---
emoji: 💿  
title: JPA가 뭐야?  
date: '2022-05-23 14:30'  
author: 여름  
tags: jpa  
categories: ECT
---

## Persistence
데이터를 생성한 프로그램이 종료되더라도 사라지지 않는 데이터의 특성  
=영속성

## jdbc의 개념
마치 내가 이름 모르는 나라에 가서도 금과 은을 캐낼 수 있는 환경을 만드는 것으로 비유할 수 있다.  
  
<img width="50%" src="https://user-images.githubusercontent.com/83997369/169747664-1f2c4f38-ef27-4e30-95b4-116266cc10ea.jpg"/>
  

## 기존의 jdbc는?  
Connection 객체를 수동으로 관리한다.  
server, username, pass 등을 바탕으로 DriverManager.getConnection을 통해 connection을 설정하는 것이 그 예이다.  
sql문을 작성한다.  
prepareStatement로 sql을 전달한다.

## JPA의 장점?
1. java application 내에서 sql문을 직접 작성할 경우가 적어진다.
2. sql 구조를 java application 내에서 적용하지 않아도 된다.

## jdbc와 jpa의 구조 비교
<img width="70%" src="https://user-images.githubusercontent.com/83997369/169747997-79371278-1056-48f7-b405-5a76ceb5649c.jpg"/>


### 참고
우아한Tech: [올레의 JPA와 JDBC](https://youtu.be/Ppqc3qN75EE)
