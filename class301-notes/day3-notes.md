# Read: Class 03

## React Docs - lists and keys

1. **What does .map() return?** It returns the data in an array by creating a new array.

2. **If I want to loop through an array and display each value in JSX, how do I do that in React?** You can use the .map() method.

3. **Each list item needs a unique ____.** key attribute.

4. **What is the purpose of a key?** It's used to know what happened if you insert, delete, or reorder items.

## The Spread Operator

1. **What is the spread operator?** It allows you to expand an array or object into a list of arguments.

2. **List 4 things that the spread operator can do.** It can expand an array or object into a list of arguments, combine two arrays, add a new item to an array, and combine two objects into one.

3. **Give an example of using the spread operator to combine two arrays.** 

4. **Give an example of using the spread operator to add a new item to an array.**

`const array1 = [1, 2];`
`const array2 = [3, 4];`

`const combinedArray = [...array1,...array2];`

5. **Give an example of using the spread operator to combine two objects into one.**

`const object1 = { name: 'todd', age: 20 };`
`const object2 = { name: 'jane', age: 20 };`

`const mergedObject = {...object1,...object2 };`

## How to Pass Functions Between Components

1. **In the video, what is the first step that the developer does to pass functions between components?** Pass the function as a prop.

2. **In your own words, what does the `handleClick` function do?** The `handleClick` function is so when you click on apply, the code works.

3. **How can you pass a method from a parent component into a child component?** create function in parent component that accepts callback that passes to child component.

4. **How does the child component invoke a method that was passed to it from a parent component?** Invoke it with the callback function.

## `Things I want to know more about`
