# Data Structures and Algorithms with Java Basics

Welcome to the Data Structures and Algorithms with Java Basics repository! This repository is designed for beginners who are learning about data structures and algorithms using the Java programming language.

## Introduction

This repository aims to provide a beginner-friendly guide to understanding data structures and algorithms using Java. Whether you're new to programming or looking to strengthen your understanding of fundamental concepts, this repository is a great starting point.

## Content

The repository includes the following:

- **Code Examples:** Illustrated examples of various data structures and algorithms implemented in Java.
- **Explanatory Comments:** Detailed comments within the code to help learners understand the logic and functionality.


class Main {
    public static void main(String[] args) {
        int[] arr = {12, 18, 39, 10, 54, 23};
        int min = minNumber(arr);
        System.out.println(min);
    }

    // Method to find the minimum number in an array
    static int minNumber(int[] arr) {
        // Check if the array is empty
        if (arr.length == 0) {
            // Return some default value, or handle it according to your requirements
            System.out.println("Array is empty");
            return -1;
        }

        // Initialize the minimum to the first element of the array
        int min = arr[0];

        // Loop through the array starting from the second element
        for (int index = 1; index < arr.length; index++) {
            // Compare the current element with the current minimum
            if (arr[index] < min) {
                // Update the minimum if the current element is smaller
                min = arr[index];
            }
        }

        // Return the minimum value found in the array
        return min;
    }
}
