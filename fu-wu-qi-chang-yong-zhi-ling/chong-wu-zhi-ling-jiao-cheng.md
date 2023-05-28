# 宠物指令教程

## 聊天命令

* `<option>` -> 必选!
* `[option]` -> 可选 大多数命令都有别名，如 /pi。使用它们代替长版本。

您还可以通过 **`[TAB]`** **键使用自动完成功能来浏览命令选项**。

### 我的宠物命令 <a href="#mypet-commands" id="mypet-commands"></a>

#### `/mypet` <a href="#mypet" id="mypet"></a>

* 显示所有可用的 _MyPet_ 命令。

#### `/petinfo` <a href="#petinfo" id="petinfo"></a>

* 语法： `/petinfo [宠物名]`
* 显示有关您或其他玩家的宠物的以下信息。
  * hit-points 生命值
  * hunger 饥饿
  * food items 食品
  * behavior 行为
  * experience 经验
  * level 等级
  * owner 主人（仅当宠物不属于您时）
  * skilltree 技能树
* 别名：
  * `/pinfo`

#### `/petname` <a href="#petname" id="petname"></a>

* 语法：
  * `/petname <new-pet-name>`
* 设置宠物的名称。
* 主人可以使用颜色使宠物的名字更加丰富多彩，通过这个占位符：
  * `<black>`, `<darkaqua>`, `<darkblue>`, `<darkgreen>`, `<darkred>`, `<darkpurple>`, `<gold>`, `<gray>`, `<darkgray>`, `<blue>`, `<green>`, `<aqua>`, `<red>`, `<lightpurple>`, `<yellow>`, `<white>`, `<magic>`, `<bold>`, `<strikethrough>`, `<underline>`, `<italic>`, `<reset>`

#### `/petrelease` <a href="#petrelease" id="petrelease"></a>

* 语法： `/petrelease [宠物名称]`
* 释放您的宠物，这样您就不再拥有宠物了

#### `/petcall` <a href="#petcall" id="petcall"></a>

* 将您的宠物传送给您。
* 别名：
  * `/pc`
  * `/petc`

#### `/petsendaway` <a href="#petsendaway" id="petsendaway"></a>

* 送走你的宠物。
* 仍然可以使用 `/petcall` 命令调用它
* 别名：
  * `/psa`
  * `/petsa`

#### `/petrespawn` <a href="#petrespawn" id="petrespawn"></a>

* 语法： `/petrespawn [`**`pay`**`or`**`show`**`or`**`auto`**`]`
* 显示有关您或其他玩家的宠物的以下信息。
  * 带有加法参数（整数）的 auto 确定玩家想要支付的最长时间
  * 示例：玩家使用 `/petrespawn auto 10`，宠物死亡，重生时间为 16 秒。现在插件会等到重生时间为 10 秒，然后在主人可以支付重生费时重生宠物。
* 别名：
  * `/petr`
  * `/pr`

#### `/petswitch` <a href="#petswitch" id="petswitch"></a>

* 允许您在宠物之间切换。
* 别名：
  * `/pswitch`

#### `/petstore` <a href="#petstore" id="petstore"></a>

* 允许您存放活跃的宠物
* 存储的宠物可以通过 `/petswitch` 命令检索
* 别名：
  * `/pstore`
  * `/pst`

#### `/pettrade` <a href="#pettrade" id="pettrade"></a>

* 语法： `/pettrade [`**`接受`或`拒绝`或`取消`**`或`**`<玩家名称`**>`] <价格>`
* 原文： `/pettrade [`**`accept`**`or`**`reject`**`or`**`cancel`**`or`**`a <player name>`**`] <price>`
* 将您当前的宠物提供给其他玩家。
  * `<价格>`可以是任何经济价格
* 别名：
  * `/pett`
  * `/pt`

#### `/petshop` <a href="#petshop" id="petshop"></a>

* 语法： `/petshop [商店名称]`
* 打开一个显示可用宠物店的 GUI
* 别名：
  * `/petsh`
  * `/psh`

#### `/petskill` <a href="#petskill" id="petskill"></a>

* 语法： `/petskill [玩家名称]`
* 显示有关宠物技能的信息。

#### `/petstop` <a href="#petstop" id="petstop"></a>

* 命令你的宠物停止攻击他的目标
* 在`农场`和`攻击性`行为模式下无用
* 原文：useless in `farm` and `aggressive` behavior modes
* 别名：
  * `/ps`
  * `/pets`

#### `/petchooseskilltree` <a href="#petchooseskilltree" id="petchooseskilltree"></a>

* 显示所有可用的技能树，并允许您为宠物选择技能树
*   别名：

    * `/pcst`
    * `/petcst`

    ![](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXxhRBA0Gdtn7pABVJu%2F-LXxjGwOuiPqa6FxvysK%2Fpcst.png?alt=media\&token=7124eaf1-fd1b-4722-b17d-9d4d41c73703)

