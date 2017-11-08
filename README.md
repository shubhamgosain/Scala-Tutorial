# Scala-Tutorial-
Scala is a better alternative to java . It was made specially to deal with collections and generics and is very easy to implement difficult java tasks.   Here following my proceedure you will be able to learn scala easily




scala> 1+2
res1: Int = 3

scala> 2/3
res2: Int = 0

scala> 2/3.000
res3: Double = 0.6666666666666666

scala> c=10
<console>:11: error: not found: value c
       c=10
       ^
<console>:12: error: not found: value c
       val $ires8 = c


scala> var a=10
a: Int = 10


scala> println(a)
10

scala> a=20
a: Int = 20

scala> println(a)
20

scala> val b=10
b: Int = 10

scala> println(b)
10

scala> b=20
<console>:12: error: reassignment to val
       b=20
        ^

scala> val b=20
b: Int = 20




Here both var and val can be used to create a variable 
var is mutable while val is immutable variabels i.e.. value of var type variable can be changed while val cannot be changed

A good practice is to use val for security because no outsider can temper the variable value

val b=10
val b=20                        //here where are destroying first b and creating a new fresh variable




scala> val char='x'
char: Char = x

scala> val charss="xxx"
charss: String = xxx

scala> charss="zzz"
<console>:12: error: reassignment to val
       charss="zzz"
             ^


----To DEfine datatype---


scala> val a:Int=10
a: Int = 10

No need to use this because it is pointless when scala can identify datatype of its own datatype

scala> val a=10
a: Int = 10




------------------Create class in java-----------

1. case class
It creates a class with all getters and setters with other helper method to ease the user

scala>case class Test(var i: Int, var j: String)
defined class HW


scala> :javap -p Test
Compiled from "<console>"
public class Test implements scala.Product,scala.Serializable {
  private int i;
  private java.lang.String j;
  public int i();
  public void i_$eq(int);
  public java.lang.String j();
  public void j_$eq(java.lang.String);
  public Test copy(int, java.lang.String);
  public int copy$default$1();
  public java.lang.String copy$default$2();
  public java.lang.String productPrefix();
  public int productArity();
  public java.lang.Object productElement(int);
  public scala.collection.Iterator<java.lang.Object> productIterator();
  public boolean canEqual(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public Test(int, java.lang.String);
}




Here public int i() and public int j() are setters while i_$eq are getters


2. Regular class- Helper functions are not created


scala>  class c (val i: Int)
defined class c

scala> :javap -p c
Compiled from "<console>"
public class c {
  private final int i;
  public int i();
  public c(int);
}



---------------If else in scala------------




val a=10;



if(a==10) 
print("true") 
else 
print("false")


or in terneray


if(a==10) print("true") else print("false")



-------------


scala> val rand:Double=math.random*100
rand: Double = 67.93665818570148


scala> val greaterThanFive:Boolean={if(rand>=5)true else false}
greaterThanFive: Boolean = true

scala> val isBlue={if(greaterThanFive) "blue" else "red"}
isBlue: String = blue

scala> print(isBlue)
blue

--------------------------

