### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# 让机器人沿着海龟的足迹移动并摧毁障碍物!

## 第一步
通过同时使用``||agent: 代理机器人摧毁方向 前||`` 和 ``||agent:代理机器人收集所有||``指令块让机器人**摧毁树干**.尝试使用 ``||loops:重复 4 次||`` 指令块让代码有效率. 完成后，按播放按钮编译代码， 不要忘记在Minecraft里运行你的代码. 


```ghost
player.onChat("path", function () {
    for (let index = 0; index < 4; index++) {
        agent.turn(LEFT_TURN)
        agent.move(FORWARD, 1)
        agent.destroy(FORWARD)
        agent.collectAll()
    }
})
``` 