#### `/petcapturehelper` <a href="#petcapturehelper" id="petcapturehelper"></a>

* 启用/禁用捕获助手
* 别名：
  * `/pch`

#### `/petoptions` <a href="#petoptions" id="petoptions"></a>

* 语法： `/petoptions <选项> [参数...]`
* 选项：
  * `healthbar`
    * 打开/关闭操作栏运行状况栏
  * `idle-volume`
    * 设置宠物发出的闲置声音的音量
    * 参数：
      * `<percent>`

### 技能命令 <a href="#skill-commands" id="skill-commands"></a>

#### `/petinventory` <a href="#petinventory" id="petinventory"></a>

* 语法： `/petinventory [玩家名称]`
* 打开宠物的物品栏
* 打开其他玩家的物品栏需要 _`MyPet.admin`_ 权限
* 别名：
  * `/pi`
  * `/peti`

#### `/petpickup` <a href="#petpickup" id="petpickup"></a>

* 打开/关闭宠物的取件
* ​![$](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXx\_oMwnEAUiDg5XPAj%2F-LXxbF5xExmAcZLOuRpO%2Fexclaim.gif?alt=media\&token=edb76aec-65d8-4904-ac04-03dd8139cc44)需要至少具有一排插槽的库存![$](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXx\_oMwnEAUiDg5XPAj%2F-LXxbF5xExmAcZLOuRpO%2Fexclaim.gif?alt=media\&token=edb76aec-65d8-4904-ac04-03dd8139cc44)​
* 别名：
  * `/pp`
  * `/petp`

#### `/petbehavior` <a href="#petbehavior" id="petbehavior"></a>

* 语法： `/petbehavior [模式]`
* 切换宠物的行为
* 模式：
  * `friendly` - >即使受到任何东西的攻击，宠物也不会打架
    * 朋友
  * `normal` - >宠物会像正常的狼一样行事
  * `aggressive` -> 在所有者的 15 个方块内自动攻击
  * `farm` -> 自动攻击 拥有者 15 个方块内的所有**怪物**
  * `raid` - 像平常一样>，但宠物不会攻击玩家和他们的爪牙（狼、豹猫、宠物）
  * `duel` ->宠物会在 5 个方块半径内以主动决斗行为攻击其他宠物
* 别名：
  * `/pb`
  * `/petb`

#### `/petbeacon` <a href="#petbeacon" id="petbeacon"></a>

* 打开宠物的`beacon`窗口
* 别名：
  * `/pbeacon`
  * `/petbeacon`

### 下面是本教程原文，您可以根据自己的英语水平自行理解

## Commands

### Legend <a href="#legend" id="legend"></a>

* Chatcommands
  * `<option>` -> **required**!
  * `[option]` -> optionalMost commands have aliases like `/pi`. Use them instead the long version.

**You can also go through the command options by using the autocompletion with the`[TAB]`-key.**

### MyPet Commands <a href="#mypet-commands" id="mypet-commands"></a>

#### `/mypet` <a href="#mypet" id="mypet"></a>

* shows all available _MyPet_ commands.

#### `/petinfo` <a href="#petinfo" id="petinfo"></a>

