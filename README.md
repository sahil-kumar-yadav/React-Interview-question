# React-Interview-question


### 1. **What is React?**
   React is a JavaScript library for building user interfaces, developed by Facebook. It allows developers to create reusable UI components that manage their own state.

### 2. **What are components in React?**
   Components are the building blocks of a React application. They can be either class components or functional components and can accept inputs (props) and return React elements describing what should appear on the screen.

### 3. **What is JSX?**
   JSX (JavaScript XML) is a syntax extension for JavaScript that allows you to write HTML-like code within JavaScript. It makes the code easier to read and write.

### 4. **What is state in React?**
   State is an object that determines the behavior and rendering of a component. Unlike props, state is managed within the component and can be updated using `setState`.

### 5. **What are props?**
   Props (short for properties) are a mechanism for passing data from parent to child components. They are read-only and help in creating dynamic and reusable components.

### 6. **What is the difference between state and props?**
   - **State:** Managed within the component, mutable, can change over time.
   - **Props:** Passed from parent to child, immutable, used to pass data and event handlers.

### 7. **What are lifecycle methods in React?**
   Lifecycle methods are hooks that allow you to run code at specific points in a component's lifecycle, such as mounting, updating, and unmounting. Common lifecycle methods include `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount`.

### 8. **What is the virtual DOM?**
   The virtual DOM is a lightweight copy of the actual DOM. React uses it to optimize updates by determining which parts of the DOM need to be changed, reducing direct manipulation and improving performance.

### 9. **What are hooks in React?**
   Hooks are functions that let you use state and other React features in functional components. The most common hooks are `useState`, `useEffect`, and `useContext`.

### 10. **What is the purpose of `useEffect`?**
   `useEffect` is a hook that allows you to perform side effects in function components, such as data fetching, subscriptions, or manually changing the DOM. It runs after the render phase.

### 11. **What is context in React?**
   Context provides a way to pass data through the component tree without having to pass props down manually at every level. It’s useful for global data like themes or user authentication.

### 12. **What is a higher-order component (HOC)?**
   A higher-order component is a function that takes a component and returns a new component. HOCs are used to share common functionality or behavior among components.

### 13. **What is React Router?**
   React Router is a library for routing in React applications. It allows you to define multiple routes in your application and navigate between them without reloading the page.

### 14. **What are controlled and uncontrolled components?**
   - **Controlled components:** Form data is handled by the component's state.
   - **Uncontrolled components:** Form data is handled by the DOM itself.

### 15. **How do you optimize performance in a React app?**
   Common techniques include:
   - Code splitting with React.lazy and Suspense.
   - Memoization with React.memo and useMemo.
   - Avoiding unnecessary re-renders with shouldComponentUpdate or React.PureComponent.
   - Lazy loading images and components.

### 16. **What is Redux?**
   Redux is a state management library for JavaScript applications. It provides a centralized store for application state, making it easier to manage and debug state changes.

### 17. **What is the purpose of `React.memo`?**
   `React.memo` is a higher-order component that optimizes functional components by memoizing the rendered output. It prevents unnecessary re-renders when props haven’t changed.

### 18. **What is the difference between `useMemo` and `useCallback`?**
   - **useMemo:** Returns a memoized value. It’s used to optimize expensive calculations.
   - **useCallback:** Returns a memoized function. It’s used to optimize performance by preventing the creation of new function instances on every render.

### 19. **What are error boundaries?**
   Error boundaries are React components that catch JavaScript errors in their child component tree, log those errors, and display a fallback UI instead of crashing the whole application.

### 20. **What is the use of `key` in React lists?**
   The `key` prop is used to uniquely identify elements in a list. It helps React optimize rendering by allowing it to determine which items have changed, been added, or removed.

Absolutely! Here are some additional React interview questions to further enhance your README:

### 21. **What is the difference between a class component and a functional component?**
   - **Class Component:** A traditional way to create components using ES6 classes. It can manage state and lifecycle methods.
   - **Functional Component:** A simpler way to create components using functions. With the introduction of hooks, functional components can now manage state and side effects.

### 22. **What are fragments in React?**
   Fragments allow you to group multiple elements without adding extra nodes to the DOM. They can be used with `<React.Fragment>` or the shorthand syntax `<>...</>`.

### 23. **What is the purpose of `useReducer`?**
   `useReducer` is a hook that helps manage complex state logic in functional components. It is similar to Redux but built into React. It’s useful for managing state transitions based on actions.

### 24. **What are default props in React?**
   Default props are values that are set for props if no value is provided. They can be defined using the `defaultProps` property on the component.

### 25. **What is prop drilling?**
   Prop drilling refers to the process of passing data from a higher-level component down to deeply nested child components through props, which can lead to cumbersome code.

### 26. **What is the significance of keys in React?**
   Keys help React identify which items in a list have changed, been added, or removed. They should be unique and stable to help maintain component state correctly.

### 27. **What is the difference between `useEffect` with an empty dependency array and no dependency array?**
   - **Empty Dependency Array:** `useEffect` runs only once after the initial render (like `componentDidMount`).
   - **No Dependency Array:** `useEffect` runs after every render (like `componentDidUpdate`).

### 28. **What is server-side rendering (SSR) in React?**
   Server-side rendering is the process of rendering React components on the server and sending the fully rendered HTML to the client. This can improve performance and SEO.

### 29. **What is the purpose of `React.StrictMode`?**
   `React.StrictMode` is a tool for highlighting potential problems in an application. It activates additional checks and warnings for its descendants, helping identify unsafe lifecycles and other issues.

### 30. **What is a render prop?**
   A render prop is a technique for sharing code between components using a prop that is a function. This function returns a React element and allows for dynamic rendering based on the provided data.

### 31. **What is the purpose of `useContext`?**
   `useContext` is a hook that allows you to access the value of a context directly within functional components, simplifying the consumption of context without the need for a `Consumer` component.

### 32. **How can you handle forms in React?**
   Forms can be handled using controlled components (where form data is managed by React state) or uncontrolled components (where form data is managed by the DOM). You can use hooks like `useState` to manage form input values.

### 33. **What is the purpose of `React.lazy`?**
   `React.lazy` is a function that enables dynamic import of components, allowing you to split your code into smaller chunks that can be loaded on demand, improving the initial load time of your application.

### 34. **What is the difference between synchronous and asynchronous setState?**
   The `setState` function is asynchronous in React. This means that calling `setState` doesn’t immediately update the state; instead, it schedules an update, and the state is updated on the next render.

### 35. **What are some common performance optimization techniques in React?**
   - Use React.memo for functional components.
   - Use PureComponent for class components.
   - Implement lazy loading for components and routes.
   - Use useMemo and useCallback for memoizing values and functions.

### 36. **What is the purpose of `useLayoutEffect`?**
   `useLayoutEffect` is similar to `useEffect`, but it runs synchronously after all DOM mutations. This is useful for reading layout and synchronously re-rendering.

### 37. **How do you test React components?**
   React components can be tested using tools like Jest and React Testing Library. These tools allow you to simulate user interactions and assert that the UI behaves as expected.

### 38. **What is code splitting in React?**
   Code splitting is a technique that allows you to split your code into smaller bundles that can be loaded on demand, reducing the initial load time of your application. This can be done using dynamic `import()` or libraries like React Loadable.

### 39. **What are the common types of errors in React?**
   Common errors include rendering errors, incorrect state management, prop type validation errors, and lifecycle method issues. Using error boundaries can help catch and handle these errors gracefully.

### 40. **What is the use of `shouldComponentUpdate`?**
   `shouldComponentUpdate` is a lifecycle method that allows you to control whether a component should re-render or not based on changes in props or state, improving performance by avoiding unnecessary updates.


### 41. **What is a composite component?**
   A composite component is a React component that is made up of other components. It typically manages the state and behavior for its child components, allowing for more complex UIs.

