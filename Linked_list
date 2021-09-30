# This is a singly linked list

class Node:
    def __init__(self, data = None):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = Node()
    
    def add(self, data):
        new_node = Node(data)
        cur = self.head
        while cur.next != None:
            cur = cur.next
        cur.next = new_node

    def length(self):
        cur = self.head
        total = 0
        while cur.next != None:
            total += 1
            cur = cur.next
        return total

    def display(self):
        elements = []
        cur_node = self.head
        while cur_node.next != None:
            cur_node = cur_node.next
            elements.append(cur_node.data)
        return elements

    def get(self, index):
        if index >= self.length():
            print("index out of range")
            return None
        else:
            cur = self.head
            idx = 0
            while True:
                cur = cur.next
                if idx == index:
                    return cur.data
                idx += 1

    def erase(self, index):
        if index >= self.length():
            print("index out of range")
            return None
        else:
            cur = self.head
            idx = 0
            while True:
                prev_node = cur
                cur = cur.next
                if idx == index:
                    prev_node.next = cur.next
                    return
                idx += 1
    
    def insert(self, data, index):
        if index >= self.length():
            print("index out of range")
            return None
        else:
            cur = self.head
            idx = 0
            while True:
                cur = cur.next
                if idx == index-1:
                    new_node = Node(data)
                    new_node.next = cur.next
                    cur.next = new_node
                    return 
                idx += 1
   
# End                
