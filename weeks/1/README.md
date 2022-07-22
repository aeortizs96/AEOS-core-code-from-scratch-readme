## Week 1  <img src="https://i.postimg.cc/DZ6VWxqs/Recurso-2.png" with="50px" height="50px" alt="Recurso-1"/>

### Tuesday 19 July, 2022

:boom:**Exercise 1** Explanation about Interpreted And Compiled Programming Languages

        A compiled programming language is a language that needs to be transcribed from a 
        human language into a machine language;
        It is said that this type of languages were the first to be created.

        Then we have the interpreted programming languages, these languages are famous 
        because they are executed while compiling.

        I liked very much to read in the article the information of the Python programming 
        language, because it can be executed as a compiled program or as an interpreted  
        language. 
        
    
| Compiled      | Interpreted | Hybrid |
| ----------- | ----------- |----------- |
| C      | PHP       |Java |
| C++   | JavaScript       |Python |





:boom:**Exercise 2**  The language java is compiled and interpreted

        It is said that the java programming language is compiled and interpreted   
        because as you can see in the image, initially a program is created 
        containing .java files, in this file is written the java language that then 
        goes through the java compiler process that is known as javac, previously this 
        process was done by console, now it is done with a run button, from that 
        moment it is converted to a language that the machine can read, this language 
        is called ByteCode, this file will contain strange characters and symbols, 
        finally it arrives to the JVM and creates the multiplatform effect.

<img src="https://i.postimg.cc/RF5x8xb9/1.png" with="100px" height="200px" alt="Recurso-1"/>

:boom:**Exercise 3** Convert USD to BTC

~~~
        START
        PRINT 'Hello User, please enter the number to convert'
        ValueA <-- 0.000044
        ValueB <-- GET 

        IF ValueA >= 0
        TotalC <-- ValueA * ValueB
        PRINT ' The value of ' ValueB  ' USD '  ' in BTC is' TotalC

        ELSE
        PRINT 'Hello User, please enter a valid number'
        ENDIF
        END
~~~

:boom:**Exercise 4** Low-Level vs High-Level Programming Languages

        The low level languages are those that are closer to the communication with the hardware architecture and the high 
        level languages have a language closer to the human language and are used by programmers.
        
        
### Wednesday 20 July, 2022  
  
:boom:**Exercise 1**

To convert a decimal number to binary, successive divisions by 2 must be made and the remainders obtained in each division must be written in the inverse order in which they were obtained.

        1996 / 2 = 998 Residuo: 1
        998 / 2 = 499 Residuo: 0
        499 / 2 = 249 Residuo: 1 
        249 / 2 = 124 Residuo: 1
        124 / 2 = 62 Residuo: 0
        62 / 2 = 31 Residuo: 0
        31 / 2 = 15 Residuo: 1
        15 / 2 = 7 Residuo: 1
        7 / 2 = 3 Residuo: 1
        3 / 2 = 1 Residuo: 1


:boom:**Exercise 2** MIPS exercise

>Create a program that adds any two given numbers provided by the user

~~~
 .data
 
 	      message: .asciiz "\nHello User\n"
	      value1: .asciiz "\nEnter the first number: "
	      value2: .asciiz "\nEnter the second number: "
	      result_message1: .asciiz "\nThe numbers are "
	      result_message2: .asciiz " and "
.text
	      main:
                          
             # Print the code
              li $v0, 4 
              la $a0, message
              syscall  # instruction printing
              
              
              # call number 1
              
              li $v0, 4 
              la $a0, value1
              syscall  
              
              li $v0, 5  #create one block
              syscall
              
              move $t1, $v0  #saves the variable
              
              # call number 2
              
              li $v0, 4 
              la $a0, value2
              syscall  
              
              li $v0, 5  
              syscall
              
              move $t2, $v0 
              
              li $v0, 4 
              la $a0, result_message1
              syscall  
              
              # now, print one number integer
              li $v0, 1
              
              # Second, we are telling the computer where is the number that we want to print
              move $a0, $t1
              syscall
              
              li $v0, 4 
              la $a0, result_message2
              syscall 
              
              li $v0, 1
              
	      move $a0, $t2
              syscall
 ~~~
            
            
>Create a program that displays your name

~~~
  .data
	      message: .asciiz "\nHello what your name? "
	      message2: .asciiz "\n Nice to meet you "
	      userImput: .space 20
  .text
	      main:
              
              li $v0, 4
              la $a0 message
              syscall

	      # Getting user's input as text
	      li $v0, 8
              la $a0, userImput
              li $a1, 20
              syscall
              
              #Display Nice to meet you
              li $v0, 4
              la $a0 message2
              syscall
              
              #Display the name
              li $v0, 4
              la $a0 userImput
              syscall
              
              li $v0, 10
              syscall
~~~


### Thursday 21 July, 2022

:boom:**Exercise 1** Print special numbers

~~~
		for (let i = 0; i <= 100; i++) {
 			if((i % 2) == 0 ){
			 console.log(i);
 			}  
		}
~~~
