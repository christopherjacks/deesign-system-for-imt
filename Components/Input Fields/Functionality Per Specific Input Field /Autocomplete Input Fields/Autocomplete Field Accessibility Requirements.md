# AA Accessibility Requirements

## Suggestion List

**Where to Show Suggestions**
* If there are no suggestions, do not show a list.
* If there are suggestions, show them directly below the input field.
     * The suggestion list should also be near the input field in the code.
        <br>
        Ex: 
        <br>
        ![Suggestion_List_Code](/uploads/231e19af635fedc68e9185a1480ed641/Suggestion_List_Code.png)

**Suggestion List Container**

* Add ARIA markup - add role=“listbox“ to the suggestion list <div> to tell screen reader users it contains a list of selectable items.

**Suggestion Item**

* Add ARIA markup - add role=“option“ to each suggestion item, along with a unique id. That id is used by the aria-activedescendant attribute of the <input> element, whose value changes as users move through the list items with the arrow keys. 

## Keyboard Compatibility

**General Requirements**
* Use tab to get to the field.
* Use arrow keys to move through the suggestion list.
* Use the enter key to select an item on the list and close the list.
* Use esc to exit the suggestion list. If no selection is made, focus remains in the field.

**Active-Descendant**
* Aria-activedescendant should match the currently selected option.
    * As users move through the list items with the arrow keys, update the value of the aria-activedescendant attribute of the <input> element to contain the id of the currently highlighted list item.
* Announce the number of available suggestions to screen reader users.
    * User aria live attribute to do so

## Screen Reader Compatibility
* Must tell user that field is autocomplete.
* Use Accessible Rich Internet Applications (ARIA), a W3C technical specification. It defines HTML attributes to improve website code semantics and provide information to assistive technologies (e.g. screen readers) about non-native HTML components like our auto-suggest.
    * Add role=”combobox” to the <input> field to tell screen reader users that the input field is an auto-suggest.
    * Add aria-autocomplete=”both” to the <input> field to tell screen reader users they can select from the suggestion list or type their own input.
    * Add aria-owns to the <input> field to link the suggestion list to the input field.
    * Add aria-activedescendant to the <input> element and populate it with the id of the currently highlighted list item. The aria-activedescendant value changes as the user presses the Up and Down arrows.
    <br>
    Ex:
    <br>
    ![Autocomplete_Screen_Reader_Compatibility](/uploads/c25f4d50877fb913251df4bb7e929a8d/Autocomplete_Screen_Reader_Compatibility.png)

## Examples
* https://alphagov.github.io/accessible-autocomplete/examples/

