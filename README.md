# effective-cpp

---
*17. 0824*   
## Item 28th:  

避免返回类private成员变量的引用，指针，或者迭代器。若如此，外部client将可以修改类的private变量。应该通过setter()函数来修改类的private成员。  

很多时候返回引用将效率更高。此时应该考虑返回const class_name&。来兼顾效率和封装性。

