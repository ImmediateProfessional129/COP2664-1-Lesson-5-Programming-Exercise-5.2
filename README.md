# COP2664-1-Lesson-5-Programming-Exercise-5.2
This repository is a submission link for COP264-1: Lesson 5 Programming Exercise 5.2

// This program is designed to check if the number 5 appears in an array from 1 to 10 or more and verify if it is in the array which makes it true or false.

import Foundation // Imports the Foundation library
var array = [1, 2, 3, 4, 5] // Creates an array with the numbers 1 to 5
var array2 = [1, 2, 3, 4] // Creates an array with the numbers 1 to 4
var array3 = [1, 2, 3, 4, 5, 6] // Creates an array with the numbers 1 to 6
func firstLast(array: [Int]) -> Bool { // Creates a function that takes an array as a parameter
  if array.first == 5 || array.last == 5 { // Checks if the first or last number in the array is 5
    return true // Returns true if the first or last number is 5
  } else { // If the first or last number is not 5
    return false // Returns false if the first or last number is not 5
  }
}
print(firstLast(array: array)) // Prints the result of the function with the array 1 to 5
print(firstLast(array: array2)) // Prints the result of the function with the array 1 to 4
print(firstLast(array: array3)) // Prints the result of the function with the array 1 to 6
func firstLast2(array: [Int]) -> Bool { // Creates a function that takes an array as a parameter
  if array.first == array.last { // Checks if the first and last number in the array is the same
    return true // Returns true if the first and last number is the same
  } else { // If the first and last number is not the same
    return false // Returns false if the first and last number is not the same
  }
}
print(firstLast2(array: array)) // Prints the result of the function with the array 1 to 5
print(firstLast2(array: array2)) // Prints the result of the function with the array 1 to 4
print(firstLast2(array: array3)) // Prints the result of the function with the array 1 to 6
func sum(array: [Int]) -> Int { // Creates a function that takes an array as a parameter
  var sum = 0 // Creates a variable that is equal to 0
  for i in array { // Creates a for loop that goes through the array
    sum += i // Adds the value of i to the sum
  }
  return sum // Returns the sum
}
print(sum(array: array)) // Prints the result of the function with the array 1 to 5
print(sum(array: array2)) // Prints the result of the function with the array 1 to 4
print(sum(array: array3)) // Prints the result of the function with the array 1 to 6
func sum2(array: [Int]) -> Int { // Creates a function that takes an array as a parameter
  if array.count == 0 { // Checks if the array is empty
    return 0 // Returns 0 if the array is empty
  } else { // If the array is not empty
    return array.first! + sum2(array: Array(array.dropFirst())) // Returns the first number in the array and the sum of the array without the first number
  }
}
print(sum2(array: array)) // Prints the result of the function with the array 1 to 5
print(sum2(array: array2)) // Prints the result of the function with the array 1 to 4
print(sum2(array: array3)) // Prints the result of the function with the array 1 to 6
func sum3(array: [Int]) -> Int { // Creates a function that takes an array as a parameter
  if array.count == 0 { // Checks if the array is empty
    return 0 // Returns 0 if the array is empty
  } else { // If the array is not empty
    return array.last! + sum3(array: Array(array.dropLast())) // Returns the last number in the array and the sum of the array without the last number
  }
}
print(sum3(array: array)) // Prints the result of the function with the array 1 to 5
print(sum3(array: array2)) // Prints the result of the function with the array 1 to 4
print(sum3(array: array3)) // Prints the result of the function with the array 1 to 6
func sum4(array: [Int]) -> Int { // Creates a function that takes an array as a parameter
  if array.count == 0 { // Checks if the array is empty
    return 0 // Returns 0 if the array is empty
  } else { // If the array is not empty
    return array.first! + sum4(array: Array(array.dropFirst())) // Returns the first number in the array and the sum of the array without the first number
  }
}
print(sum4(array: array)) // Prints the result of the function with the array 1 to 5
print(sum4(array: array2)) // Prints the result of the function with the array 1 to 4
print(sum4(array: array3)) // Prints the result of the function with the array 1 to 6
func sum5(array: [Int]) -> Int { // Creates a function that takes an array as a parameter
  if array.count == 0 { // Checks if the array is empty
    return 0 // Returns 0 if the array is empty
  } else { // If the array is not empty
    return array.last! + sum5(array: Array(array.dropLast())) // Returns the last number in the array and the sum of the array without the last number
  }
}
print(sum5(array: array)) // Prints the result of the function with the array 1 to 5
print(sum5(array: array2)) // Prints the result of the function with the array 1 to 4
print(sum5(array: array3)) // Prints the result of the function with the array 1 to 6
