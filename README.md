# C-learning
C++ self learning


Reading Book C++ Primer 5th edition 

### Pointers
```
int *ip = &x;  
```
* pointer & address  

### Reference
```
int x = 7;
int *ip = &x;
int &y = x;

7
7
7
```
y refer to x  

```
int x = 7;
int *ip = &x;
int &y = x;

y = 8

8
8
8
```
Difference  
1.do not use an asterix to dereference a Reference  
2.no syntax for changing a reference  

note: C does not have Reference  

### Primitive Array
```
int ia[5]
ia[0] = 1  #same effect as *ia = 1
int *ip = ia;
*ip = 2;
#1st element of the Array
++ip;
*ip = 3;
*(++ip)=4;
```

### Primitive String
string is a special case of the Array  
a C string is a primitive array of characters ending with zero  
also called null terminated string   
```
char s[] = {'s','t','r','i','n','g',0}
for(char *cp = s';*cp;++cp){
  .....
}
for(char c :s){
  if(c == 0)break;
  ...
}
```

### conditionals
contine statement : goes back to the top  

### Enumeration
Enum in C++ is a data type that contains fixed set of constants.  
Points to remember for C++ Enum  
enum improves type safety  
enum can be easily used in switch  
enum can be traversed  
enum can have fields, constructors and methods  
enum may implement many interfaces but cannot extend any class because it internally extends Enum class
from https://www.javatpoint.com/cpp-enumeration
https://www.geeksforgeeks.org/enumeration-enum-c/  

### null
null pointer constant  nullptr
