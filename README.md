A desktop GUI calculator built using Java Swing that performs basic arithmetic operations such as addition, subtraction, multiplication, and division.
It features a clean interface, basic error handling, and real-time calculations using Java’s event-driven architecture.

🚀 Features

➕ Addition, ➖ Subtraction, ✖️ Multiplication, ➗ Division

💡 Intuitive graphical user interface built with Swing

⚡ Instant calculation on operator execution

❌ Error handling for invalid input and division by zero

🔄 “Clear” button to reset the display

🧰 Tech Stack
Component	Technology
Language	Java
GUI Library	Swing
IDE	IntelliJ IDEA / Eclipse / NetBeans
⚙️ How It Works

The user enters numbers via on-screen buttons or keyboard input.

An operator (+, −, ×, ÷) is selected.

On pressing =, the result is calculated and displayed.

Pressing C resets the input/display for a new calculation.

💻 Sample Code Snippet
if (command.equals("=")) {
    num2 = Double.parseDouble(display.getText());

    switch (operator) {
        case '+':
            result = num1 + num2;
            break;
        case '-':
            result = num1 - num2;
            break;
        case '*':
            result = num1 * num2;
            break;
        case '/':
            if (num2 == 0) {
                JOptionPane.showMessageDialog(this, "Cannot divide by zero!", "Error", JOptionPane.ERROR_MESSAGE);
                return;
            }
            result = num1 / num2;
            break;
    }

    display.setText(String.valueOf(result));
}

🎯 Purpose

This project serves as a beginner-friendly introduction to building GUI applications in Java. It demonstrates core concepts such as event handling, component layout, and basic arithmetic logic within a Swing-based interface.
