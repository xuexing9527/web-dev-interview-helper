# $nextTick
### $nextTick的主要作用是：
- 提供一个在 DOM 更新完成之后的 “回调函数执行环境”，数据变化导致 DOM 变化之后，立即执行一些操作。  
- 用于延迟执行回调方法，确保在 DOM 更新之后执行。

### 使用场景：
- 访问 DOM 元素。数据变化后，获取 DOM 元素的尺寸或状态
- 计算依赖于最新 DOM 元素状态的 数据


### 原理
- 基于微任务实现的
    - promise
    - MutationObserver (稍旧浏览器)
    - setImmediate (IE 10+)
    - setTimeout (最后的降级)