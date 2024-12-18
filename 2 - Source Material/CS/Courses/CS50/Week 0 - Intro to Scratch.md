

computational thinking - a clean, straight forward way of thinking

problem solving - you have an input, need a specified output, what you do to get input and convert to correct output is problem solving\

bit - binary digit, either 0 or 1

a byte represents the number 255, 2^8 is 256, but we start at 0, so 0-255 is still 256 combinations

the English alphabet starts at binary value 65, the letter A


| pattern of bits        | 0        | 1       | 0      | 0     | 0    | 0   | 0   | 1   |        |
| ---------------------- | -------- | ------- | ------ | ----- | ---- | --- | --- | --- | ------ |
| nth place (binary)     | 128      | 64      | 32     | 16    | 8    | 4   | 2   | 1   |        |
| representation of bits | 0        | 64      | 0      | 0     | 0    | 0   | 0   | 1   | **65** |
| nth place (decimal)    | 10000000 | 1000000 | 100000 | 10000 | 1000 | 100 | 10  | 1   |        |

The alphabet is represented through a system called **ASCII**, along with various different English symbols



Representation of "Hi!" in binary

| **H**                  |     |     |     |     |     |     |     |     |                       |
| ---------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --------------------- |
| pattern of bits        | 0   | 1   | 0   | 0   | 1   | 0   | 0   | 0   |                       |
| nth place (binary      | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |                       |
| representation of bits | 0   | 64  | 0   | 0   | 8   | 0   | 0   | 0   | **72** = 'H' in ASCII |


| **I**                  |     |     |     |     |     |     |     |     |                       |
| ---------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --------------------- |
| pattern of bits        | 0   | 1   | 0   | 0   | 1   | 0   | 0   | 1   |                       |
| nth place (binary      | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |                       |
| representation of bits | 0   | 64  | 0   | 0   | 8   | 0   | 0   | 1   | **73** = 'I' in ASCII |


| **!**                  |     |     |     |     |     |     |     |     |                       |
| ---------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --------------------- |
| pattern of bits        | 0   | 0   | 1   | 0   | 0   | 0   | 0   | 1   |                       |
| nth place (binary      | 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |                       |
| representation of bits | 0   | 0   | 32  | 0   | 8   | 0   | 0   | 1   | **33** = '!' in ASCII |


Stopped at 38:00

We use unicode now as well, a superset of ASCII, that can use up to 32 bits per character, about 4 bytes, so 2^32

Unicode code point - standard way to represent unicode, uses hexadecimal, base-16

e.g. Skin tones for emojis. a default (yellow) thumbs up can be represented as unicode code point U+1F44D. A light skinned thumbs up can be represented with U+1F44D, but also by adding U+1F3FD, so U+1F44D U+1F3FD

A man-man emoji with a heart in the middle would have the unicode code point: 
U+1F468 U+200D U+2764 U+FE0F U+200D U+1F68

| U+1F468     | U+200D                   | U+2764      | U+FE0F               | U+200D                   | U+1F68      |
| ----------- | ------------------------ | ----------- | -------------------- | ------------------------ | ----------- |
| A man emoji | "glue" to connect emojis | heart emoji | color of heart emoji | "glue" to connect emojis | A man emoji |
Each code point represents a part of the final product. Male emoji can be switch out by female emoji's unicode code point, color of heart, etc.

stopped at 45:00


RGB represents a series of 3 numbers that represent how much of red, green, and blue should be represented

**Context matters** - the same set of numbers can represent different things, all based on the context. e.g. '72 73 33' can be represented by either a color if the context is in a graphical program, a word if it's in an email, or a number if shown in a calculator app


A 3MB image has about a million pixels, each pixel holding 3 bytes

So we have input -> [blank] -> output, what fills the "blank"? **Algorithms**

algorithm - step by step instructions

code - implementing an algorithm 

there are different degrees of how long it to solve a problem and the size of the problem as well, known as time complexity (Big-O notation, i.e. O(1), O(N), O(log n), etc, N being the number of instructions)

Pseudocode used to write out your thinking *algorithm*, you give a detailed step-by-step explanation on how to do something, i.e. :
//How to open a door knob
Reach out hand
Grab door knob
Rotate door knob
Push door
Enter door way
close door 

AI - uses ***large language models*** to search and create a human response back to the user 

### Scratch

In scratch, functions are represented in puzzle-like shapes, shapes that have an opening for a "connecting" piece and a connecting piece for "connecting" to other "shapes", or functions. If we think of functions as a puzzle piece, it makes great sense. You see, the missing chunk of the puzzle piece would be the parameters, what is expected to be passed in in order to use a function. The chunk that is meant to connect to another puzzle piece would be the arguments, or in other terms the **return*** value. It is what is being passed based on a function call within function or like we mentioned, the return value of the function. Interesting.

 return value - a value that is "returned" after finishing the process of a function

Stopped at 1:27:51