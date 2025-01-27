# 33.Runtime-Polymorphism-
coding:
class Vehicle {
    
    public void sound() {
        System.out.println(“Vehicle make sounds");
    }
}

class TwoWheeler extends Vehicle{
        @Override
    public void sound() {
        System.out.println("TwoWheeler make sounds");
    }
}

class ThreeWheeler extends Vehicle{
    @Override
    public void sound() {
        System.out.println("ThreeWheelers make sounds");

    }
}

public class RunTimePolymorphism {
    public static void main(String[] args) {
        
 Vehicle v1 = new TwoWheeler();                       Vehicle v2 = new ThreeWheeler();                 
                v1.sound();     
                v2.sound();    
 }
}
Output:
   TwoWheelers make sound
   ThreeWheeler make sound 
