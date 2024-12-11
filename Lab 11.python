print ("Michael Mordec, 7/12/22, Lab 11, CSC 242:")

class Node :

    # singly linked node
    def __init__(self, data = None) :
        self.data = data
        self.next = None

class singly_linked_queue :

    def __init__(self) :
        # create an empty list
        self.head = None
        self.tail = None
        self.count = 0
    def iterate_item(self) :
        # iterate through the list
        current_item = self.head
        while current_item :
            val = current_item.data
            current_item = current_item.next
            yield val
    def enqueue(self, data) :
        print("Enqueue..." + data)
        # append items on the list
        node = Node(data)
        if self.tail :
            self.tail.next = node
            self.tail = node
        else :
            self.head = node
            self.tail = node
        self.count += 1

    def dequeue(self) :
        if self.count < 1:
            print("Dequeue...Nothing!")
            return
        print("Dequeue..."+self.head.data)
        self.head = self.head.next
        self.count -= 1

    def print(self):
        if self.count < 1:
            print(" (Empty)")
            return
        s = ""
        for val in self.iterate_item() :
            s = s + " " + val
        print(s)
    
items = singly_linked_queue()

print("Linked Queue Simulator")

items.enqueue("A")
items.print()

items.enqueue("B")
items.print()

items.dequeue()
items.print()

items.enqueue("C")
items.print()

items.enqueue("D")
items.print()

items.enqueue("E")
items.print()

items.dequeue()
items.print()
  
items.dequeue()
items.print()

items.dequeue()
items.print()

items.dequeue()
items.print()

items.dequeue()
items.print()

