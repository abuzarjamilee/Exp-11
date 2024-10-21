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

``#include<iostream>
using namespace std;

class Cube {
    public:
    float l=3.0;
    float w=5.0;
    float h=7.0;
};

int main() {
    Cube c1;
    float vol=c1.l*c1.w*c1.h;
    cout<<"Volume of cube = "<<vol;
}``
