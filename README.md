# LeetCodeStudy

数据结构和算法的学习


## 工具
- [如何直观形象地树状打印一棵二叉树](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/打印树/如何直观形象地树状打印一棵二叉树？.md)

## 数据结构

- [1、算法效率的度量](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/算法效率的度量.md)
- [2、栈和队列](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/栈和队列/栈和队列.md)
- [3、链表](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/链表/链表.md)
- [4、递归](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/递归/递归.md)
- [5、二叉树](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/二叉树/二叉树.md)
- [6、集合和映射](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/集合和映射/集合和映射.md)
- [7、优先队列](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/优先队列/优先队列.md)
- [8、线段树](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/线段树/线段树.md)
- [9、Trie](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/Trie/Trie.md)
- [10、并查集](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/并查集/并查集.md)
- [11、平衡二叉树](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/平衡二叉树/平衡二叉树.md)
- [12、哈希表](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/数据结构/哈希表/哈希表.md)




***********************************************

## 算法

在开始之前我们先来写一个帮助测试的函数
```
// 生成有n个元素的随机数组,每个元素的随机范围为[rangeL, rangeR]

func generateRandomArray(count:Int,rangL:Int,rangR:Int) -> Array<Int> {

    if rangR <= rangL{
        fatalError("取值范围不准确")
    }

    var arr:[Int] = Array()
    for _ in 0..<count {
        let arc = rangR - rangL + 1
        let item:Int = Int(arc4random()) % arc + rangL
        arr.append(item)
    }

    return arr
}



// 判断arr数组是否有序
func isSorted(arr:[Int]) -> Bool {
    for i in 0..<arr.count-1 {
        if arr[i] > arr[i+1] {
            return false
        }
    }
    return true
}
```

- [十大经典排序算法](https://www.runoob.com/w3cnote/ten-sorting-algorithm.html)
- [1、简单排序](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/算法/简单排序算法/简单排序算法.md)
- [2、归并排序](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/算法/归并排序/归并排序.md)
- [3、快速排序](https://github.com/SunshineBrother/LeetCodeStudy/blob/master/算法/快速排序/快速排序.md)
