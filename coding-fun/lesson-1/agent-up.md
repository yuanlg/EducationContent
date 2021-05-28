### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# 通过编程让机器人到黄金块上去！

## Step 1
使用 ``||player:当聊天命令为 时|`` 和  ``||agent: 代理机器人移动方向 前 距离 1||`` 命令快 让机器人移动到黄金块上. 你可以编程让机器人向 **上**移动. 完成后，按**播放**按钮编译代码，然后进入Minecraft，按**t**并输入**1**，然后按回车键。



```ghost
player.onChat("up", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

```  
