# Vue3 的新特性
- Composition API（组合式 API）：Vue 3 引入了 Composition API，这是一种新的 API 风格，使得代码更加灵活和可组合。它允许将相关逻辑组合在一起，而不是按照选项的顺序组织代码。

- 新的响应式，proxy实现
    - 只能拦截属性的读取和写入，无法处理删除属性等其他操作。
    - 需要预先知道对象的所有属性，并为每个属性手动定义 getter 和 setter。
    - 对于嵌套对象，需要递归地为每个子属性定义响应式处理，性能开销较大。

- Suspense