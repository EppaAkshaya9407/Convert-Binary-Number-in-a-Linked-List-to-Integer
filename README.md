# Convert-Binary-Number-in-a-Linked-List-to-Integer
# Definition for singly-linked list.
# class ListNode:
#     def __init__(self, val=0, next=None):
#         self.val = val
#         self.next = next
class Solution:
    def getDecimalValue(self, head: ListNode | None) -> int:
        if head is None:
            return None
        a=[]
        temp=head
        while temp:
            a.append(temp.val)
            temp=temp.next
        n=len(a)
        r=0
        for i in a:
            r=r*2+i
        return r
