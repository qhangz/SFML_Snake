# SFML_Snake
### SFML版本的贪吃蛇
>来自游戏程序设计
游戏玩法在图形界面右侧都有显示
为了避免在输入模块设计时，如果同时按多个键，存在蛇调头导致的可能，导致游戏立即结束的问题：将时间抖动设置在dirChange上，实现keyClockDelay时间后才能进行下一次方向更新（初步是想到这样的实现方法）。
这个时间还是不好控制啊，随着游戏帧率的提高，两次响应的时间间隔的设置还是容易出现问题，所以将游戏逻辑设置为，当蛇头步进一个各自之后再响应下一个方向变换，这样解决相对来说效果更好一点。