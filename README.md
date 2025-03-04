# Start-CPP
# BEGINEER TRACK FOR C++_FINAL

*BEGINEER TRACK FOR C++ (with project)*

- *INSTALLATION OF IDE AND COMPILER (VS code)*

*[https://youtu.be/0yn7irrHzM8](https://youtu.be/0yn7irrHzM8) (follow this link)*

## LEVEL 1:C++ Program Structure

> Let us look at a simple code that would print the words Hello World.


```
#include <iostream>
using namespace std;
// main() is where program execution begins.
int main() {
cout << "Hello World"; // prints Hello World
return 0;
}
```
  

> Let us look at the various parts of the above program −
> 
- The C++ language defines several headers, which contain information that is either necessary or useful to your program. For this program, the header **<iostream>** is needed.
- The line **using namespace std;** tells the compiler to use the std namespace. Namespaces are a relatively recent addition to C++.
- The next line '**// main() is where program execution begins.**' is a single-line comment available in C++. Single-line comments begin with // and stop at the end of the line.
- The line **int main()** is the main function where program execution begins.
- The next line **cout << "Hello World";** causes the message "Hello World" to be displayed on the screen.
- The next line **return 0;** terminates main( )function and causes it to return the value 0 to the calling process.

TASK 1: Print Hello! Google Developers Club.

(attach .cpp file &make pull request)

# LEVEL 2: DATA TYPES

> While writing program in any language, you need to use various variables to store various information. Variables are nothing but reserved memory locations to store values. This means that when you create a variable you reserve some space in memory.You may like to store information of various data types like character, wide character, integer, floating point, double floating point, boolean etc. Based on the data type of a variable, the operating system allocates memory and decides what can be stored in the reserved memory.
> 

## Primitive Built-in Types

> C++ offers the programmer a rich assortment of built-in as well as user defined data types. Following table lists down seven basic C++ data types −
![image](https://user-images.githubusercontent.com/81976330/135765556-50d91a45-091a-44e7-a27f-6047a548a9a2.png)



> Several of the basic types can be modified using one or more of these type modifiers −
> 
- signed
- unsigned
- short
- long

> The following table shows the variable type, how much memory it takes to store the value in memory, and what is maximum and minimum value which can be stored in such type of variables.
> 

![image](https://user-images.githubusercontent.com/81976330/135765730-207aaee6-387f-4d41-8c32-75ab8048fe8c.png)



TASK 2: Write a program to print correct memory size of any 5 data types(hint: use .size() function.)

(attach .cpp file and make a pull request)

LEVEL 3: CONDITIONALS AND LOOPS:

> Decision making structures require that the programmer specify one or more conditions to be evaluated or tested by the program, along with a statement or statements to be executed if the condition is determined to be true, and optionally, other statements to be executed if the condition is determined to be false.Following is the general form of a typical decision making structure found in most of the programming languages −
> 

![image](https://user-images.githubusercontent.com/81976330/135765791-5e845731-abfa-4017-9ce9-d9df99402d44.png)

> C++ programming language provides following types of decision making statements.
> 

![image](https://user-images.githubusercontent.com/81976330/135765900-593650d6-5f8c-4348-85c1-323cadf23e6a.png)


> −LOOPS:There may be a situation, when you need to execute a block of code several number of times. In general, statements are executed sequentially: The first statement in a function is executed first, followed by the second, and so on.Programming languages provide various control structures that allow for more complicated execution paths.A loop statement allows us to execute a statement or group of statements multiple times and following is the general from of a loop statement in most of the programming languages −
> 




> C++ programming language provides the following type of loops to handle looping requirements.
> 
![image](https://user-images.githubusercontent.com/81976330/135765940-40d066e3-afa4-4854-8405-8589f37dfb91.png)


For syntax go through: [https://www.w3schools.com/cpp/cpp_for_loop.asp](https://www.w3schools.com/cpp/cpp_for_loop.asp)

TASK 3: PRINT A ISOCALES TRIANGLE USING STARS “*”

(attach .cpp file and make a pull request)

LEVEL 4: FUNCTIONS AND POINTERS:

> A function is a group of statements that together perform a task. Every C++ program has at least one function, which is main(), and all the most trivial programs can define additional functions.You can divide up your code into separate functions. How you divide up your code among different functions is up to you, but logically the division usually is such that each function performs a specific task.A function declaration tells the compiler about a function's name, return type, and parameters. A function definition provides the actual body of the function.The C++ standard library provides numerous built-in functions that your program can call. For example, function strcat() to concatenate two strings, function memcpy() to copy one memory location to another location and many more functions.A function is known with various names like a method or a sub-routine or a procedure etc.
> 

## Defining a Function

> The general form of a C++ function definition is as follows −
> 

```
  return_type function_name( parameter list ) {

body of the function

}
  ```

> A C++ function definition consists of a function header and a function body. Here are all the parts of a function −
> 
- **Return Type** − A function may return a value. The **return_type** is the data type of the value the function returns. Some functions perform the desired operations without returning a value. In this case, the return_type is the keyword **void**.
- **Function Name** − This is the actual name of the function. The function name and the parameter list together constitute the function signature.
- **Parameters** − A parameter is like a placeholder. When a function is invoked, you pass a value to the parameter. This value is referred to as actual parameter or argument. The parameter list refers to the type, order, and number of the parameters of a function. Parameters are optional; that is, a function may contain no parameters.
- **Function Body** − The function body contains a collection of statements that define what the function does.

POINTERS:

> C++ pointers are easy and fun to learn. Some C++ tasks are performed more easily with pointers, and other C++ tasks, such as dynamic memory allocation, cannot be performed without them.As you know every variable is a memory location and every memory location has its address defined which can be accessed using ampersand (&) operator which denotes an address in memory. Consider the following which will print the address of the variables defined −
> 

```
#include <iostream>

using namespace std;

int main () {

int var1;

char var2[10];

cout << "Address of var1 variable: ";

cout << &var1 << endl;

cout << "Address of var2 variable: ";

cout << &var2 << endl;

return 0;

}
```
> When the above code is compiled and executed, it produces the following result −
> 

Address of var1 variable: 0xbfebd5c0

Address of var2 variable: 0xbfebd5b6

## What are Pointers?

> A pointer is a variable whose value is the address of another variable. Like any variable or constant, you must declare a pointer before you can work with it. The general form of a pointer variable declaration is −
> 

type *var-name;

> Here, type is the pointer's base type; it must be a valid C++ type and var-name is the name of the pointer variable. The asterisk you used to declare a pointer is the same asterisk that you use for multiplication. However, in this statement the asterisk is being used to designate a variable as a pointer. Following are the valid pointer declaration −
> 

int *ip; // pointer to an integer

double *dp; // pointer to a double

float *fp; // pointer to a float

char *ch // pointer to character

TASK 4: MAKE A FUNCTION WHICH RETURNS SUM UPTO N NUMBERS:

(attach .cpp file and make a pull request)

LEVEL 4: CLASSES &OBJECTS :

> The main purpose of C++ programming is to add object orientation to the C programming language and classes are the central feature of C++ that supports object-oriented programming and are often called user-defined types.A class is used to specify the form of an object and it combines data representation and methods for manipulating that data into one neat package. The data and functions within a class are called members of the class.
> 

## C++ Class Definitions

> When you define a class, you define a blueprint for a data type. This doesn't actually define any data, but it does define what the class name means, that is, what an object of the class will consist of and what operations can be performed on such an object.A class definition starts with the keyword class followed by the class name; and the class body, enclosed by a pair of curly braces. A class definition must be followed either by a semicolon or a list of declarations. For example, we defined the Box data type using the keyword class as follows −
> 
```
class Box {

public:

double length; // Length of a box

double breadth; // Breadth of a box

double height; // Height of a box

};
  ```

> The keyword public determines the access attributes of the members of the class that follows it. A public member can be accessed from outside the class anywhere within the scope of the class object. You can also specify the members of a class as private or protected which we will discuss in a sub-section.
> 

## Define C++ Objects

> A class provides the blueprints for objects, so basically an object is created from a class. We declare objects of a class with exactly the same sort of declaration that we declare variables of basic types. Following statements declare two objects of class Box −
> 
```
Box Box1; // Declare Box1 of type Box

Box Box2; // Declare Box2 of type Box
 ```

> Both of the objects Box1 and Box2 will have their own copy of data members.
> 

## Accessing the Data Members

> The public data members of objects of a class can be accessed using the direct member access operator (.). Let us try the following example to make the things clear −
> 

```

#include <iostream>

using namespace std;

class Box {

public:

double length; // Length of a box

double breadth; // Breadth of a box

double height; // Height of a box

};

int main() {

Box Box1; // Declare Box1 of type Box

Box Box2; // Declare Box2 of type Box

double volume = 0.0; // Store the volume of a box here

// box 1 specification

Box1.height = 5.0;

Box1.length = 6.0;

Box1.breadth = 7.0;

// box 2 specification

Box2.height = 10.0;

Box2.length = 12.0;

Box2.breadth = 13.0;

// volume of box 1

volume = Box1.height * Box1.length * Box1.breadth;

cout << "Volume of Box1 : " << volume <<endl;

// volume of box 2

volume = Box2.height * Box2.length * Box2.breadth;

cout << "Volume of Box2 : " << volume <<endl;

return 0;

}
  ```

> When the above code is compiled and executed, it produces the following result −
> 

Volume of Box1 : 210

Volume of Box2 : 1560

> It is important to note that private and protected members can not be accessed directly using direct member access operator (.). We will learn how private and protected members can be accessed.
> 

## Classes and Objects in Detail

> So far, you have got very basic idea about C++ Classes and Objects. There are further interesting concepts related to C++ Classes and Objects which we will discuss in various sub-sections listed below −
> 

	Concept & Description
1  	Class Member Functions:A member function of a class is a function that has its definition or its prototype within the class definition like any other variable.
	
2	Class Access Modifiers:A class member can be defined as public, private or protected. By default members would be assumed as private.
	
3	Constructor & Destructor:A class constructor is a special function in a class that is called when a new object of the class is created. A destructor is also a special function which is called when created object is deleted.
4	Copy Constructor:The copy constructor is a constructor which creates an object by initializing it with an object of the same class, which has been created previously.
	
5	Friend Functions:A friend function is permitted full access to private and protected members of a class.
	
6	Inline Functions:With an inline function, the compiler tries to expand the code in the body of the function in place of a call to the function.
	
7	this Pointer:Every object has a special pointer this which points to the object itself.
	
8	Pointer to C++ Classes:A pointer to a class is done exactly the same way a pointer to a structure is. In fact a class is really just a structure with functions in it.
	
9	Static Members of a Class:Both data members and function members of a class can be declared as static.


More resources on : [https://www.tutorialspoint.com/cplusplus/cpp_inheritance.htm](https://www.tutorialspoint.com/cplusplus/cpp_inheritance.htm)

TASK 5: MAKE A CLASS WHICH RETURNS THE STDENT DATA:WHICH INCLUDES NAME,CLASS,ROLL NO. ,E-MAIL.

(attach .cpp file and make a pull request)

LEVEL 6: FILE HANDELING

> So far, we have been using the iostream standard library, which provides cin and cout methods for reading from standard input and writing to standard output respectively.This tutorial will teach you how to read and write from a file. This requires another standard C++ library called fstream, which defines three new data types −
> 

![image](https://user-images.githubusercontent.com/81976330/135795452-1f594adf-3a70-48b5-a7aa-de4d95952558.png)


> To perform file processing in C++, header files <iostream> and <fstream> must be included in your C++ source file.
> 

## Opening a File

> A file must be opened before you can read from it or write to it. Either ofstream or fstream object may be used to open a file for writing. And ifstream object is used to open a file for reading purpose only.Following is the standard syntax for open() function, which is a member of fstream, ifstream, and ofstream objects.
> 

void open(const char *filename, ios::openmode mode);

> Here, the first argument specifies the name and location of the file to be opened and the second argument of the open() member function defines the mode in which the file should be opened.
> 

![image](https://user-images.githubusercontent.com/81976330/135795513-9cc91df2-daa2-422f-b7cc-85db3e860f04.png)


> You can combine two or more of these values by ORing them together. For example if you want to open a file in write mode and want to truncate it in case that already exists, following will be the syntax −
> 

ofstream outfile;

outfile.open("file.dat", ios::out | ios::trunc );

> Similar way, you can open a file for reading and writing purpose as follows −
> 

fstream afile;

afile.open("file.dat", ios::out | ios::in );

## Closing a File

> When a C++ program terminates it automatically flushes all the streams, release all the allocated memory and close all the opened files. But it is always a good practice that a programmer should close all the opened files before program termination.Following is the standard syntax for close() function, which is a member of fstream, ifstream, and ofstream objects.
> 

void close();

## Writing to a File

> While doing C++ programming, you write information to a file from your program using the stream insertion operator (<<) just as you use that operator to output information to the screen. The only difference is that you use an ofstream or fstream object instead of the cout object.
> 

## Reading from a File

> You read information from a file into your program using the stream extraction operator (>>) just as you use that operator to input information from the keyboard. The only difference is that you use an ifstream or fstream object instead of the cin object.
> 

## Read and Write Example

> Following is the C++ program which opens a file in reading and writing mode. After writing information entered by the user to a file named afile.dat, the program reads information from the file and outputs it onto the screen −
> 

More resources on: *[https://www.tutorialspoint.com/cplusplus/cpp_files_streams.htm](https://www.tutorialspoint.com/cplusplus/cpp_files_streams.htm)*

**PROJECT: STUDENT REPORT SYSTEM**

**SOURCE CODE:**

Through this project, we can learn a lot about input/output streams and the file management system of C++. Our program collects student details like name, roll number, marks in each subject, and calculates their grade. This is a simple console app. Note that we focus only on the correct inputs in this project, and you can enhance it to handle wrong inputs. Here is the source code:
```
#include<iostream>
#include<fstream>
#include<iomanip>
using namespace std;
// the class that stores data
class student
{
int rollno;
char name[50];
int eng_marks, math_marks, sci_marks, lang2_marks, cs_marks;
double average;
char grade;
public:
void getdata();
void showdata() const;
void calculate();
int retrollno() const;
}; //class ends here
void student::calculate()
{
average=(eng_marks+math_marks+sci_marks+lang2_marks+cs_marks)/5.0;
if(average>=90)
grade='A';
else if(average>=75)
grade='B';
else if(average>=50)
grade='C';
else
grade='F';
}
void student::getdata()
{
cout<<"\nEnter student's roll number: ";
cin>>rollno;
cout<<"\n\nEnter student name: ";
cin.ignore();
cin.getline(name,50);
cout<<"\nAll marks should be out of 100";
cout<<"\nEnter marks in English: ";
cin>>eng_marks;
cout<<"\nEnter marks in Math:  ";
cin>>math_marks;
cout<<"\nEnter marks in Science:  ";
cin>>sci_marks;
cout<<"\nEnter marks in 2nd language:  ";
cin>>lang2_marks;
cout<<"\nEnter marks in Computer science:  ";
cin>>cs_marks;
calculate();
}
void student::showdata() const
{
cout<<"\nRoll number of student : "<<rollno;
cout<<"\nName of student : "<<name;
cout<<"\nEnglish : "<<eng_marks;
cout<<"\nMaths : "<<math_marks;
cout<<"\nScience : "<<sci_marks;
cout<<"\nLanguage2 : "<<lang2_marks;
cout<<"\nComputer Science :"<<cs_marks;
cout<<"\nAverage Marks :"<<average;
cout<<"\nGrade of student is :"<<grade;
}
int  student::retrollno() const
{
return rollno;
}
//function declaration
void create_student();
void display_sp(int);//display particular record
void display_all(); // display all records
void delete_student(int);//delete particular record
void change_student(int);//edit particular record
//MAIN
int main()
{
char ch;
cout<<setprecision(2);
do
{
char ch;
int num;
system("cls");
cout<<"\n\n\n\tMENU";
cout<<"\n\n\t1.Create student record";
cout<<"\n\n\t2. Search student record";
cout<<"\n\n\t3. Display all students records ";
cout<<"\n\n\t4.Delete student record";
cout<<"\n\n\t5.Modify student record";
cout<<"\n\n\t6.Exit";
cout<<"\n\n\What is your Choice (1/2/3/4/5/6) ";
cin>>ch;
system("cls");
switch(ch)
{
case '1': create_student(); break;
case '2': cout<<"\n\n\tEnter The roll number ";
cin>>num;
display_sp(num); break;
case '3': display_all(); break;
case '4': cout<<"\n\n\tEnter The roll number: ";
cin>>num;
delete_student(num);break;
case '5': cout<<"\n\n\tEnter The roll number "; cin>>num;
change_student(num);break;
case '6': cout<<"Exiting, Thank you!";exit(0);
}
}while(ch!='6');
return 0;
}
//write student details to file
void create_student()
{
student stud;
ofstream oFile;
oFile.open("student.dat",ios::binary|ios::app);
stud.getdata();
oFile.write(reinterpret_cast<char *> (&stud), sizeof(student));
oFile.close();
    cout<<"\n\nStudent record Has Been Created ";
cin.ignore();
cin.get();
}
// read file records
void display_all()
{
student stud;
ifstream inFile;
inFile.open("student.dat",ios::binary);
if(!inFile)
{
cout<<"File could not be opened !! Press any Key to exit";
cin.ignore();
cin.get();
return;
}
cout<<"\n\n\n\t\tDISPLAYING ALL RECORDS\n\n";
while(inFile.read(reinterpret_cast<char *> (&stud), sizeof(student)))
{
st.showdata();
cout<<"\n\n====================================\n";
}
inFile.close();
cin.ignore();
cin.get();
}
//read specific record based on roll number
void display_sp(int n)
{
student stud;
ifstream iFile;
iFile.open("student.dat",ios::binary);
if(!iFile)
{
cout<<"File could not be opened... Press any Key to exit";
cin.ignore();
cin.get();
return;
}
bool flag=false;
while(iFile.read(reinterpret_cast<char *> (&stud), sizeof(student)))
{
if(stud.retrollno()==n)
{
stud.showdata();
flag=true;
}
}
iFile.close();
if(flag==false)
cout<<"\n\nrecord does not exist";
cin.ignore();
cin.get();
}
// modify record for specified roll number
void change_student(int n)
{
bool found=false;
student stud;
fstream fl;
fl.open("student.dat",ios::binary|ios::in|ios::out);
if(!fl)
{
cout<<"File could not be opened. Press any Key to exit...";
cin.ignore();
cin.get();
return;
}
    while(!fl.eof() && found==false)
{
fl.read(reinterpret_cast<char *> (&stud), sizeof(student));
if(stud.retrollno()==n)
{
stud.showdata();
cout<<"\n\Enter new student details:"<<endl;
stud.getdata();
  int pos=(-1)*static_cast<int>(sizeof(stud));
  fl.seekp(pos,ios::cur);
  fl.write(reinterpret_cast<char *> (&stud), sizeof(student));
  cout<<"\n\n\t Record Updated";
  found=true;
}
}
File.close();
if(found==false)
cout<<"\n\n Record Not Found ";
cin.ignore();
cin.get();
}
//delete record with particular roll number
void delete_student(int n)
{
student stud;
ifstream iFile;
iFile.open("student.dat",ios::binary);
if(!iFile)
{
cout<<"File could not be opened... Press any Key to exit...";
cin.ignore();
cin.get();
return;
}
ofstream oFile;
oFile.open("Temp.dat",ios::out);
iFile.seekg(0,ios::beg);
while(iFile.read(reinterpret_cast<char *> (&stud), sizeof(student)))
{
if(stud.retrollno()!=n)
{
oFile.write(reinterpret_cast<char *> (&stud), sizeof(student));
}
}
oFile.close();
iFile.close();
remove("student.dat");
rename("Temp.dat","student.dat");
cout<<"\n\n\tRecord Deleted ..";
cin.ignore();
cin.get();
}
  ```
	
<h1>C++ STL (Standard Template Library)</h1>
<br><br>
	<p><b><i>Contents : </i></b><h4>Vectors - </h4><a href="#vectors"> Vectors </a><br><h4>Sets - </h4> <a href="#sets">  Sets  </a><a href="#unordered_sets">   Unordered Sets   </a><a href="#multiset">   Multiset    </a><br> <h4>Queue - </h4><a href="#queue"> queue </a><a href="#pqueue">  Priority Queue  </a><br><h4>Maps - </h4><a href="#map"> Maps </a><a href="#unordered_map">   Unordered Map   </a> <a href="#multimap">  Multimap </a><br><h4>Stacks - </h4><a href="#stacks"> Stack </a></p>
<br><br>
<div id = "vectors"></div>
<h1 align="center"><a href="#"> Vectors </a></h1>

<h2>INTRODUCTION</h2>

The simplest STL container is vector. <br />
Vector is just an array with extended functionality. In other words, vectors are dynamic arrays.

<h2>CONSTRUCTION</h2>

```C++
vector<datatype> a;  //empty vector
vector<datatype> b (no of elements, value of each element); //fixed number of elements with default value
vector<datatype> c (starting iterator/pointer,ending iterator/pointer); //inserting elements from other data structures
vector<datatype> d (name of vector to be copied);    
vector<vector<datatype> > matrix(no of rows,vector<datatype>(no of coloumn,default value)) //Declaring a 2D array

// Note:
vector<datatype> v[10]; // following declaration isn't a vector with 10 elements but an array of size ten having vector elements

```
<br />

<h2>FUNCTIONS</h2>

| <center>Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :-------------                | :-------------                   | :-------------               |
| <a>at()</a>        |Returns the reference to the element at a particular position (can also be done using ‘[ ]’ operator)       |O(1)
| <a>clear()</a>        |Deletes all the elements from the vector and assign an empty vector       |O(N)
| <a>pop_back()</a>        |Removes the last element from the vector       |O(1)
| <a>push_back()</a>        |Inserts a new element at the end of the vector       |O(1)
| <a>resize()</a>        |Resizes the vector to the new length which can be less than or greater than the current length       |O(N)


<h2>PASSING AS ARGUMENT TO FUNCTION</h2>

Another very important thing that you should remember: When vector is passed as a parameter to some function, a copy of vector is actually created. It may take a lot of time and memory to create new vectors when they are not really needed.
```C++
void some_function(vector<int> v) { // Never do it unless you’re sure what you do!
      // ...
 }
```
Instead, use the following construction:
```C++
int modify_vector(vector<int>& v) { // Correct
      V[0]++;
 }
```

<h2>Implementation</h2>

```C++
#include <iostream>
#include <vector>

using namespace std;

int main()
{
    vector <int> v;
    v.push_back(5);
    while(v.back() > 0)
        v.push_back(v.back() - 1);
    for(int i = 0;i < v.size();++i)
        cout << v.at(i) << ' ';
    cout << endl;
    while(!v.empty())
    {
        cout << v.back() << ' ';
        v.pop_back();
    }
    cout << endl;
    return 0;
}
```

Output:
```
5 4 3 2 1 0
0 1 2 3 4 5
```
<br />

<div id ="sets"> </div>
<h1 align="center" ><a href="http://www.cplusplus.com/reference/set/set/"> Sets </a></h1>

> Sets are containers which store only unique values and permit easy look ups.

> The values in the sets are stored in some specific order (like ascending or descending).

> Elements can only be inserted or deleted, but cannot be modified.

> We can access and traverse set elements using iterators just like vectors.
<br>

<div id = "members"></div>
 Operations( Member functions )

| <center>Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :------------- | :------------- | :------------- |
| <a href="#">begin( )</a>        | Returns an iterator to the first element of the set.       | O(1)
| <a href="#">end( ) </a>      | Returns an iterator pointing to a position which is next to the last element       | O(1)
| <a href="#">clear( )</a>     |  Deletes all the elements in the set and the set will be empty.       | O(N)
| <a href="#">count( ) </a>    | Returns 1 or 0 if the element is in the set or not respectively.       | O(logN)
| <a href="#">empty( ) </a>       |  Returns true if the set is empty and false if the set has at least one element       | O(1)
| <a href="#">erase( ) </a>      |  Deletes a particular element or a range of elements from the set.       | O(N)
| <a href="#">find( ) </a>      | Searches for a particular element and returns the iterator pointing to the element if the element is found otherwise it will return the iterator returned by end().       | O(logN)
| <a href="#">size( ) </a>      | Returns the size of the set or the number of elements in the set.       | O(1)
| <a href="#">insert( ) </a>      |  insert a new element.       | O(1)

<br>


### Implementation

```cpp
// declaratation

set<int> s1;                               // Empty Set
int a[]= {1, 2, 3, 4, 5, 5};
set<int> s2 (a, a + 6);                    // s2 = {1, 2, 3, 4, 5}
set<int> s4 (s3.begin(), s3.end());         // Set created using iterators
```

```cpp
#include <iostream>
#include<cstdio>
#include <set>

using namespace std;

int main()
{
        set <int> s;
        set <int>::iterator it;         // iterator to traverse
        int A[] = {3, 5, 2, 1, 5, 4};
        for(int i = 0;i < 6;++i)
                s.insert(A[i]);
        s.erase(A[3]);                  // erases 1 form the set
        printf("size of set %d\n",(int)s.size());
        for(it = s.begin();it != s.end();++it)
                cout << *it << ' ';
        cout << endl;
        return 0;

}
```
Output:
```
size of set 4
2 3 4 5
```
<br>

### Problems

 * codechef
<br>

<div id = "unordered_sets"></div>
<h1 align="center" ><a href="http://www.cplusplus.com/reference/unordered_set/unordered_set/"> Unordered-Sets </a></h1>

> Unordered sets are containers that store unique elements in no particular order, and which allow for fast retrieval of individual elements based on their value.

> Pros : Faster than sets (promises amortized O(1) for search) .

> Cons : Look up not guaranteed to be O(1) Therotical worst case is O(n)


### Note : Implementation && <a href="#members">Member functions</a> are similar as <a href="#sets">Sets</a> .

### Problems

 * codechef
<br>

<div id ="multiset"></div>
<h1 align="center"><a href="http://www.cplusplus.com/reference/set/multiset/"> Multiset </a></h1>

> Multisets are a type of associative containers similar to set, with an exception that multiple elements can have same values.

> Internally, the elements in a multiset are always sorted following a specific strict weak ordering criterion indicated by its internal [comparison object](http://www.cplusplus.com/reference/map/multimap/key_comp/) (of type Compare).
<br>

```cpp
        multiset <int , greater<int> > m ;
        m.insert(40);
        m.insert(60);
        m.insert(20);
        m.insert(60); // 60 will be added again to the multiset unlike set
```

### Note : [Implementation](http://www.cplusplus.com/reference/set/multiset/multiset/) && Member functions are same as <a href="#members">Sets</a> .

### Extending <a href="#members"> This </a> :

| <center>   Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :------------- | :------------- | :------------- |
| <a href="#">rbegin()</a>        | Returns a reverse iterator pointing to the last element in the container     | O(1)
| <a href="#">rend() </a>      | Returns a reverse iterator pointing to the theoretical element right before the first element in the  container   | O(1)
| <a href="#">equal_range() </a>     |  The function returns a pair, whose member pair::first is the lower bound of the range (the same as lower_bound), and pair::second is the upper bound     | O(logN)

### Problems

 * codechef
<br>

<div id = "queue"></div>
<h1 align="center"><a href="http://www.cplusplus.com/reference/queue/queue/"> Queue </a></h1>


> Queue is a container which follows FIFO  order (First In First Out).

> Elements are inserted at one end (  Rear  ) and extracted from another end( Front )

<br />

### Operations( Member functions )

| <center>Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :------------- | :------------- | :------------- |
| <a href="#">push( )</a>        | Inserts an element in queue at one end(rear).       | O(1)
| <a href="#">pop( )</a>     | Deletes an element from another end if queue(front).       | O(1)
| <a href="#">front( ) </a>    | Access the element on the front end of queue.       | O(1)
| <a href="#">empty( ) </a>       | Checks if the queue is empty or not.       | O(1)
| <a href="#">size( ) </a>      | returns the size of queue.       | O(1)

<br />

### Implementation

```cpp
#include<iostream>
#include<cstdio>
#include<queue>           

using namespace std;

int main(){
        int  i ;
        queue <int> q ;                 // declaratation
        for ( i = 1 ; i < 4; i++ ){
                q.push(i*i);
        }
        printf("Size of queue %d \n ", q.size());
        while(!q.empty()){
                printf(" %d ",q.front());
                q.pop();
        }
        return 0 ;
}
```
<br />

### Problems

 * codechef

<br />

<div id = "pqueue"></div>
<h1 align="center" ><a href="http://www.cplusplus.com/reference/queue/priority_queue/"> Priority-Queue </a></h1>

> A priority queue is a container that provides constant time extraction of the largest element .

> In a priority queue, an element with high priority is served before an element with low priority.

> All insertion / deletion operations takes place in Logarithmic time .


<br />

### Operations( Member functions )

| <center>Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :------------- | :------------- | :------------- |
| <a href="#">push( )</a>        | Inserts a new element in the priority queue.       | O(logN)
| <a href="#">pop( )</a>     | Removes the largest(Top) element from the priority queue .       | O(LogN)
| <a href="#">top( ) </a>    | Returns a reference to the largest element in the priority queue.       | O(1)
| <a href="#">empty( ) </a>       |  Returns true if the priority queue is empty and false if the priority queue has at least one element       | O(1)
| <a href="#">size( ) </a>      | Returns the number of element in the priority queue.       | O(1)

<br />


### Implementation

```cpp
#include <iostream>
#include <queue>

using namespace std;

int main()
{
    priority_queue<int> pq;             // declaratation
    pq.push(10);
    pq.push(20);
    pq.push(5);
    while(!pq.empty())
    {
        cout << pq.top() << endl;
        pq.pop();
    }
    return 0;
}
```
<br />

### Problems
 * codechef


#### Note - Follow up [deque](http://www.cplusplus.com/reference/deque/deque/) as above

	
<div align="center" id="map">
	<h1 align="center">Map</h1>
</div>

<h2>Introduction:</h2>

A map is a datastructure to store a key value pair.

<h2>Import:</h2>

```cpp
#include <map>
```

<h2>Properties:</h2>

1. It is a datastructure which stores a key value pair.

2. Elements are referenced using their keys not by position(unlike arrays).

3. The elements are stored in orders(i.e. they are pre-sorted).

4. Internal implementation is like a binary tree.

5. Size is increased and decreased automatically, according to storage needs.

6. Keys are unique. Same key cannot be used to store more than 1 values.

<h2>Usage:</h2>
<h3>1. Initialize</h3>

Template has two data types first for key and second for value. User defined comparator can be added as third parameter.

<h3>2. Constructors</h3>
<h4>1. Default:</h4> Makes an empty container.
<br>
```cpp
map<Type1, Type2> var_name; //Starts the var_name map with no key value pairs
```

<br>

<h4>2. Range:</h4> Used to copy range of elements from one map to other.

```cpp
map<Type1, Type2> var_name1;
//fill 10 elements in var_name
//If want to copy elements from 0-10
map<Type1, Type2>  var_name2(var_name1.begin(),var_name1.end());
```

Note: The template types should be same.<br>
<h4>3. Copy:</h4>
Copy entire container in new map object.<br>

```cpp
map<Type1, Type2> var_name(map_object);
```

Copies the map_object in var_name. The map_object should be of same type.<br><br>

<h3>3. Insert</h3>
<h4>1. Insert using key and value directly, using array-like syntax.</h4>

```cpp
map<char, int> map_object;
map_object['a'] = 10;
```

<h5 style="display:inline">Note:</h5> This method overwrites the previous value (if any).

<h4>2. Insert using insert()</h4>

```cpp
map_object.insert(make_pair<char, int>('b', 20));
```

<h5 style="display:inline">Note:</h5> This method does not overwrite the previous value (if any) but returns an object pointing to the previous value and new value is not inserted.

<h4>3. Returned object of insert()</h4>

The return_object is a pair, first is an iterator to inserted element(or the same key element if insertion was prevented) and second is a boolean object which is true if insert happened and is false if it was stopped.
<br>

```cpp
#include<maps>
map<char,int> mymap;
mymap.insert ( pair<char,int>('a',100) );
mymap.insert ( pair<char,int>('z',200) );

pair<std::map<char,int>::iterator,bool> ret;
ret = mymap.insert (pair<char,int>('z',500) );
if (ret.second==false) {
	cout << "element 'z' already existed";
	cout << " with a value of " << ret.first->second << '\n';
}
```

<h3>4. Access</h3>

<h4>1. Access using key directly</h4>

```cpp
cout << mymap['b'];
```

<h4>2. Access using at()</h4>

```cpp
cout << mymap.at('b');
```

<h4>3. Access using find()</h4>

```cpp
cout << mymap.find('b')->second;
cout << (*mymap.find('b')).second;
```
<h5 style="display:inline">Note:</h5> This method returns an iterator to the elements.

<h3>5. Delete</h3>
<h4>1. erase()</h4>

```cpp
mymap.erase('b');
it = mymap.find('a');
mymap.erase(it, mymap.end());
```

<h3>6. Iteration</h3>

<h4>1. Begin()</h4>Returns an iterator to first element in the map.
<h4>2. End()</h4>Returns an iterator to the end of map (<b>Not the last element</b>).

```cpp
map<char,int> mymap;

mymap['b'] = 100;
mymap['a'] = 200;
mymap['c'] = 300;
for (std::map<char,int>::iterator it=mymap.begin(); it!=mymap.end(); it++)
	std::cout << it->first << " => " << it->second << '\n';
return 0;
```

<h2>Complexities</h2>

<h3>Insert: O(log(n))</h3>
<h3>Access: O(log(n))</h3>
<h3>Delete: O(1) + Access = O(log(n))</h3>


<div align="center" id="unordered_map">
	<h1 align="center">Unordered Map</h1>
</div>

<h2>Introduction:</h2>

An unordered map is a datastructure to store a key value pair and access it fast enough.

<h2>Import:</h2>

```cpp
#include <unordered_map>
```

<h2>Properties:</h2>

1. It is a datastructure which stores a key value pair.

2. Elements are referenced using their keys not by position(unlike arrays).

3. The elements are not sorted.

4. Internal implementation is using hashing.

5. Size is increased and decreased automatically, according to storage needs.

6. Keys are unique. Same key cannot be used to store more than 1 values.

7. Introduced in C++11.

<h2>Usage</h2>
<h3>1. Initialize</h3>

Template has two data types first for key and second for value.

<h3>2. Constructors</h3>
<h4>1. Default:</h4> Makes an empty container.

```cpp
unordered_map<Type1, Type2> var_name; //Starts the var_name map with no key value pairs
```

<br>

<h4>2. Range:</h4> Used to copy range of elements from one map to other.

```cpp
unordered_map<Type1, Type2> var_name1;
//fill 10 elements in var_name
//If want to copy elements from 0-10
unordered_map<Type1, Type2>  var_name2(var_name1.begin(),var_name1.end());
```

Note: The template types should be same.<br>
<h4>3. Copy:</h4>
Copy entire container in new map object.<br>

```cpp
unordered_map<Type1, Type2> var_name(map_object);
```

Copies the map_object in var_name. The map_object should be of same type.<br><br>
<h4>4. List:</h4>
Initialize a list as a key value pair.


<h3>3. Insert</h3>
<h4>1. Insert using key and value directly, using array-like syntax.</h4>

```cpp
unordered_map<char, int> map_object;
map_object['a'] = 10;
```

<h5 style="display:inline">Note:</h5> This method overwrites the previous value (if any).

<h4>2. Insert using insert()</h4>

```cpp
map_object.insert(make_pair<char, int>('b', 20));
```

<h5 style="display:inline">Note:</h5> This method does not overwrite the previous value (if any) but returns an object pointing to the previous value and new value is not inserted.

<h4>3. Returned object of insert()</h4>

The return_object is a pair, first is an iterator to inserted element(or the same key element if insertion was prevented) and second is a boolean object which is true if insert happened and is false if it was stopped.

```cpp
unordered_map<char,int> mymap;
mymap.insert ( pair<char,int>('a',100) );
mymap.insert ( pair<char,int>('z',200) );

pair<std::map<char,int>::iterator,bool> ret;
ret = mymap.insert (pair<char,int>('z',500) );
if (ret.second==false) {
	cout << "element 'z' already existed";
	cout << " with a value of " << ret.first->second << '\n';
}
```

<h3>4. Access</h3>

<h4>1. Access using key directly</h4>

```cpp
cout << mymap['b'];
```

<h4>2. Access using at()</h4>

```cpp
cout << mymap.at('b');
```

<h4>3. Access using find()</h4>

```cpp
cout << mymap.find('b')->second;
cout << (*mymap.find('b')).second;
```

<h5 style="display:inline">Note:</h5> This method returns an iterator to the elements.

<h3>5. Delete</h3>
<h4>1. erase()</h4>

```cpp
mymap.erase('b');
it = mymap.find('a');
mymap.erase(it, mymap.end());
```

<h3>6. Iteration</h3>

<h4>1. Begin()</h4>Returns an iterator to first element in the map.
<h4>2. End()</h4>Returns an iterator to the end of map (<b>Not the last element</b>).

```cpp
unordered_map<char,int> mymap;

mymap['b'] = 100;
mymap['a'] = 200;
mymap['c'] = 300;
for (unordered_map<char,int>::iterator it=mymap.begin(); it!=mymap.end(); it++)
	cout << it->first << " => " << it->second << '\n';
return 0;
```

<h2>Complexities</h2>

<h3>Insert (Average Case): O(1)</h3>
<h3>Insert (Worst Case): O(n)</h3>
<h3>Access: O(1)</h3>
<h3>Delete (Average Case): O(1)</h3>
<h3>Delete (Worst Case): O(n)</h3>


<div align="center" id="multimap">
	<h1 align="center">Multimap</h1>
</div>

<h2>Introduction:</h2>

A Multimap is a datastructure to store a key value pair having multiple keys.

<h2>Import:</h2>

```cpp
#include <map>
```

<h2>Properites:</h2>

Same as maps but only it can have multiple values for a key.

<h2>Usage:</h2>
<h3>1. Initialize</h3>

Template has two data types first for key and second for value. User defined comparator can be added as third parameter.

<h3>2. Constructors</h3>
<h4>1. Default:</h4> Makes an empty container.

```cpp
multimap<Type1, Type2> var_name; //Starts the var_name map with no key value pairs
```

<br>

<h4>2. Range:</h4> Used to copy range of elements from one map to other.

```cpp
multimap<Type1, Type2> var_name1;
//fill 10 elements in var_name
//If want to copy elements from 0-10
multimap<Type1, Type2>  var_name2(var_name1.begin(),var_name1.end());
```

Note: The template types should be same.<br>
<h4>3. Copy:</h4>
Copy entire container in new map object.<br>

```cpp
multimap<Type1, Type2> var_name(map_object);
```

Copies the map_object in var_name. The map_object should be of same type.<br><br>
<h3>3. Insert</h3>
<h4>1. Insert using insert()</h4>
This method inserts an element with the key and value provided.
Use <a href = "http://www.cplusplus.com/reference/map/multimap/find/">this</a> link because it is very similar to maps and unordered_maps.
<h3>4. Access</h3>
<h4>1. Access using find()</h4>
Returns an iterator to an arbitrary element of possibly multiple elements having the given key.<br>
<a href="http://www.cplusplus.com/reference/map/multimap/find/">Example</a>

<h4>2. Access using equal_range()</h4>
Returns a pair of iterators. First is an iterator to the first element having the given key. Second is the iterator to the next to last element having the key.<br>
<a href="http://www.cplusplus.com/reference/map/multimap/equal_range/">Example</a>

<h3>5. Delete</h3>
<h4>1. erase()</h4>
Deletes an element using its iterator. Same as maps and unordered_maps.<br>
<a href="http://www.cplusplus.com/reference/map/multimap/erase/">Example</a>

<h3>6: Iteration</h3>
Same as maps and unordered_maps.<br>
<a href="http://www.cplusplus.com/reference/map/multimap/begin/">Example</a>

<h2>Complexities</h2>
<h3>Insert: O(log(n))</h3>
<h3>Access: O(log(n))</h3>
<h3>Delete: O(1) + Access = O(log(n))</h3>

<div id = "stacks"></div>
<h1 align="center"><a href="#"> Stacks </a></h1>

<h2>INTRODUCTION</h2>

Stacks are dynamic data structures that follow the Last In First Out (LIFO) principle. The last item to be inserted into a stack is the first one to be deleted from it.<br>

For example, you have a stack of trays on a table. The tray at the top of the stack is the first item to be moved if you require a tray from that stack.<br>

Stacks have restrictions on the insertion and deletion of elements. Elements can be inserted or deleted only from one end of the stack i.e. from the *top*. The element at the top is called the *top* element. The operations of inserting and deleting elements are called push() and pop() respectively.<br>

<h2>CONSTRUCTION</h2>

```cpp
stack <datatype> name;
```

<h2>FUNCTIONS</h2>

| <center>Function </center>    | <center>What it does ?</center>  | <center>Complexity</center>  |
| :-------------                | :-------------                   | :-------------               |
| <a>empty() </a>        |Returns whether the stack is empty    |O(1)
| <a>size() </a>        |Returns the size of the stack   |O(1)
| <a>top() </a>        |Returns a reference to the top most element of the stack   |O(1)
| <a>push(g)</a>        |Adds the element ‘g’ at the top of the stack    |O(1)
| <a>pop() </a>        |Deletes the top most element of the stack   |O(1)

<h2>Implementation</h2>

```cpp
#include <iostream>
#include <stack>

using namespace std;

void showstack(stack <int> kj)
{
    stack <int> c = kj;
    while (!c.empty())
    {
        cout << '\t' << c.top();
        c.pop();
    }
    cout << '\n';
}

int main ()
{
    stack <int> KJC;
    KJC.push(10);
    KJC.push(30);
    KJC.push(20);
    KJC.push(5);
    KJC.push(1);

    cout << "The stack KJC is : ";
    showstack(KJC);

    cout << "\nKJC.size() : " << KJC.size();
    cout << "\nKJC.top() : " << KJC.top();


    cout << "\nKJC.pop() : ";
    KJC.pop();
    showstack(KJC);

    return 0;
}

```

Output

```
The stack KJC is : 	1	5	20	30	10

KJC.size() : 5
KJC.top() : 1
KJC.pop() : 	5	20	30	10

```
