# Project1-RC4
creating a RC4 cipher that takes in an input file and prints it out to an output file
Project RC4

Specifications:

In this project you are to write the program “RC4.java” to implement stream cipher RC4.

Specifically, your program will read key, plaintext and ciphertext from a file named “input.txt”
(under the same directory of the program). Then your program should create a file named
“output.txt” (under the same directory) and writes the encryption and decryption results to
“output.txt”. 

Please check the attached sample files “input.txt” and “output.txt”.

input:
75 101 121
0000000000000000
eb9f7781b734ca72 

output:
eb9f7781b734ca72 
0000000000000000

In “input.txt”:

1. First line is the key represented by integers (from 0 to 255), separated by one blank space.

2. Second line is a plaintext presented by (even number of) hexadecimal digits, without blank space.

3. Third line is a ciphertext presented by (even number of) hexadecimal digits, without blank space.

In “output.txt”:

1. First line is the ciphertext presented by hexadecimal digits which is the encryption result of the plaintext in input.txt.

2. Second line is the plaintext presented by hexadecimal digits which is the decryption result of the ciphertext in input.txt.

Hints:

1. Please look up the documentation about java class java.lang.String through the main page
of the Java API:
(http://docs.oracle.com/javase/8/docs/api/).

a. Suppose the variable s stores a String object, the java code:

String[] x = s.split(regex);

Splits s around matches of the given regular expression, and stores the results to x.

For example, if the String variable s stores “1 2 3” and the String variable regex stores one blank space “ ”,

String[] x = s.split(regex);

Splits s around matches of “ ”, and stores the results to x such that x[0] = “1”, x[1] = “2”,
and x[2] = “3”.

2. Please look up the documentation about java class java.lang.Integer through the main page of the Java API 
(http://docs.oracle.com/javase/8/docs/api/).

a. The java code:

int y = Integer.valueOf(hexString, 16);

converts the hex string object stored in hexString to an integer, and stores the integer to y. 

For example, if hexString holds “a0”,

int y = Integer.valueOf(hexString, 16);

converts “a0” stored in hexString to 160, and stores 160 to y.

b. The java code:

String z = Integer.toHexString(intValue);

converts the integer stored in intValue to hexadecimal digits string, and stores the string to z. 

For example, if the integer variable intValue stores 160,

String z = Integer.toHexString(intValue);

converts 160 to “a0”, and stores “a0” to z.

3. It will be tested using command line.
First, the files “RC4.java” and “input.txt” will be placed under the same directory (A new “input.txt” file which is different than the sample data that will be used to test your program).

The command “javac RC4.java” will be entered to the command line to compile the java file and then
“java RC4” will be entered to the command line to run the program

Your program should output the file “output.txt” to the same directory. so be certain that your program compiles and runs correctly before you submit it!