### 42. **What is the purpose of `useImperativeHandle`?**
   `useImperativeHandle` is a hook that customizes the instance value that is exposed when using `ref`. It is often used with `forwardRef` to allow parent components to interact with child component methods.

### 43. **What are custom hooks?**
   Custom hooks are JavaScript functions that start with `use` and can call other hooks. They allow you to extract component logic into reusable functions.

### 44. **How does React handle forms with validation?**
   Forms can be handled using controlled components along with validation libraries (like Formik or React Hook Form) to manage form state and validate inputs easily.

### 45. **What is `React.memo` and how does it work?**
   `React.memo` is a higher-order component that memoizes a component's rendered output. It only re-renders the component if its props change, improving performance by avoiding unnecessary re-renders.

### 46. **What are the limitations of `useEffect`?**
   - It does not run during server-side rendering.
   - It cannot be called conditionally or inside loops.
   - Cleanup functions need to be handled carefully to avoid memory leaks.

### 47. **What is the purpose of `React.createContext`?**
   `React.createContext` is used to create a Context object, which can be used to provide and consume data without prop drilling. It helps manage global state across the component tree.

### 48. **What is the purpose of `forwardRef`?**
   `forwardRef` is a higher-order component that allows you to forward refs to a child component. This is useful when you want a parent component to access a child’s DOM node or instance.

### 49. **What are higher-order components (HOCs) used for?**
   HOCs are used to reuse component logic. They can add functionality to existing components, such as data fetching, conditional rendering, or wrapping components with additional props.

### 50. **What is the significance of `setState` in React?**
   `setState` is used to update the component's state and trigger a re-render. It accepts either an object or a function and may be asynchronous, which is important to consider when relying on previous state values.

### 51. **What is the purpose of `useDebugValue`?**
   `useDebugValue` is a hook that allows you to display a label in React DevTools for custom hooks. It can be helpful for debugging the state and behavior of custom hooks.

### 52. **What are React Portals?**
   Portals provide a way to render children into a DOM node that exists outside the hierarchy of the parent component. They are useful for modals, tooltips, and overlays.

### 53. **How can you manage global state in React?**
   Global state can be managed using context, Redux, MobX, or other state management libraries. Each approach has its trade-offs regarding complexity and performance.

### 54. **What is the `useRef` hook used for?**
   The `useRef` hook is used to create a mutable ref object that persists for the full lifetime of the component. It can be used to access DOM elements directly or store mutable values without triggering re-renders.

### 55. **What is the purpose of the `keyExtractor` prop in React Native?**
   In React Native, the `keyExtractor` prop is used to extract unique keys for each item in a list, helping React efficiently update the UI when items change.

### 56. **What is a thunk middleware in Redux?**
   Thunk middleware allows you to write action creators that return a function instead of an action. This enables you to perform asynchronous operations in Redux, such as API calls.

### 57. **What are the differences between Redux and Context API?**
   - **Redux:** Centralized state management, middleware support, and debugging capabilities.
   - **Context API:** Simpler, less overhead, suitable for lightweight state management.

### 58. **What are some common performance pitfalls in React?**
   - Unnecessary re-renders.
   - Large component trees.
   - Not using memoization for expensive calculations.
   - Using inline functions and objects in render methods.

### 59. **What is the purpose of `React.lazy` and `Suspense`?**
   `React.lazy` allows you to dynamically import components, while `Suspense` allows you to handle loading states for these components. Together, they enable code splitting and improved load performance.

### 60. **What is `useEffect` cleanup function?**
   The cleanup function in `useEffect` is a function returned by the effect callback. It runs before the effect re-executes and when the component unmounts, allowing you to clean up resources like subscriptions or timers.

### 61. **What is the difference between `componentDidMount` and `useEffect`?**
   - **componentDidMount:** A lifecycle method for class components that runs once after the component mounts.
   - **useEffect:** A hook for functional components that can run after every render or conditionally, depending on the dependency array.

