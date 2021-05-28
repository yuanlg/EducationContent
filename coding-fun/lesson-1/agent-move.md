### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# 编写程序让代理机器人到达黄金块上

## 第一步
 选中``||player:当聊天命令为  时||`` 指令块 并且把 **run** 改为 **1**. 选择一个 ``||agent: 代理机器人移动方向 前 距离 1|`` 指令块并把它拖拽到 ``||player:当聊天命令为  时||`` 里面. 把 距离后面的数字**1** 改为**3**，让机器人向前走3步, 这样代理机器人就可以打到金块上. 完成后，按**播放**按钮编译代码，然后进入Minecraft，按**t**并输入**1**，然后按回车键。

#### ~ 教程提示 
你可以通过修改`` | | Agent:代理机器人移动方向 前 距离 1 | ``命令块中的数字来修改机器人要移动的步数。你还可以使用` | | agent:代理机器人转动方向 左 | | ``命令块将机器人向左或向右转动。



```ghost
player.onChat("1", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

``` 
