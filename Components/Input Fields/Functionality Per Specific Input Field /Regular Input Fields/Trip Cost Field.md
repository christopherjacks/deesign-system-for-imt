# Trip Cost Field

## The Basics
* On focus, on mobile, a number keyboard appears
* Commas autofill  
* A user is also able to enter a period and there is a message that alerts the user that the number will be rounded 
    * See WEB-518 for more details.

## Validations/Error Messages

* This is not a required field
* A user is only be able to enter numbers in this field 
* A user will receive an error message if they enter more than $100,000.00 (minus $1) per traveler. 
    * Ex: A single user cannot enter more than $99,999.00 in total trip cost. A group of five travlers cannot enter a total trip cost of more than $499,999.00. 
* If a user tries to enter more than $99,999.00 per traveler into this field, the error message “Maximum cannot exceed $100,000 per traveler” appears
* When a user adds a period and their trip cost will be rounded, a message that reads “We will round up your cost to the nearest whole dollar. Some insurance providers require whole dollar trip costs.” appears
* Users should not be able to enter dashes (negative numbers) in the input field.

## Developer Notes
* Max is $100,000.00 minus $1 per traveler 
* Decimals allowed, rounded to nearest dollar
* Validated as number in xx,xxx.xx format
* Google Analytics event on page validation