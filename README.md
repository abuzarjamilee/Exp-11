# Exp-11

Aim:
To study and implement Classes and Objects

Apparatus:
Vs Code, Github

Theory:
Object Oriented Programming (OOP):
In object-oriented programming data structures, or objects are defined, each with its own properties or attributes. Some concepts of OOPS are:

Classes:
A class is a user-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class. Classes are like blueprints for objects. A class is defined using the class keyword followed by the class name and a block of code that includes its attributes.

For example: A class of car would have common properties like wheels, milage, range. The properties wheels, milage and range are data members of the class. Thier member functions can be applying brakes, increasing speed etc.

Objects:
An object is created from a class. We have already created the class so now we can use this to create objects. Objects are instance of a class holding actual values for the attributes defined by that class.

Global variables:
Global variables are declared outside of function , usually at the top of a program or in a separate file. They are accessible from any part of the program and retain their value throughout the program's lifetime. The scope of this is throughout the entire program

Local variables:
Local variables are declared within a specific block of code, such as a function or loop. They are only accessible within that block and are released from memory when the block exits. Local variables can have the same name as those in other blocks without causing conflicts, as their scope is confined to their respective block. They are typically used for temporary storage or context-specific data.
1) Defining a class:
```
#include<iostream>
using namespace std;

class Cube {
    public:
    float l=3.0;
    float w=5.0;
    float h=7.0;
};
```
output 
![image](https://github.com/user-attachments/assets/380926e5-8da8-45b4-aa85-a877096d6aef)

2)Function inside a class:
```
#include<iostream>
using namespace std;
class cube
{
    public:
    double height=3.0;
    double width=4.0;
    double length=5.0;

    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
}



int main() {
    Cube c1;
    float vol=c1.l*c1.w*c1.h;
    cout<<"Volume of cube = "<<vol;
}
```
output
![image](https://github.com/user-attachments/assets/d5559a5f-c5ae-46d8-b9ba-37c26704c8fa)
3: Public and private variables:
```
#include<iostream>
using namespace std;
class cube
{
    private:
    double height=4.0;
    double width=5.0;
    double length=6.0;

    public:
    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
}
```
output
![image](https://github.com/user-attachments/assets/aa0989f9-3a45-4173-be9c-b31da420d7b8)
4)Display function inside a class:
```
#include<iostream>
using namespace std;
class cube
{
    public:
    double height=5.0;
    double width=6.0;
    double length=7.0;

    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
    void disp_vol(double vol)
    {
        cout<<"volume :"<<vol<<endl;
    }
};
int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
    cube1.disp_vol(v);
}
```
output
![image](https://github.com/user-attachments/assets/8d2f3a74-5baf-4c47-9d75-0dd7fcbeed27)
5)
```
#include<iostream>
using namespace std;
class volume{
    public:
    float height;
    float width;
    float length;
    void input()
    {
        cout<<"enter the value of length: ";
        cin>>length;
        cout<<"enter the value of width: ";
        cin>>width;
        cout<<"enter the value of height: ";
        cin>>height;
    }
    float vol()
    {
        float v=length*width*height;
        return v;
    }
    void display()
    {
        double a=vol();
        cout<<"the volume is :"<<a;
    }
};
int main()
{
    volume volume1;
    volume1.input();
    float a=volume1.vol();
    cout<<a;
}
```
![image](https://github.com/user-attachments/assets/5e2d91ef-f6b9-4e1b-8e1e-e5c81593180d)

Conclusion:
This program helps us understand how classes and objects work in C++. How classes are created and how objects are instantanized. The difference between local and global variables.

