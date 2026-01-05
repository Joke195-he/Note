##  **安装部分**

1. 安装iterm2
2. 安装[brew](https://brew.sh/zh-cn/)
3. 安装[Git](https://git-scm.com/install/mac)
4. 安装[oh-my-zsh](https://www.haoyep.com/posts/zsh-config-oh-my-zsh/)
5. git设置
## **配置 Git 基本信息**

打开终端，执行如下命令
```shell
# 配置用户名
git config --global user.name "your_username"
# 配置邮箱
git config --global user.email "your_email@example.com"
```
验证配置是否成功：
```shell
git config --global --list
```
## **配置 SSH 密钥（推荐）**

为了安全地与 GitHub 通信，建议配置 SSH：