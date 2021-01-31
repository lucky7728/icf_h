# 大纲

##### 1232 缀点成线

- double类型数据比较
- 向量的相关性判断是够共线

##### 721 账户合并

- 并查集
- vector的insert用法，向量中插入vector

##### 1584 连接所有点的最小费用

- prim算法
- lambada表达式
- Kruskal算法
- 依据对象某一属性对对象进行排序,sort

##### 628 三个数最大乘积

- 分情况想像一下即可...
- 使用反向迭代器进行排序

##### 1489 找到最小生成树里的关键边和伪关键边

- 并查集按秩优化
- clsukal算法
- 关键边的分析

##### 17 九键字母

##### 18 二维数组查找单词

##### 46 全排列

##### 50 全排列2

##### 78 子集

##### 90 子集2

##### 216 三个数的和

##### 52 N皇后

##### 37 数独

## 树

##### 98 验证二叉搜索树

- 二叉搜索树的定义
- 解法一：二叉搜索树的中序遍历是升序
- 解法二：任一节点能唯一确定一个范围，自顶向下的方法
- 递归的写法

##### 94 二叉树的中序遍历

- 迭代的写法
- 递归的写法

##### 101对称二叉树
- 验证二叉树和二叉树中序遍历的升级版本
- 迭代写法
- 递归写法

##### 105从前序遍历以及中序遍历构造二叉树

- 递归
- **~~迭代~~**

##### 102 二叉树的层次遍历

- 利用队列求二叉树的层次遍历
- C++队列的api

##### 236 二叉树的最近公共祖先

- 深入理解递归的题目
- [优秀题解](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/solution/236-er-cha-shu-de-zui-jin-gong-gong-zu-xian-hou-xu/)

##### 124 二叉树中的最大路径和

- 权重为负数
- 104题的升级版本

##### 687 最长同值路径

- 综合题
- [优秀题解](https://leetcode-cn.com/problems/longest-univalue-path/solution/687-by-ikaruga/)

##### 543 二叉树的直径

- 递归
- [优秀题解](https://leetcode-cn.com/problems/diameter-of-binary-tree/solution/shi-pin-jie-shi-di-gui-dai-ma-de-yun-xing-guo-chen/)

##### 104 二叉树的最大深度

- 迭代
- 简单题

##### 173 二叉搜索树迭代器

- 中序遍历的迭代写法
- 理解题目的意思

##### 297

## 滑动窗口、双指针、单调队列、单调栈

##### 167 两数之和

- 暴力解法
- 双指针

##### 88 合并两个有序数组

- 三指针
- 从后往前

##### 26 删除排序数组的重复项

- 最后一个元素问题
- 指针的思想，以及指针表示的实际意义

##### 76 最小覆盖子串

- 滑动窗口
- 哈希表的使用
- 困难

##### 32 最长有效括号

- 括号的性质

##### 42 最小栈

- 辅助栈
- 应该不需要优化

##### 155 接雨水

- 单调栈解决一类问题
  - 快速查找每个数左侧第一个比他他的水
- 单调队列
  - 查找滑动窗口的最值

##### 84 柱状图中的最大矩形

- 单调栈模版

##### 918 环形子数组的最大和

- 

##### 239 滑动窗口最大值

- 单调队列的暴力解法
- 

##### 496 下一个更大的元素(1)

##### 503 下一个更大元素(2)

##### 739 每日温度

##### 901 股票价格跨度

## 贪心

##### 860 柠檬水找零

- 模拟+贪心
- 贪心算法(某种意义上的局部最优解)

##### 392 判断子序列

- 双指针问题，单调性
- 大量需要验证的子序列的处理办法

##### 455 分发饼干

- 暴力解法
- 排序优化

##### 55 跳跃游戏

- 贪心的思想
- for循环的使用

##### 45跳跃游戏(2)

- 

##### 376

##### 406

##### 452

##### 402

##### 134

## 基础算法

##### 快速排序

- 快速排序是不稳定的

- 算法思想
  - 分冶算法
- 算法步骤
  - 确定分界点，在排序的数组中随机选择一个点作为分界点
  - 调整区间，使得第一个区间的数均小于等于x，右边的数均大于等于x【难点】
  - 递归处理左右两端
- 算法技巧
  - 双指针交换数值，完成调整区间这一步

##### 归并排序

- 归并算法是稳定的
- 复杂度 nlogn

- 算法主题思想和快速排序一样
- 确定分界点这一处选定的是中间的分界点
- 将两个有序的数组合并，合二为一【难点】
  - 算法技巧
    - 双指针算法

##### 整数二分

- 寻找边界问题，左边界满足某种性质，右边界不满足某种性质
- 只要我们能找到这个性质，我们就可以使用二分找到这个性质的分界点
- 有单调性可以用二分，没有单调性也有二分
- 算法步骤
  - 定中点
  - 检查中点，check函数
- 二种模版
  - 区间被划分为```[l,mid-1][mid,r]```时使用
  - 区间被换分为```[l,mid][mid+1,r]```时使用
- 先写模版，在考虑是否需要加1
- 一定要有解，但可以根据边界判断题目对否有解

##### 实数二分

- 考虑浮点数精度问题，一般是保留位数加上2
- 直接暴力循环100次，保证精度

##### 高精度

- 对大的数进行加减乘除

- 大整数的存储

  - 大数使用string读进来，然后赋值到数组当中
  - C++中大整数的存储(123456789),使用数组进行存储，低位存个位数
  - 如果需要进位，高位加一，在数组末端加上一个数比较容易

- 高精度加减法

  - 使用进位标志即可
  - 模拟

- 高精度乘法

  - 一个大数乘以一个小一点的数
  - 高精度乘法把小数当做一个整体，仍然使用进位标志来求
  - LeetCode 43

- 高精度除法

  - 一个高精度数除以一个低精度数
  - 

  



##### 











