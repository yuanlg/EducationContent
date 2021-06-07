### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# 分离的家庭!

## 第一步
让代理机器人在冰裂缝上建桥. 确保代理机器人的背包里有 **64** 块  **橡木板**. 

#### ~ 教学提示 
不要忘记在**循环**指令中使用 **非** 指令. 想想你想让代理机器人把橡木板放在哪里. 


```ghost
player.onChat("family", function () {
    agent.setItem(PLANKS_OAK, 64, 1)
    agent.move(FORWARD, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
        agent.turn(LEFT_TURN)
    }
})

``` 
