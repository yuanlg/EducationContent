### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# 大峡谷

## 第一步
编程让代理机器人在冰裂缝上 **建一座桥** . 使用 ``||获得方块或物品||`` 指令确保代理机器人的背包中有所需要的物品. 选择**橡木**作为建桥材料，数量选择**64**. ``||loops:循环||`` 代理机器人 **非** 检测到前面有方块, 编写代码让代理机器人向 **下**放置橡木并向**前**移动来修建桥.    


```template
player.onChat("chasm", function () {
    agent.setItem(PLANKS_OAK, 1, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, DOWN))) {
    	
    }
})
```

```ghost
player.onChat("chasm", function () {
    agent.setItem(PLANKS_OAK, 64, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
})

``` 

