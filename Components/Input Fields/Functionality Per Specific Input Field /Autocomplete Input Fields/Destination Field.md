# Destination Field

## The Basics

* A user is able to add commas/special characters (ex: Côte d'Ivoire).
* A user is able to add hyphens (ex: Congo (Congo-Brazzaville)).
* A user is able to enter the previous name of a country. 
    * Ex: They are able to type Burma and get Myanmar as a result: Myanmar (formerly Burma).

**What is Listed**
* Countries
* Each of the states within the U.S. 
* Each U.S. overseas military base
* Each U.S. territory 
* Popular cities around the world
* Popular cities in the countries that our customers travel to most frequently

## Display

* United States (Orlando)
* United States (Rhode Island) 

* Saint Helena should appear if you type:
    * Saint Helena
    * St. Helena
    * St Helena

## Validations/Error Messages

* When a user focuses on the field and then clicks outside of the field, an error stating “Please select a valid destination” is shown. 
* When a user types an invalid/misspelled destination into the field, the error message “Please select a valid destination” is displayed.

## Developer Notes
* Typed input displays suggestions based on input data and geography-data
* Input is validated before being allowed to continue
* If invalid input is entered and there are suggestions available, the first suggestion is chosen in an attempt to combat typos and allow the user a chance to select the "closest" option
* On ALL bad input, event sent to Google Analytics "Error - Destination"
* Autocomplete
    * United States is omitted if first character is 's' or 'S'
    * If multiple matches are found only first entry for country is shown. For example, type in "Charl" into destination, then "Charle" and then "Charlo"
* Destination Mini App (Home Page)
    * Same rules as Destination above
    * On get a quote button clicked with valid input -> Google Analytics event "Home page - Get a quote button clicked", "Success - Entered dates page"
    * On get a quote button clicked with invalid input -> Google Analytics event "Home page - Get a quote button clicked", "Failure - Did not enter dates page"
    * On get a quote button clicked with invalid input -> Google Analytics event "Home page - Get a quote button clicked", "Failure - Did not enter dates page"
    * On valid input entered -> Google Analytics event "Home page - Destination Field", "Success - Destination selected from drop down"