### 62. **What are synthetic events in React?**
   Synthetic events are React’s cross-browser wrapper around the browser’s native events. They provide a consistent API for handling events across different browsers.

### 63. **How do you handle error boundaries in React?**
   Error boundaries are React components that catch JavaScript errors in their child component tree, log the errors, and render a fallback UI. They are implemented using the `componentDidCatch` lifecycle method.

### 64. **What is the purpose of `React.StrictMode`?**
   `React.StrictMode` is a tool for highlighting potential problems in an application. It activates additional checks and warnings for its descendants during development.

### 65. **What is a controlled vs. uncontrolled component in forms?**
   - **Controlled Component:** Form data is managed by React state, making it predictable.
   - **Uncontrolled Component:** Form data is managed by the DOM, and you use refs to access input values.

### 66. **What is the difference between `useEffect` and `useLayoutEffect`?**
   - **useEffect:** Runs after the DOM has been painted and is suitable for side effects that don't require immediate updates.
   - **useLayoutEffect:** Runs synchronously after all DOM mutations, allowing for reading layout and synchronously re-rendering.

### 67. **How do you pass data between sibling components?**
   Data can be passed between sibling components by lifting the state up to the nearest common ancestor and then passing it down as props.

### 68. **What is the purpose of `useCallback`?**
   `useCallback` is a hook that returns a memoized version of a callback function, preventing unnecessary re-creations of functions during re-renders, which can help with performance optimizations.

### 69. **What is the significance of the `propTypes` package?**
   `propTypes` is a package that allows you to validate the props that a component receives. It helps catch bugs by ensuring that components are used with the correct data types.

### 70. **How do you optimize rendering performance in large lists?**
   You can optimize rendering performance by using techniques like:
   - **Windowing:** Rendering only the visible items in a list (e.g., using libraries like `react-window` or `react-virtualized`).
   - **Memoization:** Using `React.memo` to prevent unnecessary re-renders.
   - **Key Prop:** Ensuring that each item in the list has a unique `key` prop.

### 71. **What is `ReactDOMServer`?**
   `ReactDOMServer` is a package that enables server-side rendering of React components, allowing you to render components to static markup on the server, which can improve performance and SEO.

### 72. **What are render props and when would you use them?**
   Render props is a pattern for sharing code between components using a prop that is a function. This allows for greater flexibility in rendering logic and component composition.

### 73. **What is the purpose of `getDerivedStateFromProps`?**
   `getDerivedStateFromProps` is a lifecycle method that allows you to update state based on changes in props. It is invoked before rendering and can be used to synchronize state with props.

### 74. **What is the difference between `setState` and `forceUpdate`?**
   - **setState:** Schedules an update to the component’s state and triggers a re-render.
   - **forceUpdate:** Forces a re-render of the component without changing the state.

### 75. **What are hooks rules?**
   The rules for using hooks include:
   - Only call hooks at the top level (do not call them inside loops, conditions, or nested functions).
   - Only call hooks from React function components or custom hooks.

### 76. **What are the benefits of using TypeScript with React?**
   TypeScript provides static type checking, which helps catch errors early, improves code documentation through types, and enhances developer experience with better autocompletion and refactoring tools.

### 77. **What is the role of `useReducer` in state management?**
   `useReducer` is a hook used for managing complex state logic in functional components. It allows you to manage state transitions based on dispatched actions, similar to how Redux works.

### 78. **How do you manage side effects in a React application?**
   Side effects can be managed using the `useEffect` hook, where you can perform tasks like data fetching, subscriptions, or DOM manipulation.

### 79. **What is the significance of `useEffect` cleanup function?**
   The cleanup function in `useEffect` is used to clean up resources (like subscriptions or timers) when the component unmounts or before the effect re-runs, preventing memory leaks.

### 80. **How do you handle component state with multiple fields?**
   You can manage component state with multiple fields using an object to group related fields together, or by using multiple `useState` calls. It's also common to use libraries like Formik or React Hook Form for more complex forms.

