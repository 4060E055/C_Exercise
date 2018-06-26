
# Object Oriented Programming 物件導向程式設計(OOP)
```
針對大型軟體設計提出，目的是使軟體設計更加靈活、改良與支援程式碼和設計的重用性，程式碼具有更好的可讀性和可擴展性，以及大幅降低軟體發展的難度等。
物件導向程式設計特色:封裝(Encapsulation)+繼承(Inheritance)+多型(Polymorphism)
物件導向程式設計特色:封裝
將資料以及相關的操作封裝在一起， 以便組成一個相互依存、不可分割的整體(即類別class與物件object)， 不同物件之間透過訊息機制來通訊或者同步。
針對相同類型的物件(instance)進行分頭、抽象，得出共同的特體而形成類別(class)
物件導向程式設計的關鍵， 就是如何合理地定義類別(class) ，並且祖捕多個類別(class) 之間的關 系。
```

物件導向程式設計特色:封裝(Encapsulation)+繼承(Inheritance)+多型(Polymorphism)

# 類別class與物件object

定義class類別:Circle
>* 成員方法(method)[又稱動作(actions)]:定義物件的行為(behavior)。可以在物件上呼叫方法，就等同在物件執行某個動作
>* 一個圓形物件可呼叫getArea() 來取得面積，呼叫getPerimeter() 來取得周長。
>* 所有的方法(包括建構子)都有定義的第一個參數是self ，self參數是自動設定參考到剛被建立的物件來呼叫實例方法(instance methods) 。

# 資料隱藏(data hiding)
```
為了防止直接修改資料項目，有一方法就是不要讓客戶端直接存取資料項目。
可經由定義私有資料項目(private data fields)來完成。
```

# 繼承(inheritance):父類別與子類別   

類別與類別之間的關係 
>* 關連(association):是一般的二元關係，用來描述兩類別之間的活動。 學生----課程------老師
>* 聚合(aggregation):關連的特殊格式，用以表示兩物件之間所有權的關係。聚合的關係通常以聚合類別的資料成員來表示    Name---student ---Address
>* 合成(composition):一個物件可能被許多聚合物件所擁有，如果一個物件只被一個聚合物件獨家擁有，則它們的關係就是合成(composition)
>* 繼承(inheritance)


子類別繼承父類別:
>* 子類別就自動擁有父類別的變數與函式。
>* 子類別==衍生類別(derived class)或子類別(child class)
>* 父類別==基礎類別(base class)或雙親類別(parent class)

### 方法覆寫(method overriding)

>* 子類別繼承從父類別的方法，有時可能會在子類別修改其繼承的父類別方法中的內容

# 範例: 完成底下的範例

父類別GeometricObject.cpp
```
#include "GeometricObject.h"

________::GeometricObject()
{
  color = "white";
  filled = false;
}

________::GeometricObject(const string& color, bool filled)
{
  this->color = ________;
  ________->filled = filled;
}

________ GeometricObject::getColor() const
{
  return ________;
}

________ GeometricObject::setColor(const string& color)
{
  ________ = color;
}

________ GeometricObject::isFilled() const
{
  return ________;
}

________ GeometricObject::setFilled(bool filled)
{
  ________ = filled;
}

________ ________::toString() const
{
  return "Geometric Object";
}
```

### 作業:寫下GeometricObject.h

子類別:DerivedRectangle  繼承 父類別:GeometricObject

```
#include "DerivedRectangle.h"

// Construct a default rectangle object
Rectangle::Rectangle()
{
  width = 1;
  height = 1;
}

// Construct a rectangle object with specified width and height
Rectangle::Rectangle(double width, double height)
{
  setWidth(________);
  setHeight(________);
}

Rectangle::Rectangle(double width, double height, const string& color, bool filled)
{
  setWidth(________);
  setHeight(________);
  setColor(________);
  setFilled(________);
}

// Return the width of this rectangle
double Rectangle::getWidth() const
{
  return ________;
}

// Set a new radius
void Rectangle::setWidth(double width)
{
  this->width = ________;
}

// Return the height of this rectangle
double Rectangle::getHeight() const
{
  return________;
}

// Set a new height
void Rectangle::setHeight(double height)
{
  this->height = ________;
}

// Return the area of this rectangle
double Rectangle::getArea() const
{
  return ________;
}

// Return the perimeter of this rectangle
double Rectangle::getPerimeter() const
{
  return ________;
}

// Redefine the toString function, to be covered in Section 15.5
string Rectangle::toString() const
{
  return "Rectangle object";
}
```

### 作業:寫下DerivedRectangle.h

```
#ifndef RECTANGLE_H
#define RECTANGLE_H
#________ "GeometricObject.h"

________ Rectangle: ________ GeometricObject
{
________:
  Rectangle();
  Rectangle(_______,_________);
  Rectangle(_______,_________,_________,_____);
  double _________ const;
  void _________;
  double _________ const;
  void _________(double);
  double _________const;
  double _________ const;
  string toString() const;

 _________:
  _________ width;
  _________ height;
};  // Must place semicolon here

#endif
```


==>子類別:Circle  繼承 父類別:GeometricObject

