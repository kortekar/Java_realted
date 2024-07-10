# Below code is example to implement Stack from array 
```
class Stack {
    int top;
    int maxSize;
    int[] stack;

    public Stack(int size) {
        this.maxSize = size;
        this.top = -1;
        this.stack = new int[size];
    }
```
```

    public boolean isEmpty() {
        return top == -1;
    }
```
```
    public boolean isFull() {
        return top == maxSize - 1;
    }
```
```
    public void push(int value) {
        if (isFull()) {
            System.out.println("Can't push, stack is full");
        } else {
            stack[++top] = value;
        }
    }
```
```
    public int pop() throws Exception {
        if (isEmpty() || top < 0) {
            throw new Exception("Stack is empty!!!");
        } else {
            return stack[top--];
        }
    }
```
```
    public int peek() throws Exception {
        if (isEmpty()) {
            throw new Exception("Can't peek, stack is empty");
        }
        return stack[top];
    }
```
```
    public static void main(String[] args) {
        Stack stack = new Stack(5);
        stack.push(5);
        stack.push(3);
        try {
            System.out.println(stack.peek()); 
            System.out.println(stack.pop());  
            System.out.println(stack.pop());  
            System.out.println(stack.pop());  
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }
}

```
