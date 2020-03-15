# Depart/Return
* Past dates are grayed out
* There are two fields, one for departure dates and one for return dates
    * On focus, the date field calendar appears
    
## The Basics
* On focus, on mobile, the calendar appears in the users viewport, either below or above the input field
* On desktop or tablets the calendar appears just within the user’s view on screen
* Date picker allows you to jump by month and year
* A user can manually enter a date on desktop computers and mobile
    * If a user does not manually enter slashes, the form autofills the slashes
    * If a user does enter slashes, the form remains as is
    * A user is able to enter a two digit or four digit year

## Validations/Error Messages
Validation happens when the focus leaves a date field.

Error States:
* Departure Date
    * Date must be entered and complete (mm/dd/yyyy or mm/dd/yy).
        * Error message: Enter a date as mm/dd/yyyy.
    * Date must be < 10 years from current date.
        * Error message: Departure date must be within 10 years from now.
    * Date must not be in the past.
        * Error message: Departure date cannot be in the past.
* Return Date
    * Date must be entered and complete (mm/dd/yyyy or mm/dd/yy).
        * Error message: Enter a date as mm/dd/yyyy.
    * Date must be < 10 years from the Departure Date.
        * Error message: Your return date cannot be more than 10 years after your departure date.
    * Date must not be in the past.
        * Error message: Return date cannot be in the past.
    * Date must not be prior to the Departure Date.
        * Error message: Return date must be the same as or after the departure date.

## Developer Notes
* Input is validated as a valid date
* On invalid date entered, event sent to Google Analytics "Error - Travel Dates (Departure)"
* Past Dates are disabled
* Future Dates > 10 years are prevented, however, messaging states "{Departure/Return} date must be within a year from now"