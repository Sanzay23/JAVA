DEADLINE : 16/12/21

#WAP TO IMPLEMENT STACK USING ARRAY IN JAVA


class Stack {
    static final int SIZE = 10;
    int top;
    int a[] = new int[SIZE]; 
 
    boolean isEmpty()
    {
        return (top < 0);
    }
    Stack()
    {
        top = -1;
    }
 
    boolean push(int x)
    {
        if (top >= (SIZE - 1)) {
            System.out.println("Already Full");
            return false;
        }
        else {
            a[++top] = x;
            System.out.println(x + " is sucessfully added");
            return true;
        }
    }
 
    int pop()
    {
        if (top < 0) {
            System.out.println("It is empty ");
            return 0;
        }
        else {
            int x = a[top--];
            return x;
        }
    }
 
    int peek()
    {
        if (top < 0) {
            System.out.println("It is empty");
            return 0;
        }
        else {
            int x = a[top];
            return x;
        }
    }
    
    void print(){
    for(int i = top;i>-1;i--){
      System.out.print(" "+ a[i]);
    }
  }
}
 
// Driver code
class Main {
    public static void main(String args[])
    {
        Stack s = new Stack();
        s.push(10);
        s.push(20);
        s.push(30);
        System.out.println(s.pop() + " Popped from stack");
        System.out.println("Top element is :" + s.peek());
        System.out.print("Elements present in stack :");
        s.print();
    }
}
