# Creating-a-LinkedList-
#Creating an empty linkedlist and inserting an element at the end
class Node:
    def __init__(self, value):
        self.value = value
        self.next = None
        
        
class LinkedList:
    def __init__(self):
        self.head = None
        self.tail = None
        self.length = 0
        
        
    def append(self, value):
        new_node = Node(value)
        if self.head is None:
            self.head = new_node
            self.tail = new_node
        else:
            self.tail.next = new_node
            self.tail = new_node
        self.length += 1
        
        
new_linked_list = LinkedList()
new_linked_list.append(11)
new_linked_list.append(22)
print(new_linked_list)
        
        
