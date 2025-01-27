# Compile-Time-Polymorphism
package main;
public class Main {
     public int addition(int x, int y) {
    return x + y;
  }
     public int addition(int x, int y, int z) {
    return x + y + z;
  }
      public double addition(double x, double y) {
    return x + y;
  }
public static void main(String[] args) {
    Main number = new Main();
    
     int res1 = number.addition(444, 555);
    System.out.println("Addition of Two integers:"+res1);
     int res2 = number.addition(333, 444, 555);
    System.out.println("Addition of Three integers:"+res2);
     double res3 = number.addition(10.15, 20.22);
    System.out.println("Addition of Two doubles:"+res3);
  }
}

Output:
Addition of Two integers:999
Addition of Three integers:1332
Addition of Two doubles:30.369999999999997
