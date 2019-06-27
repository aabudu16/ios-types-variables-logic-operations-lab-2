/* 1. You are given three grades obtained by 3 students, which are stored in variables grade1, grade2, grade3 and all of type Double. Create a variable called yourGrade of type Double and give it a value. Print "above average" if your grade is greater than the class average or "below average" otherwise.
*/

var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0

var yourGrade:Double = 22.0
var classAverge = (grade1 + grade2 + grade3 + yourGrade)/4

if yourGrade > classAverge{
print("your score of \(yourGrade) above average")
}else {
print("your score of \(yourGrade) below average")
}

//2. You are given a number. Print even if the number is even or odd otherwise.

let number = 2

if number % 2 == 0{
print ("even")
}else {
print("odd")
}

//3. You are given two numbers a and b. Print "divisible" if a is divisible by b and "not divisible" otherwise.

var a = 12
var b = 3

if a % b == 0{
print ("is divisible")
}else {
print("not divisible")
}

//4 . You are given three variables a, b and c. Check if at least two variables have the same value. If that is true, print "At least two variables have the same value" otherwise print "All the values are different".

var a1 = 2
var b1 = 3
var c1 = 2

if a1 == b1 || a1 == c1 || b1 == c1 {
print ("At least two variables have the same value")
}else {
print ("At least two variables have the same value")
}

//5. You are working on a smart-fridge. The smart-fridge knows how old the eggs and bacon in it are. You know that eggs spoil after 3 weeks (21 days) and bacon after one week (7 days). Given baconAge and eggsAge (both in days) determine if you can cook bacon and eggs, or which ingredients you need to throw out. If you can cook bacon and eggs, print "you can cook bacon and eggs". If you need to throw out any ingredients, for each one print a line with the text "throw out" + bacon or eggs.

var baconAge = 6 // the bacon is 6 days old
var eggsAge = 12 // eggs are 12 days old

if (baconAge < 7 && eggsAge < 21) {
print("you can cook bacon and eggs")
}else if (baconAge < 7 && eggsAge > 21) {
print("you can ONLY cook bacon and you have \(7 - baconAge) days left. Throw out the eggs.")
} else if (baconAge > 7 && eggsAge < 21) {
print("you can ONLY cook the eggs and  you have \(21 - eggsAge) days left. Throw out the bacon.")
}else {
print ("throw out both the bacon and eggs. they are old")
}

//6 .You are given a year, determine if it’s a leap year. A leap year is a year containing an extra day. It has 366 days instead of the normal 365 days. The extra day is added in February, which has 29 days instead of the normal 28 days. Leap years occur every 4 years. 2012 was a leap year and 2016 will also be a leap year. The above rule is valid except that every 100 years special rules apply. Years that are divisible by 100 are not leap years if they are not also divisible by 400. For example 1900 was not a leap year, but 2000 was. Print "Leap year!" or "Not a leap year!" depending on the year you are provided.

let year = 2014

if year % 4 == 0 {
if year % 100 != 0 || year % 400 == 0 {
print ("Leap year!")
} else {
print ("Not a leap year")
}
}

//7. If you use random() it will give you a random number within a specified range. Generate a random number and use it to simulate a coin toss. Print "heads" or "tails".

let randomNum = Int.random(in: 0...100)

if randomNum != 0 {
if randomNum % 2 == 0 {
print ("heads")
} else {
print ("tails")
}
}

//8. You are given four variables a, b, c and d. Print the value of the smallest one.

var a2 = 5
var b2 = 6
var c2 = 3
var d2 = 4

if (a2 < b2) && (a2 < c2) && (a2 < d2) {
print ("\(a2) is the smallest value")
}else if (b2 < a2) && (b2 < c2) && (b2 < d2){
print ("\(b2) is the smallest value")
}else if (c2 < a2) && (c2 < b2) && (c2 < d2){
print ("\(c2) is the smallest value")
}else {
print ("\(d2) is the smallest value")
}


var array = [a2,b2,c2,d2]
array.min()

