---
emoji: 💡   
title: Git 계정 변경하기(Windows)  
date: '2022-08-17 17:00'  
author: 여름  
tags: git, git계정 
categories: GIT
---


### Error 
- 다른 Git 계정의 repository clone 시 repository를 찾을 수 없음.
> D:\source>git clone https://github.com/exam/exam.git  
Cloning into 'exam'...  
remote: Repository not found.  
fatal: repository 'https://github.com/exam/exam/' not found

### 해결
1. git config의 user.name, user.email 설정을 변경한다.
2. 웹 자격 증명에 저장되어 있는 github 계정 정보를 삭제한다.
```shell
> git config user.name {변경할 name}
> git config user.email {변경할 email}
```


---
### 계정 로그인 안될 땐 : Password에 git personal access token 입력하기
> remote: Support for password authentication was removed on August 13, 2021.  
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.

- token 발급위치  
git hub > Settings > Developer settings > Personal access tokens > [Generate new token](https://github.com/settings/tokens)