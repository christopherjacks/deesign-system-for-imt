# Accessibility

## The Basics
* A user must be able to write directly into the input field, even if a date picker option exists.
* The input field should be flexible and accept different date formats.

## Screen Readers
* The date picker button should not be hidden from screen readers. 
* The label should state the required date format. 
    * Add aria-required=”true”. 
    * You should not use placeholder text instead of using a label if the placeholder text disappears on focus.
* Buttons in the date picker should have the correct label for each date. It is not enough just to read the number date, instead, screen readers should note the date, day of the week, and year.
    * Ex: Dates should be read as “4 April, Monday”.
    * You can use aria-label for this.
* When the month or the year in the date picker changes, the screen reader should announce the new date and/or year.
* When a date is selected, the date name (ex: 4 April, Monday), should be read back to the user as the date picker closes.

## Keyboard Navigation
* When a date picker is opened, a live region allows screen readers to provide keyboard instructions on how to move throughout the date picker. 
    * These instructions should also be listed at the bottom of the dialog box.  
* Arrow keys navigate through months in a non-sequential manner.
* Down/up arrow keys bring users to the same day in the next/previous week.
* Page down/up moves users to the same date in the next/previous month.
* Tab allows users to navigate between the next/previous month buttons and the close button. 
* The escape key should close the date picker without selecting a date, and the keyboard focus should return to the input field/date picker icon.
* The date picker should provide hotkeys for changing the month and the year and should support grid navigation keys. 
    * https://www.disabled-world.com/assistivedevices/computer/hotkeys.php

## Examples of Accessible Date Pickers
* http://eureka2.github.io/ab-datepicker/
* http://whatsock.com/tsg/Coding%20Arena/ARIA%20Date%20Pickers/ARIA%20Date%20Picker%20(Basic)/demo.htm
* https://dequeuniversity.com/library/aria/date-pickers/sf-date-picker

## Resources
* https://axesslab.com/accessible-datepickers/
* https://www.smashingmagazine.com/2017/07/designing-perfect-date-time-picker/
* https://www.hassellinclusion.com/blog/collecting-dates-accessible/
* https://www.w3.org/TR/wai-aria-practices/examples/dialog-modal/datepicker-dialog.html

