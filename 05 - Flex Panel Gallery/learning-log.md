## Flex Panels
Task to demonstrate how to use flex panels to show responsive content.

##### panels - flex container - display: flex;
sets elements vertical taking as much space as they need for words

##### panel - flex item - flex: 1;
sets so elements use all space equally

##### panel - also set as flex container - display: flex;
This sets creates a nested flex container allowing the same attributes on the individual panels.

##### flex-direction: column
words in column

##### align-content: center; && justify-content: center;
to center 

##### transform panels
    .panel > *:first-child { transform: translateY(-100%); }
    .panel.open-active > *:first-child { transform: translateY(0); }

hide some child panels by moving them off screen
on click of middle, transform them back onto screen

##### transition
not necessary but nice effect

##### JS to toggle classes
select all panels
create function that will toggle classList
addEventListener forEach panel, on click call function

function(e) {e.propertyName} - shows which transitions are ending 
if e.propertyName.includes one of the transitions, then toggle.
addEventListener on transitionend, toggleOpenActive