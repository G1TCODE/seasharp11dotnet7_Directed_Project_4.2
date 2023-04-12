# seasharp11dotnet7_Directed_Project_4.2

This application is my attempt at a coding challenge found in C#11 and .NET 7 - Modern Cross-Platform Development Fundamentals by Mark J. Price. This exercise can be found in Chapter 4 on page 197.

I have been coding for about 3 months while working full-time, and I am excited to continue learning and eventually break into the industry (hopefully!).

Reading Mark's book has taught me a bunch and I highly recommend it to anyone. 

///BREAK///
PROJECT DETAILS

Update: The Version 3 branch is my latest version of this application. While creating unit tests for the primeFactors() method, it came to my attention that my use of the "return null;" statement had unintended consequences, and that it was not simply making Compiler Error CS0161 go away. While primeFactors() was writing correct strings to the console as intended, it was returning a null value everytime it was invoked. This resulted in it failing every unit test, even though all the correct values were printing to the console. 

I fixed this issue by defining the method so that its return value was a List<string> instead of a string, and then replacing "return null;" with "return finalProduct;", which is a list of strings. I also instantiated the PFLib class in the main program class before invoking one of its methods (primeFactors()), and cleaned up the algorithm in the primeFactors() method so that it treated every scenario uniformly instead of unique responses to each scenario.

While Version 2 ran and compiled fine, I believe this version will be more reliable, and it is more in line with commonly accepted software development principles than the previous version was. 

This definitely taught me why utilizing test-driven development principles is important!

The purpose of this application is to provide the user with the prime factors of any number entered by the user under 1,001.

The solution contains a C# Console Application that references a Class Library.

The class library contains an array of all of the prime numbers up to 1,000 and the definition of a method that contains an algorithm for determining which of those prime numbers are associated with the user's entry. 

The toughest parts of this project for me were type conversions, adding project references, unit testing, and algorithm design. The files uploaded in this repository represent Version 3 of the project. While it is far from perfect, I have cleaned up a lot of the code from my original and second attempt.

I understand that this code may be more complex than is necessary, and that it could probably be faster and more efficient. If you have any suggestions for code improvement or resources that would help me along, please send them my way! 
