## 1 概念
> 默认值为0 表示不占用剩余的空白间隙扩展自己的宽度

## 2 单行单个元素
> 当前行有单个元素 并且没有占领满所有空白(剩余的空白值 * 扩展比例(最小为0 最大为1(占满剩余所有空间) 你输入大于小于这些阈值是按照阈值算)) `真实大小 = 当前元素的大小 + 剩余的空白值 * 扩展比例`

## 3 单行多(n)个元素
> `说明：flex-grow值(1 整数 2 最小值大于等于0 小于0还是0  `3 最大值理论上不限`)`

> **若多(n)个元素有剩余空间(Remaining) = 当行宽度 - n个元素宽(它们的和)**

> **现在n个元素 部分/全部要扩展自己的大小 计算公式：剩余空间(Remaining) * (每个flex-grow值(最小值大于等于0) / (每个flex-grow的值相加的和 > 1 ? 每个flex-grow的值相加的和 : 每个flex-grow的值相加的和 = 1))**

## 4 小结
> 说白就是对剩余空间的占有 怎么分配的问题 flex-grow值的比例获取大小