```
#include "DerivedCircle.h"

// Construct a default circle object
________::Circle()
{
  radius = 1;
}

// Construct a circle object with specified radius
Circle::Circle(double radius)
{
  setRadius(________);
}

// Construct a circle object with specified radius,
//  color and filled values
Circle::Circle(double radius, const string& color, bool filled)
{
  ________ = radius;
  setColor(color);
  setFilled(filled);
}

// Return the radius of this circle
double Circle::getRadius() const
{
  return ________;
}

// Set a new radius
void Circle::setRadius(double radius)
{
  this->radius = ________;
}

// Return the area of this circle
double Circle::getArea() const
{
  return ________ * 3.14159;
}

// Return the perimeter of this circle
double Circle::getPerimeter() const
{
  return ________ * 3.14159;
}

// Return the diameter of this circle
double Circle::getDiameter() const
{
  return ________;
}

// Redefine the toString function
string ________::toString() const
{
  return "Circle object";
}
```

### 作業:寫下DerivedCircle.h

主測試程式:TestGeometricObject.cpp
```
#________ "GeometricObject.h"
#________ "DerivedCircle.h"
#________ "DerivedRectangle.h"
#________ <iostream>

________ namespace std;

________ main()
{
//建立一個GeometricObject物件顏色(color)為red,有填
  GeometricObject shape;
  shape.setColor("________");
  shape.setFilled(________);
  cout << shape.toString() << endl
    << " color: " << shape.________
    << " filled: " << (shape.________? "true" : "false") << endl; 

//建立一個Circle物件半徑為11,顏色為black,沒填
  ________ circle(________);
  circle.setColor(________);
  circle.setFilled(________);
  cout << circle.toString()<< endl
    << " color: " << circle.________
    << " filled: " << (circle.________ ? "true" : "false") 
    << " radius: " << circle.________
    << " area: " << circle.________
    << " perimeter: " << circle.getPerimeter() << endl;

//建立一個Rectangle物件,顏色為orange,有填
  ________ rectangle(2, 3);
  rectangle.setColor("________");
  rectangle.setFilled(________);
  cout << rectangle.toString()<< endl
    << " color: " << circle.________
    << " filled: " << (circle.________ ? "true" : "false") 
    << " width: " << rectangle.________
    << " height: " << rectangle.________
    << " area: " << rectangle.________
    << " perimeter: " << rectangle.________ << endl;

  return 0;
}
```
### 作業:完成上述範例的UML類別圖

# 建構函式鏈(constructor chaining)與解構函式鏈(destructor chaining)

當建立子類別的物件時，子類別執行其自己的工作前，將呼叫父類別的建構函式。若父類別又繼承自其他類別，父類別建構函式在執行其工作前，將呼其父類別的建構函式，此過程將繼續進行到繼承鏈的最後一個建構函式。這稱之為建構函式鏈(constructor chaining)。

相反的，解構函式以相反的順序執之。當子類別物件被刪除時，子類別的解構函式將呼叫。當其工作執行完後，再呼叫其父類別的解構函式。此過程一直持續到繼承鏈的最後一個解構函式被呼叫。這稱之為解構函式鏈(destructor chaining)。

```
#include <iostream>
using namespace std;

class Person
{
public:
  Person()
  {
    cout << "Performs tasks for Person's constructor" << endl;
  }

  ~Person()
  {
    cout << "Performs tasks for Person's destructor" << endl;
  }
};

class Employee: public Person
{
public:
  Employee()
  {
    cout << "Performs tasks for Employee's constructor" << endl;
  }

  ~Employee()
  {
    cout << "Performs tasks for Employee's destructor" << endl;
  }
};

class Faculty: public Employee
{
public:
  Faculty()
  {
    cout << "Performs tasks for Faculty's constructor" << endl;
  }

  ~Faculty()
  {
    cout << "Performs tasks for Faculty's destructor" << endl;
  }
};

int main()
{
  Faculty faculty;

  return 0;
}
```

# 多型(Polymorphism):父型態的變數可以被子型態物件來使用。
```

```

# Virtual 函式

>* 假使一函式在父類別被定義為 virtual，則所有在子類別相同的函式皆自動設為 virtual。

為了能使函式動態的連結，您需要做兩件事情：
>* 在父類別中函式必須定義為 virtual。
>* 在 virtual 函式，參考物件的變數必須以reference或pointer的方式傳送。

### 靜態繫結(static binding) vs 動態繫結(dynamic binding)


靜態繫結(static binding)==?變數的宣告型態(declare type)在編譯時期(compile time)決定使用哪個函式

動態繫結(dynamic binding)==>編譯器依據參數型態、參數個數與參數順序尋找適當匹配的函式。一個 virtual 函式可以實作於多個子類別中，C++ 會依據變數所參考的物件類別之真實型態，在執行期間(run time)動態連結實作函式。此稱為。

### 多型的型態(polymorphic type) 


# protected 關鍵字

>* 允許子類別來存取定義在父類別中的資料項目或函式
>* 不允許非子類別存取這些資料項目與函式

```
#include <iostream>
using namespace std;

class B
{
public:
  int i;

protected:
  int j;

private:
  int k;
};

class A: public B
{
public:
  void display() const
  {
    cout << i << endl; // Fine, can access it
    cout << j << endl; // Fine, can access it
    cout << k << endl; // Wrong, cannot access it
  }
};

int main()
{
  A a;
  cout << a.i << endl; // Fine, can access it
  cout << a.j << endl; // Wrong, cannot access it
  cout << a.k << endl; // Wrong, cannot access it

  return 0;
}
```

# 抽象類別(abstract class)與抽象函式(abstract function) 




# 向上轉型(upcasting)與向下轉型 (downcasting) 




