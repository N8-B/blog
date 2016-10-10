# Program development life cycle, the good way
![Program-life-cycle.png](https://github.com/juliomatcom/blog/raw/master/content/Program-life-cycle.png)
##### 1. Problem definition - Fully understand what is the **problem**
First we better know exactly what is the problem, this is the moment to ask if anything is not clear as crystal in the specifications.

##### 2. Problem analysis - Find a valid **solution** for your team
Really, many developers tend to just start writing code before they know the solution to the problem, is like start walking to an unknow place without GPS, chances that you will get lost are huges. Just stay away from the keyboard for now.

##### 3. Algorithm - **Split** the problem into **smaller** problems
Reduce the main problem to smaller ones will make easier to resolve the whole puzzle, take this example:  
`Print the first n primes numbers which are valid for some condition`   
Will be more easy if we divide this problem in 3
- Make a prime generator
- Some validator of the condition for a given prime
- Print / output a list of number
 
Note that, it will be very easy to change *ie*, print with save in a database, or add another condition, because we divide the problem in smaller independent pieces so is easier to change a piece than one strongly linked solution.

##### 4. Write some core [tests](https://en.wikipedia.org/wiki/Test-driven_development) as you need it for the solution  
If you know what is the solution, you can test it!  
You will **save** a lot of **time** if you just run some tests after any change of the code base. 

##### 5. Coding - Write the solution
`/* CODE SOLUTION */ `

##### 6. Make tests for edge cases, refactor and documentation
Once you have the problem solved correctly (you have tried it against the tests), is the right time to add more tests for the edges cases and refactor or optimize as necesary.


#### Go back to 1
