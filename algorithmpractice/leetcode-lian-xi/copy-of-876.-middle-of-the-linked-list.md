---
description: Linked List Two Pointers
---

# Copy of 876. Middle of the Linked List

[题目链接](https://leetcode.com/problems/middle-of-the-linked-list/description/)

## 解题思路

````java
```java
class Solution {
    public ListNode middleNode(ListNode head) {
        ListNode slow = head;
        ListNode fast = head;
        while (fast != null && fast.next != null) {
            slow = slow.next;
            fast = fast.next.next;
        }
        return slow;
    }
}
```
````

## 时空复杂度

时间复杂度: O(n)

空间复杂度: O(1)
