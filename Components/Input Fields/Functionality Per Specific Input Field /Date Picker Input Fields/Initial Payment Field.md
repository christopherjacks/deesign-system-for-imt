# Initial Payment Date

## The Basics
* On focus, on mobile, the calendar appears in the users viewport, either below or above the input field
* On desktop or tablets the calendar appears just within the user’s view on screen
* Date picker allows you to jump by month and year
* A user can manually enter a date on desktop computers and mobile
    * If a user does not manually enter slashes, the form autofills the slashes
    * If a user does enter slashes, the form remains as is
    * A user is able to enter a two digit or four digit year
    
## Validations/Error Messages
* This is not a required field
* A user is not allowed to select future dates
* If a user chooses a date that is more than 5 years in the past, a message that stays “Initial trip payment cannot be more than 5 years in the past” is displayed. 
* A user can manually enter a date on desktop computers and mobile.
    * If a user does not manually enter slashes, the form autofills the slashes.
    * If a user does enter slashes, the form remains as is.
    * A user is able to enter a two digit or four digit year.

## Developer Notes
* Allowed to be blank
* Future dates are disallowed, however, the datepicker still lets you choose a future date. You are then presented with an error.
* Google Analytics event on page validation
