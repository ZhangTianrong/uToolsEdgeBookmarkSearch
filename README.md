# Edge 小助手

> 通过 uTools 来查看和搜索 Edge 浏览器书签

修改自 Licardo 根据 [Chrome 小助手](https://github.com/in3102/utools-chrome_helper) 制作的 [Edge 小助手](https://github.com/L1cardo/Edge-Helper-uTools)。

## 功能变更

+ ☒ 取消了开始状态下搜索所有书签的行为（Chrome 小助手原本的逻辑更舒服）
+ ☒ 取消了显示链接图标的行为（这些图标是真的不好看……况且浏览器`Favicons`是以数据库形式存储，`JavaScript`不好直接访问，与其猜测图标`URI`不如缺省）
+ ☑ 通过[该库](https://github.com/sxei/pinyinjs)增加了使用拼音搜索对应中文的功能（只有我觉得这是刚需吗？）
+ ☑ 增加了对书签文件夹的支持，形如`[PATTERN1]:[PATTERN2]`（中英文冒号皆可）的搜索语句会被解读为通过`[PATTERN1]`匹配路径，`[PATTERN2]`匹配书签标题
    + 比如`ziyuan:pan`可以match`资源`文件夹下`XX网盘搜索引擎`而不会match`工具`文件夹下的`XX网盘转存`诸如此类，如果你的书签目录很深形如`[DIR1\DIR2]`的搜索字段也可以帮助筛选。
    + 当然，每个人整理书签的方法是不一样的，上述场景未必会出现在每个人的日常使用中，但只要有大致的目录划分，那么这个功能总可以用来在一定程度上代替浏览器原生的`书签浏览器`，比如当你只是想要浏览一个目录下所有书签时，不妨留空`[PATTERN2]`。

## 碎碎念

平时只写`C`和`python`，不会写`JavaScript`，每次告诉自己不要学用啥查啥就行了，但`JavaScript`总能让我非很长花时间摸索不可……我真的只是从Chrome迁移到Edge之后一时兴起想要顺便补全之前没有的功能而已……