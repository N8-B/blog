# Program development life cycle, the good way
This is in my experience, the best way to  develop programs right now. You might not agree with this, and that's ok as long as your team be productive. 

![Program-life-cycle.png](https://github.com/juliomatcom/blog/raw/master/content/program-life-cycle-2.png)
##### 1. Problem definition - Fully understand what is the **problem**
First we better know exactly what is the problem, this is the moment to ask if anything is not clear as crystal in the specifications.

##### 2. Problem analysis - Find a valid **solution** for your team
Really, many developers tend to just start writing code before they know the solution to the problem, is like start walking to an unknown place without GPS, chances that you will get lost are huges. Just stay away from the keyboard for now.

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
Once you have the problem solved correctly (you have tried it against the tests), is the right time to add more tests for the edges cases and refactor or optimize as necessary.

##### 7. Deployment
[Software deployment](https://en.wikipedia.org/wiki/Software_deployment) is all of the activities that make a software system available for use. Yes, integrate the solution in the *stable* product often mean prepare branches, do some merges, resolve conflicts, make pull requests, CI, and release, this takes time of our everyday work (sometimes too much), so the process of deployment is very important in the development life cycle.

#### Go back to 1


###### Read more
- [http://gsl.mit.edu/media/programs/peru-summer-2014/materials/t04-_software_development_life_cycle.pdf](http://gsl.mit.edu/media/programs/peru-summer-2014/materials/t04-_software_development_life_cycle.pdf)
- [http://www.btechsmartclass.com/CP/program-development.htm](http://www.btechsmartclass.com/CP/program-development.htm)
- [The Six Steps in the ProgramDevelopment Life Cycle (PDLC)](http://www.academia.edu/15483069/The_Six_Steps_in_the_Program_Development_Life_Cycle_PDLC)
