## promise 可以中断吗？

### 基本概念

    promise 分三个状态，pending, fulfilled, rejected，三个状态。后两个又被称为 settled （已定型）状态，表示 promise 已经结束。

### 中断背景描述

    如果一个 promise pending 速度较快，一般不需要考虑中断，毕竟想要中断一个快速的 pending 还得考验手速。如果当一个 promise pending 时间太长，pending 过程中不想等待了，这个时候就需要中断这个 promise 了。

    理论上 promise 的中断，是指 pending 阶段，阻止 promise 接下来的操作。  