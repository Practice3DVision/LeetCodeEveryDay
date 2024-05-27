<h1 align="center">Leetcode Everyday!</h1>

> ***宝剑锋从磨砺出，梅花香自苦寒来！***

-----

### Day 1. 
**1. 感染二叉树需要的总时间** &#10008;  
- 深度优先搜索将二叉树转换为无序图（用于确定一个节点邻近节点的关系）  
- 广度优先搜索计算最长距离  
```c++
std::unordered_map<int, std::vector<int>> table;
  std::function<void(TreeNode*)> dfs = [&](TreeNode* parent) {
      for (auto& child : std::vector<TreeNode*>{parent->left, parent->right})}{
  
          if(child == nullptr)
              continue;
                
          table[parent->val].push_back(child->val);
          table[child->val].push_back(parent->val);

          dfs(child);
      }
  };

  dfs(root);
```
### Day 2.
**1. 总行驶距离** &#10004;  
### Day 3.
**1. 快照数组** &#10004;  
```c++
auto x = std::upper_bound(snaps_[index].begin(), snaps_[index].end(), std::make_pair(snap_id + 1, -1));
return x == snaps_[index].begin() ? 0 : std::prev(x)->second;
```
### Day 4. 
**1. 查询网格图中每一列的宽度** &#10004;
### Day 5. 
**1. 负二进制转换** &#10004;
### Day 6.
**1. 将矩阵按对角线排序** &#10004;
### Day 7.
**1. 满足目标工作时长的员工数目** &#10004;
### Day 8. 
**1. 雇佣 K 位工人的总代价** &#10004;
### Day 9. 
**1. 雇佣 K 名工人的最低成本** &#10004;
### Day 10. 
**1. 去掉最低工资和最高工资后的工资平均值** &#10004;  
```c++
  template<class Input, class T, class BinaryOp>
  T accumulate(Input first, Input last, T init, BinaryOp op);
```
### Day 11.
**1. 规划兼职工作** &#10006;  
```c++
动态规划+二分查找(std::upper_bound)
```
### Day 12. 
**1. 拆炸弹** &#10004;
### Day 13. 
**1. 摘樱桃** &#10004;
#### Day 14. 
**1. 二分查找** &#10004;
### Day 15. 
**1. 移除元素** &#10004;
### Day 16. 
**1. 有序数组的平方** &#10004;
### Day 17. 
**1. 长度最小的子数组** &#10004;
### Day 18. 
**1. 螺旋矩阵II** &#10004;
### Day 19. 
**1. 移除链表元素** &#10004;
### Day 20. 
**1. 设计链表** &#10004;
### Day 21. 
**1. 反转链表** &#10004;
### Day 22. 
**1. 两两交换链表中的节点** &#10004;
### Day 23. 
**1. 删除链表的倒数第 N 个结点** &#10004;  
双指针解决长度未知问题：  
1. 先让快指针走`n`步  
2. 同时让快指针慢指针运动，当快指针走到末尾时，满指针所指位置即为要求的节点
### Day 24. 
**1. 链表相交** &#10004;
#### Day 25.
**1. 环形链表 II** &#10006;
### Day 26. 
**1. 有效的字母异位词** &#10004;
### Day 27. 
**1. 两个数组的交集** &#10004;
### Day 28. 
**1. 快乐数** &#10004;
### Day 29.
**1. 两数之和** &#10004;  
**2. 四数相加 II** &#10004;

### Day 30.
**1. 赎金信** &#10004;  
**2. 三数之和** &#10006;
