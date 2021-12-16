DEADLINE DATE : 16/12/21   

WAP TO DEMONSTRATE THE USE OF THE DEFAULT METHOD IN INTERFACE


interface Example{

    default void display()
    {
        System.out.println("Hello from Default Method");
    }
}

 
class Interface implements Example{
 
    public static void main(String args[])
    {
        Interface i1 = new Interface();
        i1.display();
    }
}
