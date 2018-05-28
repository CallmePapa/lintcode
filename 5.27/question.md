<h3>题目
给定一个链表，判断它是否有环。
</h3>

<p>样例:
给出 -21->10->4->5, tail connects to node index 1，返回 true

分析:判断是否有环，是指单链表中某个节点的next指针域指向的是链表中在它之前的某一个节点，这样在链表的尾部形成一个环形结构。
最常用的方法：
定义两个指针，同时从链表的头节点出发，
一个指针一次走一步，一个指针一次走两步，
当快的指针追上了走的慢的指针，那么链表就是环形链表;
如果走的快的指针走到了链表的末尾还没追上第一个指针，那么链表就不是环形链表。