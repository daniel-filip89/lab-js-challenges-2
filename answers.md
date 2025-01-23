1. Challenge 1:

- Answer: b

- Explanation:

  Inside the bar() function, the global variable foo is reassigned to "xyz".
  The first console.log(foo) (inside the function) outputs "xyz".
  The second console.log(foo) (outside the function) also outputs "xyz" because the global variable foo was modified.

2. Challenge 2:

- Answer: c

- Explanation:

  When the function is called as example(a), the value of the global a (which is 1) is passed as an argument.
  Inside the function, the parameter a shadows the global a, creating a local variable a specific to the function scope.
  The local a is then assigned the value 10, and console.log(a) inside the function logs the local a, which is 10.
  The global a remains unaffected by what happens inside the function because the parameter a inside the function is local to that function.
  Therefore, when console.log(a) is called outside the function, it logs the global a, which is still 1.

3. Challenge 3:

- Answer: c

- Explanation:

In JavaScript, function declarations are hoisted to the top of their scope. This means that the function sayHi is available to be called even if the function call (sayHi()) appears before the function definition in the code.
  Unlike var, let, or const variables, function declarations are hoisted with their entire definition. So the JavaScript engine knows about sayHi and its implementation before executing the code.
  The sayHi() function is called, and its body is executed. Inside the function, the statement console.log("Hi there!"); is executed, which prints "Hi there!" to the console.
  There is no ReferenceError or TypeError because sayHi is properly defined as a function before its execution.
  The function does not return anything, so there is no undefined being logged.

4. Challenge 4:

- Answer: c

- Explanation:

The variable a is declared as a const, which means the reference that a holds cannot be reassigned to a different object or value.
However, the properties of the object that a references (in this case, { num: 42 }) can be modified.
When you assign const b = a;, both a and b point to the same object in memory.
Modifying b.num = 90; changes the num property of the object in memory. Since a references the same object, the change is reflected in a as well.
After b.num = 90;, the object becomes { num: 90 }.
When you log a, it outputs the modified object { num: 90 }.

5. Bonus - Challenge 5:

- Answer:
- Explanation:
