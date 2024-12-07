# lecture 2.2

>#### Two’s complement representation

> #### Advantages of 2’s complement representation

 * Mathematical operation on binary numbers
 * Both positive and negative numbers
 * All patterns are utilized
    * 8-bits can represent 256 numbers
 * Efficient addition and subtraction


>### Positive binary representation

 * Positive binary numbers are ordinary binary numbers:
    * Examples: 1, 101, 111000, 11100010
 * Smallest value: 0
 * Largest value: 2digits-1

* Overflow error can occur. Overflow says that the calculation is run, however, 
answer is not able to be stored in the computer
  * 8-digits: 1100 0000 + 1100 0000 = 1 1000 0000 (9-digits)  
  * 0100 0000 - 1000 0000 = less than zero

---

### Binary Coded Decimal

---


### Sign-Magnitude
 * Usually leftmost digit to represent the sign
    * In a 8-bit sign magnitude number
      * 1 bit (leftmost bit) (most significant bit) for sign
      * 7 bits for magnitude

### Binary Number Table

| Bit Size | Minimum Value (Binary)     | Maximum Value (Binary)     | Range (Decimal)     | Unique Values |
|----------|----------------------------|----------------------------|---------------------|---------------|
| 8-bit    | 1111 1111                  | 0111 1111                  | -127 to +127        | 255           |
| 16-bit   | 1111 1111 1111 1111        | 0111 1111 1111 1111        | -32767 to +32767    | 65535         |

---

### 1’s Complement Representation

>#### 1’s Complement Representation

* A useful mathematical tool to turn a subtraction into a complement and an 
addition operation
  * A simplify circuitry significantly
  * Complement is simple operation called “Negation”
      * All the 0s becomes 1s
      * All the 1s becomes 0s

* 1’s complement representation is the system that uses 1’s complement 
operation to 
work out a positive binary number’s corresponding negative number
* If the negative number is in 1’s complement format, we cannot directly 
convert it into decimal


>#### Two’s Complement Representation

* There is an extra step for 2’s complement representation (compared with 1’s 
complement representation)
 * Two steps:
   * 1’s complement operation (bit inversion)
   * Add one

Examples:    

 (b) 0100 1110 + 1110 1111  
* The second number is a negative number.
 However, the addition can be performed as usual.
 0100 1110 + 1110 1111 = ~~1~~ 0011 1101
 We drop the extra carry 1.
 Remark: 78 + (-17) = 61  


 (c) 0100 1110 - 1110 1111 
 * It is a subtraction problem
 Convert it back to addition
 0100 1110 - 1110 1111 becomes 0100 1110 + (-1110 1111) Apply 2’s complement to the second number 
0100 1110 + 0001 0001 = 0101 1111
 Remark: 78 - (-17) = 95

#### How to check whether there is overflow?


| Operation                                      | Overflow  | Detection                                      |
|------------------------------------------------|-----------|------------------------------------------------|
| Addition of two positive numbers               | Possible  | Overflow if the result is a negative number    |
| Addition of two negative numbers               | Possible  | Overflow if the result is a positive number    |
| Addition of one positive and one negative number| Impossible| N/A                                            |



>#### Arithmetic operations with 2’s complement representation

 * ALU has at least 3 operations
    * Negation, addition, subtraction
 * Number of bits to represent numbers in an ALU is fixed
    * Determine the range of numbers
    * Causes overflow errors

