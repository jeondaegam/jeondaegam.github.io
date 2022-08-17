---
emoji: 💡   
title: Git 필수 명령어  
date: '2022-07-01 17:00'  
author: 여름  
tags: git, git명령어  
categories: GIT
---


### Error 
- 기존 프로젝트를 git에 추가하기위해 remote url을 설정하는 과정
> fatal: unable to access 'https://github.com/jeondaegam/{project_name}.git/': Could not resolve host: github.com

### 해결
- remote url을 www를 포함하여 재설정한다.
```shell
> git remote remove origin
> git remote -v
> git remote add origin https://www.github.com/jeondaegam/{project_name}.git
> git push -u origin main
```
