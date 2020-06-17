# KarlFreecss.github.io



## 参赛记录

### 华为软件精英挑战赛2020

**成绩** 复赛A榜全国第 11 名

**解题思路**

0. IO优化（最终证明此比赛唯一有意义的地方）

1. 开一个大数组建图，减少cache不命中情况，内存够的情况下每个点的出边占用空间最好是cache line的整数倍;
2. 双向搜索;
3. 构建二级图，也就是根据出发点，下一个点，快速查找到下下个金额合法的点，多线程预处理时，征用写答案的buffer;
4. 对于正向分情况写判断条件，反向也分情况写判断条件.

**代码**: https://github.com/KarlFreecss/huawei_2020_comp/blob/master/final_code_a_test.cpp