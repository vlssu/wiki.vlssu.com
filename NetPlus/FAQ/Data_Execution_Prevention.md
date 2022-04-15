---
title: 关闭数据执行保护
description: 
published: true
date: 2022-01-19T15:54:25.140Z
tags: 
editor: markdown
dateCreated: 2022-01-19T10:01:01.117Z
---

# 正常关闭数据执行保护
## 右击计算机，选择属性
![dep1.png](/img/netplus/dep1.png)
## 选择高级系统设置
![dep2.png](/img/netplus/dep2.png)
## 点击高级，选择设置
![dep3.png](/img/netplus/dep3.png)
## 选择数据执行保护，然后在下面仅为基本windows程序和服务启用DEP前面点亮，然后点击确定
![dep4.png](/img/netplus/dep4.png)

# 数据执行保护呈灰色时关闭
> 默认的管理员账号是关闭开不了的
> 需要创建一个新的管理员账户才能关闭
{.is-warning}

## 创建一个新管理员账户
### 进入控制面板
![dep5.png](/img/netplus/dep5.png)
### 在大图标下进入用户账户
![dep6.png](/img/netplus/dep6.png)
### 在电脑设置中添加新用户
![dep7.png](/img/netplus/dep7.png)
### 管理其他账户
![dep8.png](/img/netplus/dep8.png)
### 添加账户
![dep9.png](/img/netplus/dep9.png)
### 输入你要创建的这个账户的一些信息
![dep10.png](/img/netplus/dep10.png)
> 记得要管理员权限
{.is-warning}

## 登陆新创的账户
> 只要注销在登录的时候切换成新账户就行了（由于我的电脑不需要，所以没截图了）
{.is-info}

## 输入指令
### 在开始页输入cmd并以管理员身份运行
![dep11.png](/img/netplus/dep11.png)
### 输入 `bcdedit /set nx optin alwaysoff` 并回车运行后重启
![dep12.png](/img/netplus/dep12.png)

## 再切换回你之前的账户
> 你就看到你成功啦，你会发现，DEP也被开启了
{.is-success}
