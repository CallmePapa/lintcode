<h3>给定一个链表，如果链表中存在环，则返回到链表中环的起始节点的值，
<br/>如果没有环，返回null。</h3>


<h3>样例
<p>给出 -21->10->4->5, tail connects to node index 1，返回10

<h4>分析
上一题的进阶。
首先，利用快慢指针判断有无环，若遇到slow == fast时，跳出循环；
然后，调整fast=head，slow不变，此时slow与fast同步移动，
直至再次相遇，即是链表中环的起始节点。
