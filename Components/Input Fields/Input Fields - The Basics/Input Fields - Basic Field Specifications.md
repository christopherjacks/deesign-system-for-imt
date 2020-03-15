# Field Redlines
* https://app.axure.cloud/app/project/jmtdmo/overview

# Specifications

**The Basics**
* On focus, on mobile, the fields move based on the phones native functionality.
* A user is able to add spaces after entering information into an input field. 

**Height**
* 48px (57px on homepage)
    
**Width**
* Input widths correlate with the width of the input text (ex: smaller fields for age, date, trip cost). 
* On mobile, the largest input fields expand to the full width of the screen.
    * This does not occur with smaller fields: age, age of other travelers, and total trip cost.

**Padding** 
* 16px of padding to the left of the placeholder text/calendar icon and 16px of padding to the right of the error icon
* 17px of padding to the left of help text and error message for the resting and completed state and 18px of padding to the left of help text and error message for the focus and error state.
	* The numbers may look off, but everything should line up. The measurements take into account the fields border thickness 
* 10px of padding between the label and input field and between the input field and help text  

# States 

**Resting**
* Black outline with placeholder text
* This is the input field's resting state.

![Resting_State](/uploads/84e40588a6e389f3655192a1f038ad25/Resting_State.png)

**On Focus**
* Blue outline with blue shadow and placeholder text
* This state occurs when a user clicks or tabs into a field.

![On_Focus](/uploads/11fed152d40985e303a353de76184713/On_Focus.png)

**Completed**
* Black outline with black text
* This state occurs after a user has entered information into the field and clicks out of the field.
	* The entered information must have also passed any validations. 

![Completed_State](/uploads/05cf13732ddac5ef3ed404da132e90c7/Completed_State.png)
    
**Error**
* Red outline, red error symbol, and red error message
* The error state occurs when a user has entered invaid information.
* The error state is shown as soon a user has clicked or tabbed out of the field with the invalid information. 

![Error_State](/uploads/3b403649c0742851c2886758e790e2b8/Error_State.png)


