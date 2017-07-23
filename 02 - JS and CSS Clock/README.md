### 思路
- 一秒为单位的定时器，每秒触发时，获取当前时分秒，利用transform重置三个针的位置。
- 页面初始化的时候，将时分秒针重置的12点位置，（向前加90度）。
- 每一次重置时分秒针的位置，都要向前加90度。

### 错误
- 之前考虑，获取项目启动的秒数，每一秒向前加6度。

### 技术重点
- 获取时分秒的三个方法：
```
getHours() getMinutes() getSeconds()
```
- js修改transform的方法:
```
 DOM.style.transform = `rotate(${minsDegrees}deg)`;
 ```
- 要习惯使用const定义常量，如选中的dom元素
