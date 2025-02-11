# Ruby Instance Variable Modification Bug
This repository demonstrates a subtle bug related to modifying instance variables in Ruby through accessor methods.  The code in `bug.rb` shows that directly assigning a value to an accessor method (like `my_object.value = 30`) does not update the underlying instance variable, unlike modifying it directly using `instance_variable_set`.  This behavior can be unexpected for programmers coming from other languages.
The `bugSolution.rb` file provides a corrected implementation which offers a clearer and more intuitive way to handle instance variable updates.

## How to Reproduce
1. Clone this repository.
2. Run `ruby bug.rb` to see the unexpected behavior.
3. Run `ruby bugSolution.rb` to see the corrected behavior.

This example highlights the importance of understanding Ruby's object model and how instance variables interact with accessor methods.