# [JSL03] Project Submission: Which one is which? Declarative or Imperative?!

Loom Recording Link: [Insert Link]

## Example #: 1 

The code uses the imperative approach, simulating a process step-by-step to cooking a steak. It focuses on how to cook steak in step-by-step instructions, from preheating the grill to serving the steak.

The let grillTemperature and steakTemperature variables are declared with values of 0, allowing them to adjust during the cooking process and hold the current temperature of the grill and the steak, respectively.

The following steps break down the process:
Step 1 explicitly assigns a value (204°C) to the grillTemperature variable. 
Step 2 assigns the only seasoning type to both sides of the steak to a constant seasoning variable. 
Step 3 uses a while loop to repeat the cooking process until the steakTemperature reaches the desiredDoneness. The while loop condition checks if the passed steak temperature argument is less than the passed steak doneness argument. The loop likely monitors and adjusts the grill temperature or cooking time and updates the steak temperature to reflect the progress until the steakTemperature once is no less than the desiredDoneness celsius to cook the steak to medium-rare.
Step 4 uses an if/else statement to check if the steakTemperature has reached the desired temperature level. If steakTemperature is greater than or equal to desiredDoneness, the function returns a message indicating the steak is ready or returns a message indicating the steak needs more cooking.

This imperative approach details the "how" to cook a steak and provides explicit instructions for each step. The while loop and if/else statement control the execution flow based on the current temperature state, modifying grillTemperature and steakTemperature variables throughout the process to track the changing level.


## Example #: 2

The code uses the declarative approach, defining the cooking process for a steak without explicitly detailing every step. The grillTemperatureCelsius and seasoning are declared as constant variables, representing the unchanging internal temperature and seasoning flavour.

The core logic resides in the cookingProcess variable declared as an array of objects. Each object represents an action and its details, describing the specific action to take and might have a temperature or desiredDoneness property based on the action taken.

The for-of loop iterates through each step in the cookingProcess array. A switch statement within the for-loop examines the current step's action property. Based on the action, the corresponding code snippet executes.

The declarative approach leverages data structures effectively using an array and objects. The cookingProcess array is the heart of this approach. It offers an ordered list of steps, and each element in the array is an object. This approach allows for a structured representation of each step, including the action and relevant details, promoting readability and maintainability.

## Learning Outcome

Imperative focuses on "how" to achieve the outcome through detailed instructions and can modify variables during execution, offering a clear and understandable way to represent the cooking process, potentially for beginners to follow the logic easily.

Declarative focuses on "what" needs to be done, leaving the execution details to built-in mechanisms and often favours immutability, using new data structures with the desired outcome. Declarative code can be more concise and understandable on complex processes by separating concerns.