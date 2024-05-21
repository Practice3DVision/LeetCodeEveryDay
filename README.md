<h1 align="center">Leetcode Everyday!</h1>

> ***宝剑锋从磨砺出，梅花香自苦寒来！***

-----

#### Day 1. 感染二叉树需要的总时间  
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
#### Day 2. 总行驶距离
#### Day 3. 快照数组
```c++
auto x = std::upper_bound(snaps_[index].begin(), snaps_[index].end(), std::make_pair(snap_id + 1, -1));
return x == snaps_[index].begin() ? 0 : std::prev(x)->second;
```
#### Day 4. 查询网格图中每一列的宽度
#### Day 5. 负二进制转换
#### Day 6. 将矩阵按对角线排序
#### Day 7. 满足目标工作时长的员工数目
#### Day 8. 雇佣 K 位工人的总代价
#### Day 9. 雇佣 K 名工人的最低成本
#### Day 10. 去掉最低工资和最高工资后的工资平均值
```c++
  template<class Input, class T, class BinaryOp>
  T accumulate(Input first, Input last, T init, BinaryOp op);
```
#### Day 11. 规划兼职工作
```c++
动态规划+二分查找(std::upper_bound)
```
#### Day 12. 拆炸弹
#### Day 13. 摘樱桃
#### Day 14. 二分查找
#### Day 15. 移除元素
#### Day 16. 有序数组的平方
#### Day 17. 长度最小的子数组
#### Day 18. 螺旋矩阵II
#### Day 19. 移除链表元素
#### Day 20. 设计链表
#### Day 21. 反转链表
#### Day 22. 两两交换链表中的节点
#### Day 23. 删除链表的倒数第 N 个结点
双指针解决长度未知问题：
1. 先让快指针走`n`步
2. 同时让快指针慢指针运动，当快指针走到末尾时，满指针所指位置即为要求的节点
#### Day 24. 链表相交
#### Day 25. 环形链表 II
#### Day 26. 有效的字母异位词
#### Day 27. 两个数组的交集