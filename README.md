class Queue:
    def __init__(self):
        self.qList = []
    def isEmpty(self):
        return not self.qList
    def __len__(self):
        return len(self.qList)     
    def enqueue(self, item):
        self.qList.append(item)
        print(f"Inserted element = {item}")
    def dequeue(self):
        if not self.isEmpty():
            print(f"Deleted element = {self.qList.pop(0)}")
        else:
            print("Cannot delete from an empty queue.")
    def display(self):
        print(self.qList)

# Dynamic input for enqueue operations
q = Queue()
for i in [10, 20, 30, 40, 50, 60, 70, 80]:
    q.enqueue(i)
q.display()
# Dequeue operations
for _ in range(9)
    q.dequeue()
