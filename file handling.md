# File Handling:
1. File is a collection of data which occupied some space in the disk.
2. C++ file handling provide a machanism to store output of a program in a file and read output from a file display on the disk.
3. Files are mainly deals with three classes "fstream", "ifstream", "ofsteam" available in fstream readfile.
# uses:
1. ifstream = To read the information from the file.
2. ofstream = To write something into a file we have to create object ofsteam.
3. fstream = to perform both read and write operation, we have to create object fstream. 

# text mode vs binary mode:
- Text mode is default opening mode.
- Binary mode can be specified with ios::binary
- cout<<"My name is \nAayush";
In this line the meaning of "\n" is consider, it means "\n" is for new line character.

In screen,

"My name is

Aayush"

will be print.

- fout<<"My name is \nAayush";

If we write this line in file, "\n" will be print as it is or the meaning of "\n" will be consider, it depend in which mode the file is open. text mode or binary mode?
 
 If this file is open in text mode, then the meaning of "\n" will be print i.e., new line. whereas in binary mode "\n" will print as it is.