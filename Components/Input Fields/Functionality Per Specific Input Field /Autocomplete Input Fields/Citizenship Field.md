# Citizenship Field

## The Basics
* A user is able to enter any country into this field. 
* A user is able to add commas/special characters (ex: Côte d'Ivoire).

## Validations/Error Messages
* When a user types an invalid/misspelled country of citizenship into the field, the error message “Please enter a country of citizenship” is displayed.
    * However, when a user mistypes a country name and then hits the tab button, the first autocomplete suggestion in the list below will be selected.

## Developer Notes
* Typed input displays suggestions based on input data and geography-data (countries only).
* On invalid country entered, event sent to Google Analytics "Error - Traveler Citizenship".