Certainly! Here are some popular and frequently asked questions about React performance and comparisons with other frameworks and libraries:

### React Performance Questions

### 81. **What are some strategies for optimizing React application performance?**
   - **Code Splitting:** Use `React.lazy` and `Suspense` to load components on demand.
   - **Memoization:** Utilize `React.memo`, `useMemo`, and `useCallback` to prevent unnecessary re-renders.
   - **Virtualization:** Implement libraries like `react-window` or `react-virtualized` to render only visible items in long lists.
   - **Avoid Inline Functions:** Define functions outside of the render method to prevent re-creation on each render.
   - **Optimize Context Usage:** Be cautious with context to prevent unnecessary re-renders of consumers.

### 82. **What is the significance of the `key` prop in React performance?**
   The `key` prop helps React identify which items have changed, are added, or are removed. Using stable, unique keys improves the efficiency of updates and minimizes the number of re-renders.

### 83. **How does React's reconciliation algorithm improve performance?**
   React's reconciliation algorithm efficiently updates the DOM by using a virtual DOM to determine the minimum number of changes needed. It compares the new virtual DOM tree with the previous one, reducing direct DOM manipulation.

### 84. **What is the role of `shouldComponentUpdate` in performance optimization?**
   `shouldComponentUpdate` allows you to control whether a component should re-render based on changes in props or state, enabling performance optimizations by preventing unnecessary updates.

### 85. **What is the difference between class components and functional components in terms of performance?**
   Functional components, especially when optimized with hooks like `useMemo` and `useCallback`, can lead to better performance due to their simpler structure and ability to leverage React's optimization techniques.

### 86. **How can you measure performance in a React application?**
   You can use tools like the React Profiler, Chrome DevTools, and Lighthouse to measure performance. The React Profiler helps identify performance bottlenecks and optimize rendering behavior.

### 87. **What is the importance of `React.PureComponent`?**
   `React.PureComponent` is a base class for class components that implements a shallow comparison of props and state, preventing unnecessary re-renders for components that receive the same data.

### 88. **How does lazy loading improve performance in React?**
   Lazy loading allows you to load components only when they are needed, reducing the initial load time and improving the overall performance of the application.

### 89. **What is the impact of heavy rendering on performance?**
   Heavy rendering can lead to increased load times and sluggish user experience. Techniques like code splitting, memoization, and avoiding large component trees can mitigate these issues.

### 90. **How can you optimize image loading in a React application?**
   Techniques include using lazy loading for images, optimizing image sizes, and serving responsive images based on device capabilities. Libraries like `react-lazyload` can help with lazy loading.


### Comparisons with Other Frameworks and Libraries

### 91. **How does React compare to Angular in terms of performance?**
   - **React:** Uses a virtual DOM for efficient updates and is generally faster for rendering dynamic content.
   - **Angular:** Uses a real DOM, which can be slower for complex UIs, but has built-in optimizations like change detection.

### 92. **What are the differences between React and Vue.js regarding performance?**
   - **React:** Utilizes a virtual DOM and can be optimized with memoization and lazy loading.
   - **Vue.js:** Also uses a virtual DOM but provides more built-in optimization techniques and reactivity that may lead to easier performance tuning.

### 93. **How does React's approach to state management compare to Redux?**
   - **React:** Uses local state and Context API for simple state management.
   - **Redux:** Centralizes state management, which can simplify debugging but adds complexity. Performance may be impacted by large state trees unless optimized.

### 94. **How do React and Svelte compare in terms of performance?**
   - **React:** Uses a virtual DOM and has a more extensive ecosystem and community support.
   - **Svelte:** Compiles to optimized vanilla JavaScript, leading to faster runtime performance with less overhead.

### 95. **What are the advantages of using React over jQuery for building web applications?**
   - **React:** Promotes a component-based architecture, making it easier to manage UI complexity and state.
   - **jQuery:** Primarily focuses on DOM manipulation and lacks built-in support for component reusability and state management.

