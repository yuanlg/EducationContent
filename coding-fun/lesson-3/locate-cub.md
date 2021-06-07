### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# 寻找cub!

## Step 1
编程让代机器人挖掘通道，当不知道要挖多远时，需要使用 ``||loops:循环||`` & ``||agent:代理机器人检测||`` 指令.代理机器人需要使用 ``||agent:代理机器人摧毁 方向 上||`` 指令帮你从雪中走出来! 代码编写好后, 按下 **播放** 按钮来编译代码.不要忘了在mc中执行你的代码. 

#### ~ 教学提示 
当你把代码编写好后仔细检查一下. 使用 ``||agent:代理机器人移动方向 前||``.

```template
player.onChat("cub", function () {
    while (agent.detect(AgentDetection.Block, FORWARD)) {
    	
    }
})
```

```ghost
player.onChat("cub", function () {
    while (agent.detect(AgentDetection.Block, FORWARD)) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
        agent.destroy(UP)
    }
})

``` 
