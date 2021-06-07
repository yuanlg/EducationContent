### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration false 
### @explicitHints 1


# 高地!

## 第一步
编程让代理机器人使用**10**块**橡木** 方块建造一个塔. 首先使用 ``||agent:代理机器人获取方块或物品||``指令获取**64** 块 **橡木**方块. 然后使用``||agent:代理机器人放置方向||`` 指令向**前**, **左** & **右** 放置橡木块. 代理机器人放置后需要**向上移动** .  

#### ~ 教程提示 
 尝试使用``||loops:循环||`` 命令块 同时把循环次数修改为 **10**. 

## 第二步
编程让代理机器人从塔上向下移动同时建造 **10** 块高的 **梯子** . 你需要梯子才能爬上去!

#### ~ 教程提示 
不要忘了使用``||agent: 代理机器人获取方块或物品||``指令，并指定 **64** 块 **梯子**  , 让后让代理机器人把梯子放好. 


```ghost
player.onChat("tower", function () {
    agent.move(FORWARD, 1)
    agent.setItem(LADDER, 64, 1)
    for (let index = 0; index < 10; index++) {
        agent.place(FORWARD)
        agent.move(UP, 1)
    }
    agent.move(DOWN, 10)
})

``` 


