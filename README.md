This is a calculator app done using HTML, CSS and Javascript
The display bar is linked to a javascript variable; 'Display' using it's id : 'display' which was formerly readonly but i later removed.
For the number and operators buttons, the onclick event triggers a javascript display function "Display(para)"
that accepts a parammeter to display in the display bar where the parameters are the value of the respective buttons
so that when these buttons are clicked, the values are shown in the display bar

While for the equal-to button, the onclick attribute triggers a function 'calculate()' that uses the javascript inbuilt evaluate function 'eval()' to evaluate the input in the display bar 
And when the input on the display bar is an expression that is not valid for evaluation, theres an error handler (try,catch) that sets the display value to 'Error'
catch(error){
display.value = 'Error'
}
The clear button (C) has an onclick attribute that triggers a javascript function clearDisplay() that sets the display value to an empty string : display.value = ""
