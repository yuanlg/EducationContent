### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# 编写程序让代理机器人到达黄金块上!

## 第一步
编写程序让机器人移动到黄金块上。你需要留在你的黄金快上，而机器人需要留在另一个黄金快上。完成后，按**播放**按钮编译代码。去Minecraft运行你的代码。


```ghost
player.onChat("last", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```  
