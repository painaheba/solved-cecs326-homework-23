Download Link: https://assignmentchef.com/product/solved-cecs326-homework-23
<br>
Purpose: This assignment provides experience with checksums and digests.

1) Get a copy of the instructor’s checksum.txt file from the 326 directory.

<ol>

 <li>Use the Linux system cksum command to compute the checksum of the file. Your results should be the same as every other student in the class. Report the checksum in hexadecimal.</li>

 <li>Modify one letter in the file. Pick one randomly, do not modify the same letter as another student. Runthe cksum command on the modified file. Report the check sum in hexadecimal.</li>

</ol>

Hint: with the command bc -l you can set the output base of the display to hexacdecimal with the commmand “obase=16”. Just type in a decimal number and hit return to get the hexadecimal equivalent.

2) Redo homework 2, copy.c (again).

As you make the copy, compute the md5 hash. After you are done the copy, print the md5 hash. Check your program to make sure identical files give identical hashes and different files give different hashes.

You will need to read and write in blocks of 64 bytes.

The size of the file may not be exact multiple of 64 bytes. To handle this we will pad the file with zeros. The easiest way to do this is: before you read, use the memset command to zero out the entire buffer. Now if the read is shorter than 64 bytes, the rest of the buffer is already zero.

An extended version of the md5.c program from lecture is provided in the 326 directory.

Demo: Part 2.

Submit: Part 1 handwritten or printed. Include the commands you ran, the letter you changed, and the resulting checksums.

Nathan Pickrell             28 November 2019 (Week 13 Lecture 2)             Due: 5 December 2019 (Week 14, Lab 2)