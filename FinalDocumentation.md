**Background:**
A brief introduction of lambda function and map function is given.

**Lambda Function:**
A lambda function, also known as an anonymous function or lambda expression, is a way to create small, inline, and nameless functions in Python. Lambda functions are typically used for simple operations or calculations.


**Example of Lambda function**
1)
 
add = lambda x, y: x + y
result = add(3, 5)
print(result)  # Output: 8




2)
numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))
print(squared)  # Output: [1, 4, 9, 16, 25]



**Map Function:**

The map() function in Python is used to apply a given function to all elements of an iterable (e.g., a list, tuple, or other iterable data structures) and return an iterator. It takes two arguments: the function to apply and the iterable to apply it to. The result is an iterator that yields the results of applying the function to each element of the iterable one by one.



**Example of syntax of map function**
1)
numbers = [1, 2, 3, 4, 5]
squared = list(map(lambda x: x**2, numbers))
print(squared)  # Output: [1, 4, 9, 16, 25]



>**Work Calculation and Testing Script by using lambda function and map function:**

This Python script defines a function for calculating work done by a car as a function of its velocities and mass.
It also includes a test function to ensure the correctness of the work calculation function.


**Steps:**
1) Define a function calculate_work_done(velocities, mass).
2) Calculates the work done by a car based on its velocities and mass.
3) Define parameters.
   velocities (list of float): A list of velocities (in m/s) at different points in time.
   mass (float): The mass of the car (in kilograms).
4) Returns:
    - `work_done` (list of float): A list of work done (in joules) at each point in time.
5) test_calculate_work_done()`: Tests the `calculate_work_done` function to ensure its correctness.

6) Usage:
    1. Defines given data (velocities in mph, conversion factor, mass of car).
    2. Converts velocities from mph to m/s by using the lambda function.
    3. Get a list of velocities in m/s by using the map function.
    4. Manually calculate the expected work done at each point.
    5. Calls `calculate_work_done` to calculate work done.
    6. Compares the calculated and expected values within a small tolerance.
    7. Prints the calculated work done.

## Stacked Bar Plot Documentation

## Introduction
This code generates a stacked bar plot using Matplotlib to visualize the relationship between velocity and work done. The plot displays work done (in Joules) at different velocities (in mph).

## Code Explanation
The code consists of several components:
**Setting Figure Size**: 
   - `plt.figure(figsize=(10, 6))`: This line sets the size of the figure to be 10 inches in width and 6 inches in height.

2. **Creating the Stacked Bar Plot**:
   - `plt.bar(velocities_mph, work_done_list, width=10, align='center', label='Work Done (Joules)')`: This line creates a stacked bar plot using the `bar()` function from Matplotlib. It uses `velocities_mph` as the x-axis values, `work_done_list` as the y-axis values, sets the bar width to 10 units, aligns the bars to the center of each x-value, and labels the bars as 'Work Done (Joules)'.

3. **Axis Labels and Title**:
   - `plt.xlabel('Velocity (mph)')`: Sets the label for the x-axis as 'Velocity (mph)'.
   - `plt.ylabel('Work Done (Joules)')`: Sets the label for the y-axis as 'Work Done (Joules)'.
   - `plt.title('Work Done vs. Velocity (Stacked Bar Plot)')`: Sets the title of the plot as 'Work Done vs. Velocity (Stacked Bar Plot)'.

4. **Grid Lines**:
   - `plt.grid(axis='y', linestyle='--', alpha=0.7)`: Adds dashed grid lines to the y-axis with an alpha (transparency) value of 0.7 for improved readability.

5. **Legend**:
   - `plt.legend()`: Adds a legend to the plot, which will display the label 'Work Done (Joules)' to explain the meaning of the bars.
6. **Displaying the Plot**:
   - `plt.show()`: Finally, this line displays the generated plot to the user.

## Usage
To use this code, you need to provide values for `velocities_mph` and `work_done_list`, which represent the velocities (in mph) and the corresponding work done (in Joules) for your specific dataset. You can modify these values to create a stacked bar plot for your own data.

**Code**
[WorkDonebyMapAndLambda.md](https://github.com/sharmistharanit/23-Homework3G4/files/12807475/WorkDonebyMapAndLambda.md)
![output_1_0](https://github.com/sharmistharanit/23-Homework3G4/assets/143737948/2bb3b4f0-59dd-48a1-8830-777e22dc304c)


**References:**
1) https://docs.python.org/3/howto/functional.html#small-functions-and-the-lambda-expression
2) https://docs.python.org/3/library/functions.html#map
3) https://docs.python.org/3/howto/functional.html
4) Chatgpt
