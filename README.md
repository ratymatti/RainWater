# RainWater Trapping

This is a Java program that calculates the amount of rainwater that can be trapped within a histogram represented by an array of heights. It uses a two-pointer approach to efficiently find the amount of rainwater that can be stored between the heights.

## How It Works

The program works by iterating through the array of heights from both the left and right sides using two pointers. It maintains two variables, `leftBound` and `rightBound`, which represent the maximum height encountered from the left and right sides, respectively. The `totalWater` variable accumulates the amount of water trapped.

- The `leftPointer` starts from the leftmost element, and the `rightPointer` starts from the rightmost element.
- While the `leftPointer` is less than the `rightPointer`, it checks the heights at these positions.
- If the height at the `leftPointer` is less than or equal to the height at the `rightPointer`, the program updates `leftBound` and accumulates the trapped water between `leftBound` and the current height. Then, it increments the `leftPointer`.
- If the height at the `leftPointer` is greater than the height at the `rightPointer`, the program updates `rightBound` and accumulates the trapped water between `rightBound` and the current height. Then, it decrements the `rightPointer`.

The program continues this process until the `leftPointer` and `rightPointer` meet, and the total trapped water is calculated.

## How to Use

1. Clone this repository to your local machine.
2. Make sure you have Java installed.
3. Compile and run the program using the following commands:

```bash
javac RainWater.java
java RainWater

