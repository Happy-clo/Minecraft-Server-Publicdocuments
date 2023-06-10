# 领地指令教程

## 设置领地：

1. 用一根木棍左键敲击一方块设置点A，右键敲击一方块设置点B。（可以输入“`/res select size`”查看所选区域的大小）
2. 输入“`/res create 123`”（例）来创建一个以AB连线为体对角线的长方体的名为123的领地（包括A、B所在边），设置领地需要金钱。

## 移除领地：

输入“`/res remove 123`”（例）来移除名为123的领地。注意，移除领地无法从服务器获得金钱！

## 领地内权限设置：

输入“`/res set 123 flags true/false`”（例）来设置领地内的权限，其中：

* 123是领地名，不填则默认为当前所处领地；
* flags是权限，包括：move（移动）、build（改变地形）、place（放置物品）、destroy（破坏）、use（使用）、container（打开箱子）、pvp（玩家伤害）、tp（传送到该领地）、ignite（点火）、firespread（火的传播）、bucket（桶的使用）、flow（后面两个总括）、lavaflow（岩浆流动）、waterflow（水的流动）、creeper（JJ怪爆炸）、tnt（TNT爆炸）、monsters（怪物出生）、animals（动物出生）、subzone（子空间）、healing（治疗）和piston（活塞）（活塞不适用于单人命令）；
* true/false是权限状态，若输入true则为开启，false则为关闭。

也可以进行单人权限设置，例如：拿destroy权限来举例，输入“`/res pset 领地名字 玩家名字 destroy true`”。

## 子空间设置：

1. 如同设置领地一样选择区域。
2. 输入“`/res subzone 123 abc`”（例）来设置母领地为123的名为abc的子空间，该区域的权限设置和移除需要将领地名变为123.abc，如果没有则默认为当前所处领地（在子空间则为子空间）。

### **选择命令**

* `/res select [x] [y] [z]` - 选择领地的长方体区域，X Y 和 Z 都是从你当前位置为中心的距离，你也可以用一个工具（默认是木锄）来选择地块。
* `/res select chunk` - 选取一整个 Chunk。
* `/res select expand [格数]` - 向你的前方延伸选区。
* `/res select size` - 显示已选择区域的尺寸。
* `/res select shift [格数]` - 向你的前方移动选区。
* `/res select vert` - 把选区延伸到从天顶到地底。

### 创建命令：

* `/res area [add/remove/replace] <领地名> [区域id]` - 向叫做\[领地名]的领地增加(add)、从其中去除(remove)或是替换 (replace) 区域。可与同一领地内的区域重合。
* `/res create [领地名]` - 选择好区域后创建一个叫做\[领地名]的领地
* `/res remove [领地名]` - 移除一个叫\[领地名]的领地
* `/res removeall` - 移除所有领地
* `/res subzone <领地名> [子区域名]` - 在领地内创建一块子区域，你必须是所有者才行。

### 信息命令：

* `/res area list [领地名]` - 列出某领地的所有区域
* `/res area listall [领地名]` - 列出某领地的所有区域以及他们的坐标
* `/res current` - 显示你所在的领地
* `/res info <领地名>` - 得到某领地的信息
* `/res list` - 显示你拥有的领地
* `/res limits` - 显示重要的权限
* `/res sublist` - 显示你所在领地的所有子区域

### 权限命令：

* `/res gset <领地名> [群组名] [权限] [true/false/remove]` - 设置某领地对于某群组的权限
* `/res lset <领地名> [黑名单/忽略名单] [材质]` - 从某领地的黑名单/忽略名单中增加/移除某材质
* `/res lset <领地名> info` - 显示某领地的黑名单/忽略名单设置
* `/res pset <领地名> [玩家名] [权限] [true/false/remove]` - 设置某领地对于某玩家的权限
* `/res set <领地名> [权限] [true/false/remove]` - 设置某领地的权限

### 其他命令：

* `/res default [领地名]` - 重置某领地的权限设置
* `/res give [领地名] [玩家名]` - 将某领地赠与某玩家，你必须是领主且被赠予玩家在线
* `/res lists` - 预定领地许可清单的详细信息
* `/res message [领地名] [enter/leave] [信息]` - 设置进入/退出某领地时候显示的信息
* `/res message [领地名] remove [enter/leave]` - 移除进入/退出某领地时候的信息
* `/res mirror [源领地名] [目标领地名]` - 复制源领地的权限设置至目标领地
* `/res rename - [旧名称] [新名称]` - 重命名领地.对于子空间旧名称必须全名，新名称可以只写子空间名
* `/res renamearea [领地名] [旧名称] [新名称]` - 重命名某领地中某区域的名称
* `/res tp [领地名]` - 传送至某领地
* `/res tpset` - 设置当前领地的传送点为你站立的地方
* `/res unstuck` - 将你从当前领地移出

### 交易命令

* `/res lease [renew/cost] [领地名]`：更新/显示一个领地的费用。
* `/res market list`：显示在售的所有领地。
* `/res market info [领地名]`：显示在售的某个领地的信息。
* `/res market sell [领地名] [价格]`：将某个领地出售。
* `/res market unsell [领地名]`：将某个领地下架。
* `/res market buy [领地名]`：购买某个领地。
* `/res market rentable [领地名] [价格] [天数] <repeat:t/f>`：将某个领地以指定价格和天数出租，并设置是否可自动续期。
* `/res market rent [领地名] <repeat:t/f>`：设置某个领地是否可以出租并设置是否可自动续期。
* `/res market release [领地名]`：解除某个领地的出租。

### 注：以上命令不写领地名则为当前所在的领地

### 权限表：

* admin：领地的全权管理权限，仅能给与某玩家。
* container：是否能使用箱子、发射器等容器类物品。
* bucket：设置是否能使用桶。
* ignite：点火的权限。
* piston：活塞是否能使用。
* build：建造权限（包括 destroy 和 place）。
* destroy：毁坏权限。
* place：放置权限。
* move：进入权限。
* tp：传送权限。
* use：使用权限（工作台、炉子等）。
* subzone：是否能设置子空间。
* tnt：设置 TNT 是否有效。
* creeper：设置苦力怕是否有效（设置 F 的话苦力怕就废了）。
* damage：设置领地内是否能造成伤害（不能防止被挤死）。
* monsters：设置是否刷新怪物。
* animals：设置是否刷新动物。
* firespread：火是否能蔓延。
* flow：液体流动，包括 waterflow 和 lavaflow。
* waterflow：水的流动。
* lavaflow：岩浆流动。
* healing：设置是否能恢复生命。
* pvp：设置是否能进行 PVP。
