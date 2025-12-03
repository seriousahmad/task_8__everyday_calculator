# __Phase 1: Constitution__
-   _Principle 1:_ Simplicity. The calculator should be intuitive and easy to use for everyday arithmetic. The user interface will be clean and uncluttered.
  - _Principle 2:_ Accuracy. All calculations must be accurate for standard integer and floating-point arithmetic.
  - _Principle 3:_ Responsiveness. The calculator should provide immediate feedback. Keystrokes and calculations should feel instantaneous.
  - _Principle 4:_ Standard Technologies. The project will be built using plain HTML, CSS, and JavaScript, without any external frameworks, to ensure it is
  lightweight and easy to understand.
  - _Principle 5:_ Maintainability. The code will be well-structured, commented, and organized into separate files for HTML, CSS, and JavaScript to make it easy to maintain and extend.

# __Phase 2: Specification__
  __1. User Interface:__
  - Display: A single, clear display at the top of the calculator. It will show the current number being entered, and the result of calculations.
  - Buttons: A grid of buttons for the numbers 0-9, the four basic arithmetic operations (+, -, , /), a decimal point (.), an equals sign (=), and a clear button
  (C).

  - The layout will be a standard calculator layout:

  +-----------+
  
  | Display   |

  +-----------+
  
  | C  del  |
  
  | 7 8 9 / |
  
  | 4 5 6 * |
  
  | 1 2 3 - |
  
  | 0 . = + |
  
  +-----------+

  __2. Core Functionality:__
  - Input: Users can input numbers by clicking the number buttons.
  - Operations: Supports addition, subtraction, multiplication, and division.
  - Calculations: Pressing the equals (=) button will perform the calculation and display the result.
  - Clear: Pressing the clear (C) button will reset the current input and any ongoing calculation, preparing the calculator for a new problem.
  - Decimal Point: Allows for floating-point number entry.

  __3. User Interaction Flow:__
  - The user clicks number buttons to form the first number. The number appears in the display.
  - The user clicks an operator button (+, -, , /).
  - The user clicks number buttons to form the second number. This new number replaces the first in the display.
  - The user clicks the equals (=) button. The display shows the result of the operation.
  - If the user clicks another operator button instead of equals, the calculator will chain the operations (e.g., 5 * 2 + 3 will first calculate 5 * 2 = 10, then wait for the next input).


# __**Phase 3: Plan**__

  __1. _index.html_ (The Structure):__
    - Create a main container for the calculator.
    - Inside the container, add a div that will serve as the display screen.
    - Create a grid of button elements for all the numbers (0-9), operators (+, -, , /), decimal point (.), equals (=), and clear (C). Each button will have a
  unique identifier or class so our JavaScript can interact with it.

  __3. _style.css_ (The Presentation):__
    - Style the main calculator container to give it a defined shape and border.
    - Use CSS Grid to arrange the buttons into the correct layout.
    - Define the appearance of the display: font size, text alignment, background color, etc.
    - Style the buttons: size, color, font, and hover/active states for user feedback.

  __4. _script.js_ (The Logic):__
    - Initialization: When the script loads, get references to the display element and all the button elements from the HTML.
    
    - State Management: Create variables to keep track of the calculator's state:
    
      - currentOperand: The number currently being entered.
        
      - previousOperand: The first number in a calculation.
      
      - operator: The selected operation (+, -, etc.).
      
    - Event Handling: Add a single event listener to the container holding all the buttons to efficiently capture clicks.
    
    - Core Functions:
    
      - appendNumber(number): Appends a digit to the currentOperand.
        
      - chooseOperator(op): Sets the operator and moves the currentOperand to previousOperand.
      
      - calculate(): Performs the calculation based on the previousOperand, currentOperand, and operator.
      
      - clear(): Resets all state variables to their initial values.
      
      - updateDisplay(): Updates the HTML display with the current value.


# __Phase 4: Task__

    ## File: index.html
    - Task 1: Create the main HTML document structure.
    - Task 2: Add <link> for style.css and <script> for script.js.
    - Task 3: Build the calculator's body with a <div> for the grid and another for the display.
    - Task 4: Add all 16 buttons (0-9, ., +, -, *, /, =, C) inside the grid.

    ## File: style.css
    - Task 5: Center the calculator on the page.
    - Task 6: Define the CSS Grid layout for the calculator buttons.
    - Task 7: Style the calculator display area.
    - Task 8: Style the buttons, giving them a consistent look and feel.
    - Task 9: Add hover effects to the buttons for interactivity.

    ## File: script.js
    - Task 10: Get references to all the HTML button and display elements.
    - Task 11: Create variables to hold the calculator's state (current number, previous number, operator).
    - Task 12: Implement the appendNumber function to add digits to the current number.
    - Task 13: Implement the chooseOperator function to handle operator clicks.
    - Task 14: Implement the calculate function to compute the result.
    - Task 15: Implement the clear function to reset the calculator.
    - Task 16: Implement the updateDisplay function to show the current number or result on the screen.
    - Task 17: Add event listeners to all buttons to trigger the correct functions.


# __Phase 5: Implementation__

    - Define the Constitution for the calculator project 
    - Create the Specification for the calculator 
    - Develop the Plan for implementation
    - Break down the Plan into Tasks 
    - Implement the calculator 
