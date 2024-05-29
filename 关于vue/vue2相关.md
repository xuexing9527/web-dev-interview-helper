# vue2 相关
- computed 和 watch 的区别和应用场景
    - computed是计算属性，其结果具有缓存属性，只有它依赖的值发生变化，才会在下次获得computed的值的时候重新计算computed。一般在进行数值计算并且依赖他的结果时使用。
    - watch 是"监听"

    (1)计算属性有缓存机制,侦听器没有  
    (2)计算属性不支持异步操作, 侦听器支持异步操作  
    (3)计算属性是一个额外新增的属性， 侦听器只能侦听data中的属性  
    (4)计算属性有返回值return,侦听器不需要return  
    (5)计算属性可以监听多个数据变化(计算属性内部用到的数据变化了，就会执行计算属性方法), 侦听器只能侦听一个数据的变化。  
- 生命周期【10个】

- 谈谈keep-alive的理解
    - 概念：缓存组件状态的内置组件
    - 两个相对应的生命周期函数
        - actived 激活
        - deactived 停用(不激活)
    - 问题思考
        - 什么时候被 keep-alive 包裹的组件会触发 distory 类钩子呢？
            - 没有被 keep-alive 包裹的父组件被切换时，父组件内部的 keep-alive 包裹的子组件会触发 distory 类钩子
            - v-if 条件渲染 keep-alive 包裹的组件，会触发 distory 类钩子

- 组件间通信的几种方式
    - props
    - $emit
    - ref
    - provide inject 依赖注入
    - eventBus
    - mixins
    - slot
    - router

- $nextTick

- 如何实现组件缓存

-  Vue是如何实现双向数据绑定的
    - Object.defineProperty()

- Vue常用修饰符有哪些

- Vue中有时候数组会更新页面，有时候不更新为什么？
    - push()
    
    - slice()