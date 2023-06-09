---
coverY: 0
---

# 服务器其他问题

### 一、为什么进不去服务器

#### 1. 常见问题

请确认以下几点，以确保你可以顺利连接服务器：

* 我们的服务器版本为JAVA版，支持1.12.x到1.20.1的版本，确保你的客户端版本与服务器版本匹配。
* 检查你的ID，它应仅包含大小写英文字母、数字和下划线(\_)，不应包含汉字或其他特殊字符。
* 我们的服务器不支持皮肤站登录，如果你试图使用皮肤站登录，你可能会看到"无效的个人信息公钥签名"的错误信息。我们的服务器仅支持离线和正版登录。
* 我们的服务器具有安全策略，如果你第一次尝试连接时失败，可能是因为服务器正在分析你的连接。请尝试多次连接。

#### 2. Java问题

不同版本的Minecraft需要使用不同版本的Java：

* Minecraft的1.17及以上版本需要使用Java 17。
* Minecraft的1.16及以下版本需要使用Java 8或11。

`java.lang.NoSuchMethodError: sun.security.util.ManifestEntryVerifier.<init>(Ljava/util/jar/Manifest;)V`

如果你遇到这样的错误，这可能是你需要降级你的Java版本：

* 对于Java 8用户，你需要降级到8u320版本或更早的版本。
* 对于Java 11用户，你需要降级到11.0.13版本或更早的版本。

### OpenJDK

OpenJDK是开源的Java开发工具包，由全球Java社区维护和开发。

* 全部版本：[OpenJDK](https://adoptium.net/temurin/releases/)
* 清华大学镜像站：[OpenJDK - 清华大学镜像站](https://mirrors.tuna.tsinghua.edu.cn/Adoptium/)

### Oracle JDK

Oracle JDK是Oracle公司的Java开发工具包，与OpenJDK基本相同，但包含一些商业特性。

* 全部版本：[Oracle JDK](https://www.oracle.com/java/technologies/downloads/archive/)

### DragonWell JDK

DragonWell JDK是阿里巴巴维护的OpenJDK的分支，对性能进行了优化。

* Java 17：[DragonWell 17](https://github.com/alibaba/dragonwell17/releases/latest)
* Java 11：[DragonWell 11](https://github.com/alibaba/dragonwell11/releases/latest)
* Java 8：[DragonWell 8](https://github.com/alibaba/dragonwell8/releases/latest)

#### 3.检查服务器地址是否正确

* 服务器IP：`mcfun.us`
* 核心版本：`1.20.1`
* 兼容版本：`1.12.x-1.20.1`
* 正版验证：否

### 二、游戏的下载途径

**对于电脑用户：**

1. 下载并安装jdk17（提供运行环境）以及HMCL启动器或PCL2启动器。
2. 从群文件中下载整合包。

**对于基岩版用户：**

请直接访问Minecraft官方网站进行下载。

**对于手机用户：**

可以尝试使用Java版启动器进行安装（注意：此方法可能稍显复杂，如果遇到困难，建议自行寻找解决方案）。

* iOS用户需要自己搜索并利用外网ID进行下载。

**相关资源链接：**

* [HMCL启动器下载](https://hmcl.huangyuhui.net/download)
* [Java环境下载](http://www.java.com)
* [MC百科](https://www.mcmod.cn)

### 三、账户注册及密码管理

**注册与登录：**

* 请注意，您设置的密码是用于登录游戏，而非服务器密码，请确保记住。
* 注册账号，请使用以下指令（注意：不要输入方括号）：
  * `/register [您的密码] [重复您的密码]`
  * 或
  * `/reg [您的密码] [重复您的密码]`
* 登录时，请使用以下指令：
  * `/login [您的密码]`
  * 或
  * `/l [您的密码]`

**邮箱绑定与更改密码：**

* 确保您已经有一个有效的邮箱。登录后，在聊天框中输入：
  * `/email add [要绑定的邮箱地址] [再次输入要绑定的邮箱地址]`
  * 注意：一个账号只能绑定一个邮箱。
* 如果您忘记了密码并想要通过邮箱更改，确保您的账户已绑定邮箱。在未登录前，在聊天框中输入：
  * `/email recover`
  * 系统会向您的绑定邮箱发送一封含有新密码和重置指令的邮件。在收到邮件后，在聊天框中输入：
  * `/email setpassword [新密码]`
  * 然后用新密码登录。
* 如果您未绑定邮箱且忘记了密码，请联系管理员进行密码重置。

**更换绑定邮箱：**

* 登录后，在聊天框中输入：
  * `/email change [旧的邮箱地址] [新的邮箱地址]`

### 四、封禁政策与纠纷解决

**封禁政策：**

游戏中的不良行为可能会导致您的账号被封禁，主要有以下几种情况：

* 刷取物品
* 使用作弊工具
* 在游戏中发表敏感言论或引发争吵。通常会先禁言一段时间。

如若被封禁，您可以联系服务器管理员（admin@mcfun.us）进行申诉，并需要提供一份50-100字的诚意保证书。

**纠纷解决：**

游戏过程中可能出现矛盾和冲突，如果出现争吵，建议冷静后主动与对方沟通解决，或寻求服务器管理员/OP的帮助。

请注意，如果持有强硬态度并且是自己方存在错误，将会根据事件的严重程度进行封禁、禁言或关入监狱等处罚。
