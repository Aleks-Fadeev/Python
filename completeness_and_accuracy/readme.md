# Completeness and accuracy.

**completeness_and_accuracy.ipynb** - code  
**test1.txt** - small test data  

**Task description.**  
We have an automatic license plate recognition system that accepts an image of a license plate as input and returns the recognized number as a string. The truck classifier is arranged as follows: it takes an image of the number as input, performs its recognition, and then checks the resulting string for compliance with the format adopted for trucks.  
Truck numbers have the following format:  
• region code (digit from 2 to 9);  
• hyphen (character '-');  
• a four-digit number from 11 to 99999999, written with leading zeros (for example, 0023);  
• two or three uppercase Latin letters. Combinations of BIG, BAG, BAG, BG, UG are acceptable, while combinations of BIG and BAD are not used for the region with the code "5".  
An example of a valid number that satisfies the specified format: 3-0023BAG.  
To control the quality of the classifier, a test sample of car license plate images was prepared. For your convenience, the sample is divided into two parts. The first part contains the results of number recognition, about the original images of which it is known for sure that they belong to heavy—duty vehicles, and the second part contains the results of number recognition of cars, about the images of which it is known for sure that they do not belong to heavy-duty vehicles.  
Calculate the completeness and accuracy of the classifier.  

**Input**  
The first line contains two numbers, n and k are integers.
This is followed by n+k lines with the results of car license plate recognition, of which the first n lines belong to the first part of the sample, and the next k lines belong to the second.
The length of one line is from 3 to 20 characters, it can include numbers, uppercase and lowercase letters of the Latin alphabet, as well as hyphens and spaces.  

**Output**  
Output two numbers: completeness and accuracy of the car license plate recognition system. The numbers should be output on one line separated by a space with an accuracy of at least four decimal places.
