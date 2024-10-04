LinkedQueueSimulator
Overview

LinkedQueueSimulator is a Python-based project that simulates the fundamental operations of a singly linked queue. This project provides an efficient implementation of common queue operations such as enqueue (insertion) and dequeue (removal) using dynamic memory management. The project is designed to help developers and learners understand the mechanics behind queue data structures, particularly linked queues, which are useful for implementing first-in-first-out (FIFO) logic in various applications.
Features

    Singly Linked Queue Implementation: Uses nodes to store data and manage dynamic memory, allowing flexible queue resizing.
    Enqueue Operation: Adds items to the end (tail) of the queue.
    Dequeue Operation: Removes items from the front (head) of the queue.
    Iterative Queue Traversal: Easily traverse the queue to display current items.
    Dynamic Memory Management: Automatically adjusts to the number of items in the queue without pre-allocated space.

Table of Contents

    Installation
    Usage
    Class Structure
        Node Class
        singly_linked_queue Class
    Example
    Contributing

Installation

To run the LinkedQueueSimulator locally, you need to have Python 3 installed on your machine. Follow these steps to install and run the project:

    Clone this repository:

    bash

git clone https://github.com/yourusername/LinkedQueueSimulator.git

Navigate to the project directory:

bash

cd LinkedQueueSimulator

Run the Python script:

bash

    python Queue.py

Usage

The LinkedQueueSimulator demonstrates basic queue operations. Once you run the script, it will simulate adding and removing elements from the queue and print the results to the console after each operation. The script is designed to be intuitive and educational, showcasing how queues work behind the scenes.
Sample Output

css

Linked Queue Simulator
Enqueue...A
 A
Enqueue...B
 A B
Dequeue...A
 B
...

Class Structure
Node Class

python

class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None

The Node class is the fundamental building block of the singly linked queue. Each node contains:

    data: Stores the value of the node.
    next: A reference to the next node in the queue.

singly_linked_queue Class

python

class singly_linked_queue:
    def __init__(self):
        self.head = None
        self.tail = None
        self.count = 0

The singly_linked_queue class manages the overall structure of the queue, performing essential operations such as:

    enqueue(data): Adds a new item to the queue.
    dequeue(): Removes the first item from the queue.
    print(): Displays the current state of the queue.
    iterate_item(): A generator function to iterate through queue elements.

Example

Here is an example of how to use the singly_linked_queue class in your code:

python

items = singly_linked_queue()

items.enqueue("A")
items.print()

items.enqueue("B")
items.print()

items.dequeue()
items.print()

This will output the following to the console:

css

Enqueue...A
 A
Enqueue...B
 A B
Dequeue...A
 B

Contributing

Contributions are welcome! If you have suggestions, ideas, or bug reports, please feel free to create an issue or submit a pull request. To contribute, follow these steps:

    Fork the repository.
    Create a new branch: git checkout -b feature-branch-name.
    Make your changes and commit them: git commit -m 'Add some feature'.
    Push to the branch: git push origin feature-branch-name.
    Open a pull request.
