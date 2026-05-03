# final-practiceUnit0--Arika---F-
// Meal Prep Planner - Unit 0 Code Examples

MODULE: Values, Data Types, and Operations
let mealName = "Grilled Chicken and Rice"; // string - the name of the meal
let mealCalories = 550; // number - calories in meal
let mealCost = 4.75; // number - how much it costs
let isHighProtein = true; // 
let tax = mealCost * 0.08; // multiply cost by 8% tax
let totalCost = mealCost + tax; // add tax to the original cost

console.log(totalCost); // Expected output: 5.13

MODULE: Stringing Characters Together
let mealSummary = `${mealName} has ${mealCalories} calories and costs $${totalCost.toFixed(2)}`;

console.log(mealSummary);
// Expected output: "Grilled Chicken and Rice has 550 calories and costs $5.13"

MODULE: Control Structures and Logic
Set the user's calorie goal
If the meal is at or under the goal, tell them it works
If not, tell them by how many calories it goes over

let userCalorieGoal = 500;

if (mealCalories <= userCalorieGoal) {
  console.log(mealName + "fits your calorie goal!");
} else {
  console.log(mealName + "is over your goal by" + (mealCalories - userCalorieGoal) + "calories. Try a lighter meal.");
}
// Expected output: "Grilled Chicken and Rice is over your goal by 50 calories. Try a lighter meal."

MODULE: Building Arrays
let availableMeals = ["Grilled Chicken and Rice","Ground Turkey and Veggies","Salmon and Sweet Potato","Greek Yogurt Parfait","Egg White Omelette"];

console.log(availableMeals);
// Expected output: a list of all 5 meals

MODULE: Using Arrays
Using .length to count the meals and brackets to grab a specific one.
let mealCount = availableMeals.length;
let featuredMeal = availableMeals[0];

console.log(mealCount); // Output: 5
console.log(featuredMeal); // Output: Grilled Chicken and Rice

MODULE: Working With Loops
Using a for loop to go through and display every meal in the list.
for (let i = 0; i < availableMeals.length; i++) {
  console.log(availableMeals[1][i]);
}
// Expected output:
// Option 1: Grilled Chicken and Rice
// Option 2: Ground Turkey and Veggies
// Option 3: Salmon and Sweet Potato
// Option 4: Greek Yogurt Parfait
// Option 5: Egg White Omelette
