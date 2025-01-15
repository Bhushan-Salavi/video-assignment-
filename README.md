# video-assignment-
        explaining the Global Execution Context, Function Execution Context, and the Call Stack 


Google Drive Link of Video=https://drive.google.com/file/d/1vdNLbThUazljIYrYe0GN85eqYxqZEkEu/view?usp=sharing


Execution Context -
        An execution context is an environment where JavaScript code runs. It determines what variables and functions are accessible.

    Type of Execution Context:
      1)Global Execution Context
      2)Function Execution Context

    1)Global Execution Context:-
       The Global Execution Context (GEC) is the default environment where your code begins 
     execution. It is created when the JavaScript engine starts running your script.

      The engine scans the code and allocates memory for variables and functions. Variables 
    declared with var are initialized with undefined, while let and const are stored in a 
    "temporal dead zone" until they are initialized.

    Example 
            var x = 10;
            let y = 20;

             function greet() {
                console.log("Hello, World!");
              }


      2)Function Execution Context:-
          A Function Execution Context (FEC) is created whenever a function is called. Each 
      function call gets its own unique execution context.

      Variable Environment for variables declared inside the function.
      Lexical Environment linked to the outer (parent) environment.
      This Binding specific to how the function was called.

       Example
       function add(a, b) {
            var result = a + b;
            return result;
        }
          var sum = add(5, 10);



     Call Stack:-
          The Call Stack is a data structure that keeps track of all the execution contexts in 
    the order they were created. It's a stack-based structure (LIFO: Last In, First Out).

    The GEC is pushed onto the stack.
    When a function is called, its FEC is pushed onto the stack.
    When the function finishes, its FEC is popped off the stack.

    Example 
     function multiply(x, y) {
        return x * y;
     }

     function square(n) {
        return multiply(n, n);
     }

     console.log(square(4));












    
