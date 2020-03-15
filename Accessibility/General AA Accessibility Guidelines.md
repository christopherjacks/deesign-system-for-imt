# Preface
The following guidelines meet the WCAG AA level standard. The additional reference numbers and names (ex: 3.1.1 Language of Page) at the end of each segment pertain to the particular section of the WCAG AA standard where more information on that specific topic can be found. The official guideline's website can be found here: https://www.w3.org/TR/WCAG21/.

<br>
These are the overall accessibility guidelines that should be followed when updating or creating new pages on InsureMyTrip's website. These are general and high level guidelines that cover accessibility standards for most components. For a more detailed accessibility guideline for each component, please visit that components individual page in the design system. 

<br>
<br>

## Language
* Add the HTML language code - [list of language codes](https://www.w3schools.com/tags/ref_language_codes.asp). 

<br>

* 3.1.1. Language of Page

<br>

## Parsing
* Ensure HTML elements have complete start ( < > ) and end ( </ > ) tags where needed.
* Use unique Ids
* No duplicate HTML attributes

<br>

* 4.1.1 Parsing

<br>

## Keyboard
* Ability to tab through fields
* Make keyboard focus visible (border/underline)
* Test third party widgets to see if they are keyboard accessible
* Add ability to bypass header and footer - use: [Skip to Content](https://github.com/paypal/skipto)

<br>

* 2.1.1. Keyboard
* 2.1.2. No Keyboard Trap
* 2.4.1 Bypass Blocks
* 2.4.7 Focus Visible

<br>

## Meaningful Sequence
* Present content in a meaningful order.
* Separate navigation menus from content.
* Turn off the site’s Cascading Style Sheet (CSS) and check that the web page 
displays in the correct order. You can use an extension like [Pendule for Chrome](url)
to easily toggle CSS on and off.

<br>

* 1.3.2 Meaningful Sequences
* 2.4.3 Focus Order

<br>

## Sensory Characteristics
* Use more than one sense for instructions

<br>

## Consistent Navigation
* Keep navigation menus in the same location on all pages.
* Present the options in navigation menus in the same order on all pages.

<br>

* 3.2.3 Consistent Navigation

<br>

## Headings
* Headings don’t need to decrease from 1 to 6 on every page, however, they must be sequential. 
* Label HTML headings correctly 
* Each page has a title - must make sense out of context

<br>

* 2.4.2 Page Titled
* 2.4.6 Headings and Labels

<br>

## Color/Contrast/Text
* Text Option 1: text is less than 18 point if not bold and less than 14 point if bold
    * There is a color contrast ratio of at least 4.5:1
* Text Option 2: text is at least 18 point if not bold and at least 14 point if bold
    * There is a color contrast ratio of at least 3:1
* User Interface Components
    * Have a contrast ratio of 3:1 
* Disabled Components
    * Do not need to follow contrast guidelines
* Instructions must not rely on color alone.

<br>

* 1.4.1 Use of Color
* 1.4.3 Contrast
* 1.4.11 Non-text Contrast

<br>

## Text Spacing
* Line height (line spacing) to at least 1.5 times the font size
* Spacing following paragraphs to at least 2 times the font size
* Letter spacing (tracking) to at least 0.12 times the font size
* Word spacing to at least 0.16 times the font size

<br>

* 1.4.12 Text Spacing

<br>

## Resize Text
* Can resize up to 200%
* Resize should not require users to scroll horizontally

<br>

* 1.4.4 Resize Text

<br>

## Links
* A links purpose should be clear from link text/surrounding content.
* If the link is an image the alt text must make link's purpose clear.
* Links with the same description point to the same place. 
* A links purpose does not have to be clear if it is ambiguous to all users.

<br>

* 2.4.4 Link Purpose

<br>

## Labels
* Label all input fields (if not using visible labels make sure to label in code).
* If a field needs a specific format give an example.
* Mark required fields with an icon and explain what the icon means before the form.

<br>

* 3.3.2 Labels or Instructions
* 2.4.6 Headings and Labels

<br>

## On Focus
* Do not open links automatically on focus.
* Do not have any automatic pop-ups on focus.
* Focus should not jump from one element to another.
* Forms do not submit without the user taking action.

<br>

* 3.2.1 On Focus

<br>

## On Input
* Focus should not automatically jump to the next field on input.

<br>

* 3.2.2. On Input

<br>

## Errors
* Use a clear visual cue.
* Do not just rely on color.
* Automatically identify and explain any mistakes.
* Explain what is wrong and how to fix it.
* If a form requires input in a certain format, show and describe the required format.
* If a mandatory field is empty, highlight the field and explain what’s required.
* Build forms to be forgiving, accepting variations on the formats you prefer.
* Provide extra help by giving your contact details on all pages.

<br>

* 1.3.3 Sensory Characteristics
* 3.3.1 Error Identification
* 3.3.3 Error Suggestion