### 96. **How does React Native compare to Flutter in terms of performance?**
   - **React Native:** Leverages native components and bridges between JavaScript and native code, leading to good performance but may require native modules for complex features.
   - **Flutter:** Compiles to native code, offering high performance and consistency across platforms, but has a steeper learning curve.

### 97. **What performance optimizations are unique to React?**
   React's unique optimizations include:
   - Reconciliation and the virtual DOM.
   - Hooks for local component state management.
   - Context API for efficient prop drilling avoidance.

### 98. **How does server-side rendering (SSR) affect React performance compared to client-side rendering (CSR)?**
   SSR can improve initial load performance and SEO by rendering content on the server. However, CSR may provide a more dynamic experience once the initial load is complete.

### 99. **How do you handle large datasets in React compared to other libraries?**
   - **React:** Use libraries like `react-window` or `react-virtualized` for efficient rendering of large lists.
   - **Other Libraries:** Some may have built-in virtual scrolling or pagination features, but React's flexibility allows for more customized solutions.

### 100. **How does React's learning curve compare to other frameworks?**
   React has a moderate learning curve, primarily due to its component-based architecture and JSX syntax. While some find it easier to grasp than Angular's complexity, others may find Vue.js simpler to start with.

# bonus questions:

### 1. **What is hoisting in JavaScript?**
   Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their containing scope during the compilation phase. This means you can use variables and functions before they are declared in the code.

### 2. **How does it work?**
   During hoisting, only the declarations are hoisted, not the initializations. For example:
   ```javascript
   console.log(myVar); // undefined
   var myVar = 5;
   ```
   Here, `myVar` is hoisted but not initialized, leading to `undefined`.

### 3. **What is the difference between `let` and `var`?**
   - **Scope:** `var` is function-scoped, while `let` is block-scoped.
   - **Hoisting:** `var` declarations are hoisted and initialized to `undefined`, while `let` declarations are hoisted but not initialized, leading to a "temporal dead zone" until they are declared.

### 4. **What is the Event Loop?**
   The Event Loop is a mechanism that allows JavaScript to perform non-blocking I/O operations despite being single-threaded. It continuously checks the call stack and the message queue, executing tasks as the call stack becomes empty.

### 5. **What is precedence in the Event Loop?**
   Precedence in the Event Loop refers to the order in which the event loop processes tasks. It processes all synchronous code first (in the call stack) before moving on to the asynchronous tasks in the message queue, ensuring that microtasks (like promises) are processed before macrotasks (like setTimeout).

### 6. **What is the difference between `setTimeout` and `setInterval`?**
   - **setTimeout:** Executes a function after a specified delay once.
   - **setInterval:** Repeatedly executes a function at specified intervals until cleared.

### 7. **Where do you use the Rest Operator?**
   The Rest Operator (`...`) is used to collect multiple elements into a single array. It can be used in function parameters to gather remaining arguments:
   ```javascript
   function sum(...args) {
       return args.reduce((acc, curr) => acc + curr, 0);
   }
   ```

### 8. **Have you heard of `array.reverse`?**
   Yes, `array.reverse()` is a built-in method in JavaScript that reverses the elements of an array in place and returns the reversed array.

### 9. **What is meant by Shallow copy and Deep copy?**
   - **Shallow Copy:** Creates a new object, but nested objects are still referenced. Changes in nested objects affect both the original and copied objects.
   - **Deep Copy:** Creates a new object and recursively copies all nested objects, ensuring that changes do not affect the original.

### 10. **What are Closures?**
   A closure is a function that retains access to its lexical scope even when the function is executed outside that scope. It allows for data encapsulation and privacy.

### 11. **Have you used the `reduce` function in JavaScript?**
   Yes, the `reduce` function is used to iterate over an array, accumulating a single value based on a callback function:
   ```javascript
   const sum = [1, 2, 3].reduce((acc, curr) => acc + curr, 0); // 6
   ```

