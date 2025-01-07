[LeetCode-JS 通关指南](https://2xiao.github.io/leetcode-js/)

# General Info

<details>
  <summary>
    数据结构与算法 Data Structures and Algorithms
  </summary>

9 个数据结构：[数组](https://2xiao.github.io/leetcode-js/book/array.html)、[链表](https://2xiao.github.io/leetcode-js/book/linked_list.html)、[栈](https://2xiao.github.io/leetcode-js/book/stack.html)、[队列](https://2xiao.github.io/leetcode-js/book/queue.html)、[哈希表](https://2xiao.github.io/leetcode-js/book/hash.html)、[树](https://2xiao.github.io/leetcode-js/book/tree.html)、[堆](https://2xiao.github.io/leetcode-js/book/heap.html)、[图](https://2xiao.github.io/leetcode-js/book/graph.html)、[字符串](https://2xiao.github.io/leetcode-js/book/string.html);
  
11 个算法：[枚举算法](https://2xiao.github.io/leetcode-js/book/enumeration.html)、[递归算法](https://2xiao.github.io/leetcode-js/book/recursion.html)、[分治算法](https://2xiao.github.io/leetcode-js/book/divide_conquer.html)、[回溯算法](https://2xiao.github.io/leetcode-js/book/backtracking.html)、[贪心算法](https://2xiao.github.io/leetcode-js/book/greedy.html)、[动态规划](https://2xiao.github.io/leetcode-js/book/dynamic_programming.html)、[位运算](https://2xiao.github.io/leetcode-js/book/bit.html)、[排序算法](https://2xiao.github.io/leetcode-js/book/sort.html)、[二分查找](https://2xiao.github.io/leetcode-js/book/binary_search.html)、[双指针](https://2xiao.github.io/leetcode-js/book/two_pointer.html)、[滑动窗口](https://2xiao.github.io/leetcode-js/book/slide_window.html); </details>

Data Structures and Algorithms

9 Data Structures:

Array, Linked List, Stack, Queue, Hash Table, Tree, Heap, Graph, String

11 Algorithms:

Enumeration Algorithm, Recursive Algorithm, Divide and Conquer Algorithm, Backtracking Algorithm, Greedy Algorithm, Dynamic Programming, Bit Manipulation, Sorting Algorithm, Binary Search, Two Pointers, Sliding Window

![1-1-1-RNsJLNFS](https://github.com/user-attachments/assets/a50752bd-3f2a-4262-973d-9de77c37f57f)


# Time Complexity of an Algorithm

Time complexity is a function that qualitatively describes the running time of an algorithm. It is used to evaluate the time consumed by executing a program, allowing an estimation of the program’s impact on processor usage.

Time complexity is commonly expressed using Big O notation. In this context, time complexity is considered asymptotic, meaning it examines the behavior of the algorithm as the input size approaches infinity.

大 O 标记法 | 计算 10 个元素 | 计算 100 个元素 | 计算 1000 个元素
-- | -- | -- | --
O(1) | 1 | 1 | 1
O(log N) | 3 | 6 | 9
O(N) | 10 | 100 | 1000
O(N log N) | 30 | 600 | 9000
O(N^2) | 100 | 10000 | 1000000
O(2^N) | 1024 | 1.26e+29 | 1.07e+301
O(N!) | 3628800 | 9.3e+157 | 4.02e+2567



<details>
  <summary>
    数据结构操作的复杂性 Complexity of Data Structure Operations
  </summary>

数据结构 | 连接 | 查找 | 插入 | 删除 | 备注
-- | -- | -- | -- | -- | --
数组 | 1 | n | n | n |  
栈 | n | n | 1 | 1 |  
队列 | n | n | 1 | 1 |  
链表 | n | n | 1 | 1 |  
哈希表 | - | n | n | n | 在完全哈希函数情况下，复杂度是 O(1）
二分查找树 | n | n | n | n | 在平衡树情况下，复杂度是 O(log(n))
B 树 | log(n) | log(n) | log(n) | log(n) |  
红黑树 | log(n) | log(n) | log(n) | log(n) |  
AVL 树 | log(n) | log(n) | log(n) | log(n) |  
布隆过滤器 | - | 1 | 1 | - | 存在一定概率的判断错误（误判成存在）

</details>

| **Data Structure**    | **Access** | **Search** | **Insert** | **Delete** | **Notes**                                   |
|------------------------|------------|------------|------------|------------|---------------------------------------------|
| **Array**             | O(1)       | O(n)       | O(n)       | O(n)       | -                                           |
| **Stack**             | O(n)       | O(n)       | O(1)       | O(1)       | -                                           |
| **Queue**             | O(n)       | O(n)       | O(1)       | O(1)       | -                                           |
| **Linked List**       | O(n)       | O(n)       | O(1)       | O(1)       | -                                           |
| **Hash Table**        | -          | O(n)       | O(n)       | O(n)       | Complexity is O(1) with a perfect hash function |
| **Binary Search Tree** | O(n)       | O(n)       | O(n)       | O(n)       | Complexity is O(log(n)) for balanced trees |
| **B-Tree**            | O(log(n))  | O(log(n))  | O(log(n))  | O(log(n))  | -                                           |
| **Red-Black Tree**    | O(log(n))  | O(log(n))  | O(log(n))  | O(log(n))  | -                                           |
| **AVL Tree**          | O(log(n))  | O(log(n))  | O(log(n))  | O(log(n))  | -                                           |
| **Boolean**      | -          | O(1)       | O(1)       | -          | Has a probability of false positives        |




<details>
  <summary>
    数组排序算法的复杂性 Complexity of Array Sorting Algorithms
  </summary>

排序算法 | 平均时间复杂度 | 最好情况 | 最坏情况 | 空间复杂度 | 排序方式 | 稳定性
-- | -- | -- | -- | -- | -- | --
冒泡排序 | O(n^2) | O(n) | O(n^2) | O(1) | in-place | 稳定
选择排序 | O(n^2) | O(n^2) | O(n^2) | O(1) | in-place | 不稳定
插入排序 | O(n^2) | O(n) | O(n^2) | O(1) | in-place | 稳定
希尔排序 | O(nlogn) | O(nlog^2n) | O(nlog^2n) | O(1) | in-place | 不稳定
归并排序 | O(nlogn) | O(nlogn) | O(nlogn) | O(n) | out-place | 稳定
快速排序 | O(nlogn) | O(nlogn) | O(n^2) | O(logn) | in-place | 不稳定
堆排序 | O(nlogn) | O(nlogn) | O(nlogn) | O(1) | in-place | 不稳定
桶排序 | O(n+k) | O(n+k) | O(n^2) | O(n+k) | out-place | 稳定
计数排序 | O(n+k) | O(n+k) | O(n+k) | O(k) | out-place | 稳定
基数排序 | O(n*k) | O(n*k) | O(n*k) | O(n+k) | out-place | 稳定

</details>

| **Sorting Algorithm** | **Average Time Complexity** | **Best Case** | **Worst Case** | **Space Complexity** | **Sorting Type** | **Stability** |
|------------------------|-----------------------------|---------------|----------------|-----------------------|------------------|---------------|
| **Bubble Sort**        | O(n^2)                     | O(n)          | O(n^2)         | O(1)                 | In-place         | Stable        |
| **Selection Sort**     | O(n^2)                     | O(n^2)        | O(n^2)         | O(1)                 | In-place         | Unstable      |
| **Insertion Sort**     | O(n^2)                     | O(n)          | O(n^2)         | O(1)                 | In-place         | Stable        |
| **Shell Sort**         | O(n log n)                 | O(n log² n)   | O(n log² n)    | O(1)                 | In-place         | Unstable      |
| **Merge Sort**         | O(n log n)                 | O(n log n)    | O(n log n)     | O(n)                 | Out-place        | Stable        |
| **Quick Sort**         | O(n log n)                 | O(n log n)    | O(n²)          | O(log n)             | In-place         | Unstable      |
| **Heap Sort**          | O(n log n)                 | O(n log n)    | O(n log n)     | O(1)                 | In-place         | Unstable      |
| **Bucket Sort**        | O(n + k)                   | O(n + k)      | O(n²)          | O(n + k)             | Out-place        | Stable        |
| **Counting Sort**      | O(n + k)                   | O(n + k)      | O(n + k)       | O(k)                 | Out-place        | Stable        |
| **Radix Sort**         | O(n * k)                   | O(n * k)      | O(n * k)       | O(n + k)             | Out-place        | Stable        |

### Notes:
- **In-place**: Sorting is performed without using extra space proportional to the input size.
- **Out-place**: Requires extra space proportional to the input size.
- **Stability**: A stable sorting algorithm preserves the relative order of elements with equal keys.
- **n**: Number of elements in the array.
- **k**: Range of input (used in counting-based algorithms like Counting Sort and Radix Sort).


# 

<Details>
  <summary>
    分析复杂度的一些规则 Rules for Analyzing Complexity
  </summary>

多个时间复杂度相加，如果都是与 n 相关，则取取复杂度高的那一个，例如：O(nlogn + n) = O(nlogn)，O(nlogn + n^2) = O(n^2)。

多个时间复杂度相加，如果其中有些项的复杂度和 n 不相关则不能忽略任何项，例如：O(AlogA + B)，O(AlogA + B^2)

两个循环依次执行，则取复杂度高的那个，嵌套多个循环则需要累乘复杂度。
  
</Details>

1.	Adding Time Complexities Related to ￼:
When adding multiple time complexities that are all related to ￼, the term with the highest growth rate dominates.

Example:
O(n \log n + n) = O(n \log n) 
O(n \log n + n^2) = O(n^2)


2.	Adding Time Complexities with Independent Terms:
If some terms are not related to ￼, they cannot be ignored. The final complexity will include all unrelated terms.

Example:
O(A \log A + B) : Includes both terms because  A  and  B  are independent.
O(A \log A + B^2) : Includes both  A \log A  and  B^2  as separate complexities.

3.	Sequential Loops:
When two loops execute one after another, the overall complexity is determined by the higher of the two.
	•	Example:
```
for (int i = 0; i < n; i++) {  // O(n)
  // some operations
}
for (int j = 0; j < n * n; j++) {  // O(n^2)
  // some operations
}
```

Total complexity =  O(n^2) 

4.	Nested Loops:
When loops are nested, their complexities are multiplied.
	•	Example:
```
for (int i = 0; i < n; i++) {        // O(n)
  for (int j = 0; j < n; j++) {      // O(n)
    for (int k = 0; k < n; k++) {    // O(n)
      // some operations
    }
  }
}
```

Total complexity =  O(n^3) 

Key Takeaways

- Focus on the dominant term when terms depend on ￼.
- Do not ignore unrelated independent terms.
- Multiply complexities for nested loops and compare for sequential loops.
- Always analyze how different variables and loops interact when combining complexities.
