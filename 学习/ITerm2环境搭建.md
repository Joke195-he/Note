##  **安装部分**

1. 安装iterm2
2. 安装[brew](https://brew.sh/zh-cn/)
3. 安装[Git](https://git-scm.com/install/mac)
4. 安装[oh-my-zsh](https://www.haoyep.com/posts/zsh-config-oh-my-zsh/)
5. git设置
## **配置 Git 基本信息**

打开终端，执行如下命令
```bash
# 配置用户名
git config --global user.name "your_username"
# 配置邮箱
git config --global user.email "your_email@example.com"
```
验证配置是否成功：
```bash
git config --global --list
```
## **配置 SSH 密钥（推荐）**

为了安全地与 GitHub 通信，建议配置 SSH：
```bash
# 生成 SSH 密钥
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

# 按 Enter 使用默认位置，可设置密码或直接回车
```
**添加到 GitHub：**

1. 复制公钥内容：`cat ~/.ssh/id_rsa.pub`
2. 登录 GitHub → Settings → SSH and GPG keys
3. 点击 "New SSH key" 并粘贴公钥

**测试连接：**
```bash
ssh -T git@github.com
```