* Syntax: `/petinfo [username]`
* shows the following info about your or another player's pet.
  * hit-points
  * hunger
  * food items
  * behavior
  * experience
  * level
  * owner (only when pets isn't yours)
  * skilltree
* alias:
  * `/pinfo`

#### `/petname` <a href="#petname" id="petname"></a>

* Syntax:
  * `/petname <new-pet-name>`
* sets the name of your pet.
* owners can use colors to make the name of their pets more colorfull with this placeholder:
  * `<black>`, `<darkaqua>`, `<darkblue>`, `<darkgreen>`, `<darkred>`, `<darkpurple>`, `<gold>`, `<gray>`, `<darkgray>`, `<blue>`, `<green>`, `<aqua>`, `<red>`, `<lightpurple>`, `<yellow>`, `<white>`, `<magic>`, `<bold>`, `<strikethrough>`, `<underline>`, `<italic>`, `<reset>`

#### `/petrelease` <a href="#petrelease" id="petrelease"></a>

* Syntax: `/petrelease [pet-name]`
* release your pet so you don't have a pet anymore

#### `/petcall` <a href="#petcall" id="petcall"></a>

* teleports your pet to you.
* alias:
  * `/pc`
  * `/petc`

#### `/petsendaway` <a href="#petsendaway" id="petsendaway"></a>

* sends your pet away.
* it can be still called by using the `/petcall` command
* alias:
  * `/psa`
  * `/petsa`

#### `/petrespawn` <a href="#petrespawn" id="petrespawn"></a>

* Syntax: `/petrespawn [`**`pay`**`or`**`show`**`or`**`auto`**`]`
* shows the following info about your or another player's pet.
  * auto with an addition parameter (Integer) determines what the maximum time is the player want to pay for
  * Example: A player used `/petrespawn auto 10` and the pet dies and has a respawn time of 16 seconds. Now the plugin will wait until the respawntime is 10 seconds and then respawn the pet when the owner can pay the respawn fee.
* alias:
  * `/petr`
  * `/pr`

#### `/petswitch` <a href="#petswitch" id="petswitch"></a>

* allows you to switch between pets.
* alias:
  * `/pswitch`

#### `/petstore` <a href="#petstore" id="petstore"></a>

* allows you to store your active pet
* stored pets can be retrieved by the `/petswitch` command
* alias:
  * `/pstore`
  * `/pst`

#### `/pettrade` <a href="#pettrade" id="pettrade"></a>

* Syntax: `/pettrade [`**`accept`**`or`**`reject`**`or`**`cancel`**`or`**`a <player name>`**`] <price>`
* offers your current pet to another player.
  * `<price>` can be any economy price
* alias:
  * `/pett`
  * `/pt`

#### `/petshop` <a href="#petshop" id="petshop"></a>

* Syntax: `/petshop [shopname]`
* opens a GUI that shows the available pet shops
* alias:
  * `/petsh`
  * `/psh`

#### `/petskill` <a href="#petskill" id="petskill"></a>

* Syntax: `/petskill [playername]`
* shows info about the skills of your pet.
* as an admin this command you can also shows info about other player's pets

#### `/petstop` <a href="#petstop" id="petstop"></a>

* orders your pet to stop attacking his target
* useless in `farm` and `aggressive` behavior modes
* alias:
  * `/ps`
  * `/pets`

#### `/petchooseskilltree` <a href="#petchooseskilltree" id="petchooseskilltree"></a>

* shows all available skilltrees and lets you selects a skilltree for your pet
*   alias:

    * `/pcst`
    * `/petcst`

    ![](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXxhRBA0Gdtn7pABVJu%2F-LXxjGwOuiPqa6FxvysK%2Fpcst.png?alt=media\&token=7124eaf1-fd1b-4722-b17d-9d4d41c73703)

#### `/petcapturehelper` <a href="#petcapturehelper" id="petcapturehelper"></a>

* enables/disables the CaptureHelper
* alias:
  * `/pch`

#### `/petoptions` <a href="#petoptions" id="petoptions"></a>

* Syntax: `/petoptions <option> [parameters...]`
* options:
  * `healthbar`
    * toggles actionbar healthbar on/off
  * `idle-volume`
    * set the volume of the idle sound pets make
    * parameters:
      * `<percent>`

### Skill Commands <a href="#skill-commands" id="skill-commands"></a>

#### `/petinventory` <a href="#petinventory" id="petinventory"></a>

* Syntax: `/petinventory [playername]`
* opens the inventory of your pet
* opening the inventory of another player requires the _`MyPet.admin`_ permission
* alias:
  * `/pi`
  * `/peti`

#### `/petpickup` <a href="#petpickup" id="petpickup"></a>

* toggles pickup of your pet on/off
* ​![$](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXx\_oMwnEAUiDg5XPAj%2F-LXxbF5xExmAcZLOuRpO%2Fexclaim.gif?alt=media\&token=edb76aec-65d8-4904-ac04-03dd8139cc44)requires Inventory with at least one row of slots![$](https://1228222188-files.gitbook.io/\~/files/v0/b/gitbook-legacy-files/o/assets%2F-LXhRZyUgDZpPIQrYK1o%2F-LXx\_oMwnEAUiDg5XPAj%2F-LXxbF5xExmAcZLOuRpO%2Fexclaim.gif?alt=media\&token=edb76aec-65d8-4904-ac04-03dd8139cc44)​
* alias:
  * `/pp`
  * `/petp`

#### `/petbehavior` <a href="#petbehavior" id="petbehavior"></a>

* Syntax: `/petbehavior [mode]`
* toggles the behavior your pet
* modes:
  * `friendly` -> the pet will not fight even when it's attacked by anything
    * friend
  * `normal` -> the pet will act like a normal wolf
  * aggressive -> attacks automaticly everythink within 15 blocks of the owner
    * aggro
  * `farm` -> attacks automaticly every **Monster** within 15 blocks of the owner
  * `raid` -> like normal but the pet will not attack players and their minions (wolves, ocelot, pets)
  * `duel` -> pets will attack other pets with active duel behavior within a 5 block radius
* alias:
  * `/pb`
  * `/petb`

#### `/petbeacon` <a href="#petbeacon" id="petbeacon"></a>

* opens the beacon window of your pet
* alias:
  * `/pbeacon`
  * `/petbeacon`
