``` java

class Animal{
    String name;
    String food;
    Animal(){ //Default Constructor
    name = "Tiger"; 
}
    Animal(String food){
    //parameterized constroctor
        this.food = food;
    }
    
}
class Constructors{
    public static void main(String arg[]){
        Animal Tiger = new Animal("meat");
        System.out.println("Domestic animal we are talking about is" + Tiger.name);
        System.out.println("Tiger eats " + Tiger.food );
    }
}
```