### 12. **What is the difference between `map` and `reduce`?**
   - **map:** Transforms each element of an array and returns a new array of the same length.
   - **reduce:** Accumulates a single value from an array by applying a function across all elements.

### 13. **What parameters does the `map` function accept?**
   The `map` function accepts a callback function and an optional `thisArg`. The callback receives three parameters: the current element, the index, and the original array.

### 14. **What is the difference between a Promise and a Callback?**
   - **Promise:** Represents an asynchronous operation that can complete in the future, allowing chaining with `.then()` and `.catch()`.
   - **Callback:** A function passed as an argument to another function, which can lead to callback hell if not managed properly.

### 15. **What position attributes in CSS have you used?**
   The position attributes include `static`, `relative`, `absolute`, `fixed`, and `sticky`.

### 16. **What is the difference between them?**
   - **static:** Default positioning; elements are positioned according to the normal flow.
   - **relative:** Positioned relative to its normal position.
   - **absolute:** Positioned relative to the nearest positioned ancestor (not static).
   - **fixed:** Positioned relative to the viewport; remains fixed during scrolling.
   - **sticky:** Switches between relative and fixed based on the scroll position.

### 17. **What is Flexbox?**
   Flexbox is a CSS layout module that allows for the design of complex layouts with ease. It provides a more efficient way to lay out, align, and distribute space among items in a container, even when their size is unknown.

### 18. **What is the difference between `display: none` and `visibility: hidden`?**
   - **display: none:** The element is removed from the document flow, and it does not take up space.
   - **visibility: hidden:** The element is not visible but still takes up space in the document flow.

### 19. **What Hooks have you used?**
   Commonly used hooks include `useState`, `useEffect`, `useContext`, `useReducer`, `useRef`, and `useMemo`.

### 20. **What is the purpose of `useCallback`?**
   `useCallback` is a hook that returns a memoized version of a callback function, helping to optimize performance by preventing unnecessary re-creations of functions on re-renders.

### 21. **What are Class-based Lifecycle methods?**
   Class-based lifecycle methods are special methods in React that allow you to hook into specific moments of a component's lifecycle, including `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount`.

### 22. **How can you achieve `componentDidMount`, `componentDidUpdate`, and `componentDidUnmount` in a functional component?**
   These can be achieved using the `useEffect` hook:
   ```javascript
   useEffect(() => {
       // componentDidMount
       return () => {
           // componentDidUnmount
       };
   }, []); // Runs once

   useEffect(() => {
       // componentDidUpdate
   }, [dependencies]); // Runs on dependency change
   ```

### 23. **What are Pure Components and their purpose?**
   Pure Components are components that implement `shouldComponentUpdate` with a shallow prop and state comparison. They help optimize performance by preventing unnecessary re-renders.

### 24. **What are Higher Order Components (HOCs)?**
   HOCs are functions that take a component and return a new component, enabling the reuse of component logic. They are often used for cross-cutting concerns like authentication, logging, or data fetching.

### 25. **What HOCs have you used?**
   Common HOCs include `withRouter` (from React Router), `connect` (from Redux), and custom HOCs for logging or data fetching.

### 26. **Have you used the Context API?**
   Yes, the Context API is used for managing global state and avoiding prop drilling. It provides a way to share values between components without passing props explicitly.

### 27. **You already have state management in React, so why go for Redux?**
   Redux provides a centralized store for managing state, making it easier to handle complex state logic, share state across components, and enable features like time-travel debugging and middleware.

### 28. **How does Redux work?**
   Redux follows a unidirectional data flow where:
   - Actions are dispatched to modify the state.
   - Reducers handle these actions and return the new state.
   - The store holds the application state, which components can subscribe to.

### 29. **Have you used any Middlewares?**
   Yes, commonly used middlewares include `redux-thunk` for handling asynchronous actions and `redux-saga` for managing side effects.

### 30. **What is the purpose of using middlewares?**
   Middlewares in Redux allow you to intercept actions before they reach the reducer. They are useful for logging, handling asynchronous actions, and modifying actions or the dispatch process.

