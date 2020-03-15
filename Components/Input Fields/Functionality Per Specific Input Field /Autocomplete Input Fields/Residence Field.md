# Residence Field

## The Basics
* A user is able to enter any U.S./Canadian state, province, or territory into this field.
* A user may also enter “Neither U.S. nor Canada”.

## Validations/Error Messages
* When a user focuses on the field and then click outside of the field, an error stating “Please enter a state or province for residence” is shown. 
* When a user types an invalid/misspelled country of citizenship into the field, the message in the field automatically autofills with “Neither U.S. nor Canada”.

## Developer Notes
* Typed input displays suggestions based on input data and geography-data (states only)
* On empty input, event sent to Google Analytics "Error - Traveler Residence"
* On invalid residence entered, "Neither U.S. nor Canada" default is selected
* On invalid residence entered, "Neither U.S. nor Canada" default is selected
* Checks for primary residence (deprecated?)
* Does NOT check that residence is valid for citizenship (which is fine)
* Checks for Canadian residences to set residence country. Residence country is not collected via the quote process
