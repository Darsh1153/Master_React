# Master_React

React App using React.createElement

This project shows how to create a basic React app without JSX, using React.createElement.

What this project does?

Creates a simple React element
Renders it into the browser
Displays a heading text on the screen


<img width="665" height="323" alt="Screenshot 2025-12-15 at 10 30 56 PM" src="https://github.com/user-attachments/assets/f77526d1-f24a-43f3-ba01-395b228c64c4" />

What is JSX?
JSX stands for JavaScript XML.
It is a syntax extension for JavaScript used in React that allows us to write HTML-like code inside JavaScript.

Example
<img width="542" height="81" alt="Screenshot 2025-12-15 at 10 33 46 PM" src="https://github.com/user-attachments/assets/775e7f09-613d-4b0b-9a57-f2891c7a16a1" />

What happens behind the scenes?
JSX is NOT understood by the browser.

So this JSX code: <br/>
<img width="499" height="79" alt="Screenshot 2025-12-15 at 10 34 22 PM" src="https://github.com/user-attachments/assets/bf2d1ae2-74a6-40be-8484-cdf75ca02ae3" />

is converted (compiled) into:
<img width="529" height="85" alt="Screenshot 2025-12-15 at 10 34 47 PM" src="https://github.com/user-attachments/assets/4bcd13ec-8510-4eb6-947c-85b45c4dc9a6" /> <br/>
This conversion is done by tools like Babel. <br/>
👉 JSX is just a cleaner way to write React.createElement. <br/> <br/>


# What are Hooks in React?
Hooks are special functions in React that allow functional components to:

1. Manage state
2. Use lifecycle features
3. Access other React features

Before Hooks (pre-React 16.8), these features were only available in class components.
<br/>
Hooks let you “hook into” React features from function components.

## useState Hook
What is useState?
useState is a React Hook that allows you to:
1. Create state variables
2. Update state
3. Automatically re-render the component when state changes.<br/>
<img width="643" height="651" alt="Screenshot 2025-12-16 at 11 11 01 PM" src="https://github.com/user-attachments/assets/f6887ef5-c3df-4eb5-95e9-ce0413c81961" />

<br/>
## How it Works:
Component renders with count = 0

Button click calls setCount(1)

React updates state

Component re-renders with updated value <br/>


# What is Reconciliation in React?
Reconciliation is the process by which React updates the UI when state or props change.
When something changes in your app:
React figures out what changed
React updates only those parts of the UI

<br/>
