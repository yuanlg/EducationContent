### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# 让机器人沿着海龟的足迹移动!

## 第一步
通过使用``||agent: 代理机器人移动方向 前 距离 1 ||`` 和 ``||agent: 代理机器人转动方向 左 ||``指令快让机器人沿着海龟足迹移动.完成后，按播放按钮编译代码，不要忘记在Minecraft里运行你的代码. 

```ghost
player.onChat("tracks", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
for (let index = 0; index < 4; index++) {
    	
 }
``` 
