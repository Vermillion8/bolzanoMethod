# **Bolzano Method**

This program implements the bisection method for finding the roots of a function. It uses the bisection method to approximate the root of a given function within a specified error tolerance.

## **Function Definition**
The program starts by defining the function `f(x)` that represents the equation whose root needs to be found. In this case, the function is `x**3 - 3 * x + 1`. You can modify this function to solve for different equations.

## **Bisection Method Implementation**
The bisection method is implemented in the `bisection` function. It takes three parameters: `x0` and `x1` are the initial guesses for the root, and `e` is the error tolerance. The function iteratively bisects the interval `[x0, x1]` until the approximate root is found with the desired accuracy.

## **Execution**
The program sets the initial guess values `x0` and `x1` and the error tolerance `e`. It then checks if the initial guess values bracket the root by evaluating the function at those points. If they do not bracket the root, the program prints an error message and suggests trying different guess values. Otherwise, it proceeds to find the root using the bisection method.

During the bisection process, the program prints the iteration number, the current approximation `x2`, and the value of the function `f(x2)` at each iteration. Once the root is found, the program prints the final result.

## **Graph Plotting**
After finding the root, the program uses the `matplotlib` library to plot the graph of the function along with the root. It creates an array `x` of values from `x0` to `x1` with a step size of `e` and evaluates the function at those points to obtain the corresponding `y` values. The graph is then plotted using `plt.plot`.

The root is indicated on the graph by a vertical line and a red dot. The line is created using `plt.axvline` with the root value, and the dot is plotted using `plt.scatter` with the coordinates `(root, f(root))`.

## **Dependencies**
This program requires the following dependencies:

+ `matplotlib`: Make sure you have matplotlib installed to run the graph plotting part of the program.
You can install matplotlib using the following command:
```bash
pip install matplotlib
```

## **Screenshots**
![Screenshot 1](https://github.com/Vermillion8/image-dump/blob/main/Bolzano%20Method/Code_dn4az9ZmGH.png?raw=true)
![Screenshot 2](https://github.com/Vermillion8/image-dump/blob/main/Bolzano%20Method/python_I62jWUSIWZ.png?raw=true)

## **References**
+ Graph Plotting in Python: https://www.geeksforgeeks.org/graph-plotting-in-python-set-1/
+ Bisection Method Python Program: https://www.codesansar.com/numerical-methods/bisection-method-python-program.htm
