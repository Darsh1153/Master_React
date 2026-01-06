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

## useEffect Hook
What is useEffect in React?
<img width="730" height="503" alt="image" src="https://github.com/user-attachments/assets/f59f6bfb-2a20-4f4e-b5d7-11b02da0e8f1" />
<br/>
<img width="1470" height="1320" alt="image" src="https://github.com/user-attachments/assets/288e5073-0cb0-4c7e-88e3-e11358ac9529" /> <br/>
<img width="761" height="969" alt="image" src="https://github.com/user-attachments/assets/4c988dd7-b930-494a-9059-126088579b56" /> <br/>


<br/> <br/>

# What are Class Based Components?
Class based components are an older way of creating components in React using JavaScript classes. <br/>
They: <br/>
1. Extend React.Component
2. Have a render() method
3. Can manage state
4. Can use lifecycle methods (like componentDidMount) <br/>

Before Hooks existed, class components were the only way to use state and lifecycle logic. <br/>

<img width="592" height="324" alt="Screenshot 2026-01-06 at 1 06 52 PM" src="https://github.com/user-attachments/assets/342fea36-291b-4b3a-a766-e0cb79f5bc15" />
<br/>

### What’s happening here? <br/>
class User → creates a component <br/>
extends React.Component → inherits React features <br/>
render() → returns JSX (UI) <br/>

<br/>

## Using state in class components <br/>
### State = component’s own data
 <br/>
<img width="565" height="575" alt="Screenshot 2026-01-06 at 1 08 40 PM" src="https://github.com/user-attachments/assets/dec4fb69-1ed8-47f1-9d7c-1f3ec32cee33" />
 <br/>
 
### Important rules about state
<br/>
❌ Never modify state directly <br/>
✅ Always use this.setState() <br/>
State updates are asynchronous <br/>

<br/> <br/>

# 🌱 What are Lifecycle Methods? <br/>
Lifecycle methods are special methods in class-based components that React automatically calls at different stages of a component’s life. <br/>
👉 Just like humans: <br/>
1. Born <br/>
2. Grow <br/>
3. Die <br/>

### A React component: <br/>
1. Mounts (comes to the screen) <br/>
2. Updates (changes) <br/>
3. Unmounts (leaves the screen) <br/>

## 1. MOUNTING PHASE (Component appears first time) 
<br/>

This happens only once. <br/>
<img width="487" height="166" alt="Screenshot 2026-01-06 at 1 15 12 PM" src="https://github.com/user-attachments/assets/daaf1906-1571-433a-8759-7abcb7d039f9" /> <br/>

## 1️⃣ constructor(props) 
<br/>
### What it does: <br/>
Initializes state <br/>
Binds methods <br/>
Runs before render <br/>

### Rules: 
<br/>
Must call super(props) <br/>
Runs only once <br/>
<img width="463" height="259" alt="Screenshot 2026-01-06 at 1 16 40 PM" src="https://github.com/user-attachments/assets/10034d0b-1b54-4a31-8e22-c6d65d3f673e" />
<br/>

# 2️⃣ render() <br/>
## What it does: <br/>
Returns JSX (UI) <br/>
Pure function <br/>
Must NOT: <br/>
Call API <br/>
Modify state <br/>
Runs: <br/>
On mount <br/>
On every update <br/>

<img width="534" height="186" alt="Screenshot 2026-01-06 at 1 18 09 PM" src="https://github.com/user-attachments/assets/bd2c2dfb-5cb2-495e-bd32-cbcdf4dc7a13" /> <br/>

# 3️⃣ componentDidMount()
<br/>
## What it does:
<br/>
Runs after first render <br/>
DOM is now ready <br/>
Used for: <br/>
API calls <br/>
Timers <br/>
Subscriptions <br/>

<img width="477" height="200" alt="Screenshot 2026-01-06 at 1 19 23 PM" src="https://github.com/user-attachments/assets/78144ff3-b8fb-4011-97d8-5e1ad9d7b3f0" /> <br/>

<br/>

// import React from 'react'

// const User = () => {
//   return (
//     <div className='user-card'>
//       <h1>Name - Darshan</h1>
//       <h3>Profile - Darsh1153</h3>
//       <h3>Email - imdarshan19@gmail.com</h3>
//     </div>
//   )
// }

// export default User



import React from "react";

class UserClass extends React.Component{

    constructor(props){
        super(props);
        this.state = {
            name: "Dummy",
            login: "dummy profile",

            count: 0,
            count2: 0,
        }
        console.log("Child Constructor");
    }

    componentDidUpdate(prevProps, prevState) {
        if(this.state.count !== prevState.count){
        console.log("Called only when you update the dom");
        }
    }

    async componentDidMount(){
        // const data = await fetch("https://api.github.com/users/Darsh1153");
        // const json = await data.json();
        // this.setState({
        //     name: json.name,
        //     login: json.login,
        // })

        this.timer = setInterval(() => {
            console.log("Rendering multiple times");
        }, 1000);
    }

    componentWillUnmount() {
        clearInterval(this.timer);
        console.log("Component Unmounted");
    }


    render() {
        console.log("Child Render");
        const {name, login, count, count2} = this.state;
        return (
            <div className="user-card">
                <h1>Count - {count}</h1>
                <button onClick={() => {
                    this.setState({
                        count: this.state.count + 1,
                    })
                }}>Increase Count</button>

                <h1>{count2}</h1>
                <button onClick={() => {
                    this.setState({
                        count2: this.state.count2 - 1, 
                    })
                }}>Decrease Count</button>

                <h1>Name - {name}</h1>
                <h3>Profile - {login}</h3>
                <h3>Email - imdarshan19@gmail.com</h3>
            </div>
        )
    }
}

export default UserClass;
<br/> <br/>

# What is Lazy Loading?
<br/>
Lazy loading is a performance optimization technique where non-critical website resources (like images, videos, or code) are loaded only when they are needed, usually when a user scrolls to them or interacts with a specific part of the page, instead of all at once. <br/>

import React, {lazy, Suspense} from "react";
import ReactDOM from "react-dom/client";
import Header from "./components/Header";
import Body from "./components/Body";
import About from "./components/About";
import Contact from "./components/Contact";
import Error from "./components/Error";
import { createBrowserRouter, RouterProvider, Outlet } from "react-router";
import RestaurantMenu from "./components/RestaurantMenu";
import Shimmer from "./components/Shimmer";

const Grocery = lazy(() => import("./components/Grocery"));

const App = () => {
    return (
        <div>
            <Header />
            <Outlet />
        </div>
    )
}

const appRouter = createBrowserRouter([
    {
        path: "/",
        element: <App />,
        children: [
            {
                path: "/",
                element: <Body />
            },
            {
                path: "/about",
                element: <About />
            },
            {
                path: "/contact",
                element: <Contact />
            },
            {
                path: "/grocery",
                element: <Suspense fallback={<h1><Shimmer /></h1>}><Grocery /></Suspense>
            },
            {
                path: "/res/:resId",
                element: <RestaurantMenu />
            }
        ]
    }
])

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<RouterProvider router={appRouter} />);

<br/>
