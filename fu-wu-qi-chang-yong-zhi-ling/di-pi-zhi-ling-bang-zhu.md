# 地皮指令教程

## 以下是一些常用的玩家指令，以及它们的用法和示例。

### 基础指令

#### /plot auto

这个指令会自动为你分配一个空地块。你只需要站在任何位置，并输入：

```
/plot auto
```

#### /plot home

这个指令会将你传送回你当前拥有的地块的主要传送点。在你拥有多个地块时非常方便，你只需要输入：

```
/plot home
```

#### /plot claim

这个指令可以用来申请一个新的地块。如果你站在一个没有被其他玩家占据的空地上，输入：

```
/plot claim
```

就可以获得该地块的所有权。

#### /plot add

这个指令可以用来将其他玩家添加到你所拥有的地块中。你需要先拥有该地块的所有权，然后输入：

```
/plot add <player>
```

其中 `<player>` 是被邀请加入的玩家的用户名。例如，要将用户 "Steve" 添加到你的地块中，输入：

```
/plot add Steve
```

#### /plot remove

这个指令可以用来将其他玩家从你所拥有的地块中移除。你需要先拥有该地块的所有权，然后输入：

```
/plot remove <player>
```

其中 `<player>` 是要从地块中删除的玩家的用户名。例如，要将用户 "Alex" 从你的地块中移除，输入：

```
/plot remove Alex
```

#### /plot trust

这个指令可以用来让其他玩家在你的地块上执行一些特定的操作。你需要先拥有该地块的所有权，然后输入：

```
/plot trust <player> <permission>
```

其中 `<player>` 是被授权的玩家的用户名，`<permission>` 是被授权的权限。例如，要让用户 "Bob" 在你的地块上建造和破坏方块，输入：

```
/plot trust Bob build,destroy
```

#### /plot untrust

这个指令可以用来撤回其他玩家在你的地块上的权限。你需要先拥有该地块的所有权，然后输入：

```
/plot untrust <player> <permission>
```

其中 `<player>` 是被撤销权限的玩家的用户名，`<permission>` 是要撤销的权限。例如，要撤销用户 "Sarah" 在你的地块上建造和破坏方块的权限，输入：

```
/plot untrust Sarah build,destroy
```

* `/plot help claiming`：地皮申领相关的帮助。
* `/plot help teleport`：地皮传送相关的帮助。
* `/plot help settings`：地皮保护相关的帮助。
* `/plot help schematic`：网页相关的帮助。
* `/plot help info`：信息相关的帮助。
* `/plot help all`：地皮全面帮助。
