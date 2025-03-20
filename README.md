# DSA_Nicolas_midtrem-exam
//NUMBER1
// Create a new JavaScript file named userProfile.js.
// Collect the following user information with the use of prompt():
let fullName = prompt("Enter your full name (first and last name):");
let age = prompt("Enter your age:");
let favoriteNumber = prompt("Enter your favorite number:");
let favoriteColor = prompt("Enter your favorite color:");

// Use these variables to store the collected information and log it in the console.
console.log("Full Name:", fullName);
console.log("Age:", age);
console.log("Favorite Number:", favoriteNumber);
console.log("Favorite Color:", favoriteColor);
//NUMBER2
// Create a new JavaScript file named classSubjects.js.
// Collect the following user information with the use of prompt():
let subjectTitle = prompt("Enter the subject title:");
let classSchedule = prompt("Enter the class schedule (Time, Days):");
let classroom = prompt("Enter the classroom:");
let classInstructor = prompt("Enter the class instructor:");
let studentName = prompt("Enter the student name:");

// Use variables to store this information and log it to the console following the string 
// "{Student Name} is currently enrolled in {Subject Title} with a class schedule of {Class 
// Schedule} at room {Classroom}. The instructor for the subject is {Class Instructor}"
console.log(`${studentName} is currently enrolled in ${subjectTitle} with a class schedule of ${classSchedule} at room ${classroom}. The instructor for the subject is ${classInstructor}`);
//NUMBER3
// Collect the user's age using prompt
let age = parseInt(prompt("Please enter your age:"));

// Use a conditional statement to categorize the user into one of the following age groups:
let ageCategory;

if (age < 5) {
  ageCategory = "Toddler";
} else if (age >= 5 && age <= 12) {
  ageCategory = "Child";
} else if (age >= 13 && age <= 19) {
  ageCategory = "Teenager";
} else if (age >= 20 && age <= 35) {
  ageCategory = "Young Adult";
} else if (age >= 36 && age <= 60) {
  ageCategory = "Middle-Aged";
} else {
  ageCategory = "Senior";
}

// Log the appropriate message for each category in the console log.
console.log(`You are categorized as a ${ageCategory}.`);
//NUMBER4
// Declare a variable that will hold the favNumber.  Let's assume a random number between 1 and 100 for demonstration.
const favNumber = Math.floor(Math.random() * 100) + 1;

// Use a while loop and prompt() window object to ask the user to guess their favorite number until they guess correctly.
let guess;
let correct = false;

while (!correct) {
  guess = parseInt(prompt("Guess my favorite number (between 1 and 100):"));

  // For each guess, log whether the guess is too high, too low, or correct.
  if (guess === favNumber) {
    console.log("Correct!");
    correct = true;
  } else if (guess < favNumber) {
    console.log("Too low!");
  } else {
    console.log("Too high!");
  }
}
//NUMBER5
// Create an array to store three colors the user likes.
let favoriteColors = [];

// Use a prompt() window object and a loop statement to allow the user to input a value.
for (let i = 0; i < 3; i++) {
  let color = prompt(`Enter your favorite color #${i + 1}:`);
  favoriteColors.push(color);
}

// Use the push() method to add a new color to the array.  Let's add one more for demonstration.
let newColor = prompt("Enter one more favorite color:");
favoriteColors.push(newColor);

// Each push() or user input, the array list must be updated and printed out to the console log.
console.log("Your favorite colors are:", favoriteColors);
//NUMBER6
// Create a prompt that will ask for the user to create a grocery list (y/n):
let createList = prompt("Do you want to create a grocery list? (y/n)");

if (createList.toLowerCase() === "y") {
  // The program then must ask for user input the number of items to be registered in the grocery list.
  let numItems = parseInt(prompt("How many items do you want to add?"));

  // The program must ask for the items to be included in the list.
  let groceryList = [];
  for (let i = 0; i < numItems; i++) {
    let item = prompt(`Enter item ${i + 1}:`);
    groceryList.push(item);
  }

  // The grocery list must be sorted out safely and stored in groceryListSort, and reversed safely and stored in groceryListReverse.
  let groceryListSort = [...groceryList].sort(); // Create a copy to avoid modifying the original
  let groceryListReverse = [...groceryList].reverse(); // Create a copy to avoid modifying the original

  // Print via alert() the grocery list, groceryListSort, and groceryListReverse.
  alert(`Original Grocery List: ${groceryList}\nSorted Grocery List: ${groceryListSort}\nReversed Grocery List: ${groceryListReverse}`);
} else {
  alert("Grocery list creation cancelled.");
}
//NUMBER6
// Create a prompt that will ask for the user to create a grocery list (y/n):
let createList = prompt("Do you want to create a grocery list? (y/n)");

if (createList.toLowerCase() === "y") {
  // The program then must ask for user input the number of items to be registered in the grocery list.
  let numItems = parseInt(prompt("How many items do you want to add?"));

  // The program must ask for the items to be included in the list.
  let groceryList = [];
  for (let i = 0; i < numItems; i++) {
    let item = prompt(`Enter item ${i + 1}:`);
    groceryList.push(item);
  }

  // The grocery list must be sorted out safely and stored in groceryListSort, and reversed safely and stored in groceryListReverse.
  let groceryListSort = [...groceryList].sort(); // Create a copy to avoid modifying the original
  let groceryListReverse = [...groceryList].reverse(); // Create a copy to avoid modifying the original

  // Print via alert() the grocery list, groceryListSort, and groceryListReverse.
  alert(`Original Grocery List: ${groceryList}\nSorted Grocery List: ${groceryListSort}\nReversed Grocery List: ${groceryListReverse}`);
} else {
  alert("Grocery list creation cancelled.");
}
