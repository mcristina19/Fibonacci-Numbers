# Fibonacci-Numbers

Fibonacci Numbers is a list of numbers in which each number (after the first two) is the sum of the two preceding ones.
This shows the two ways you can get the Fibonacci numbers by a generator or a list. 

The process to create the Fibonacci Numbers generator:
* First create a function with one parameter (number). 
* Next create two variables for the first two numbers.
      a = 0
      b = 1
* Then create a range generator that will loop whatever number of times the number parameter is given. 
* Now you want to make a to equal what b was and b to be the next number. To do that first yield a which will keep whatever number a is (a is 0 at this point) but then pauses the function until the next part. 
* Next create a temporary variable that will hold on to what a was when you get there which was 0.
* After you want to modify a to equal b, which is 1
* Then you want to make b = temp + b, and b was originally 1 so it’s  0 + 1 
* Finally to try out the function write,
      for x in fib(21):
            print(x)
This code is saying for every number in the function fib run this function 21 times. 
* In order to get the first 20 numbers you have to put 21 as the parameter because the count starts at 0 so if 20 was the parameter you would only get the first 19 numbers.

The process to create the Fibonacci Numbers in a list is very similar to the generator way that you can copy the previous code and start with that.
* First you change the function name, in this case I did fib2
* With a list you need to add an empty list. 
      result = []
* Instead of yield a, replace that with result.append(a). This will append the value a which is 0.
* Then keep the following code the same from before the same so instead of yeilding a it's now adding the value a to the list.
* At the end add return result, which will return the list
* Finally to run the function print(fib2(21))
