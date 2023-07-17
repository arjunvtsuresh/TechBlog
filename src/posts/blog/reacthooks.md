---
title: "ReactJS"
category: "Programming"
date: "2022-07-17 12:00:00 +09:00"
desc: "Create Your First Angular Project"
thumbnail: "./images/react/react.png"
alt: "apple and shaking hands"
---

# React Hooks

![React](./images/react/react.png)

## Hooks allow function components to have access to state and other React features

### Basic Hooks in react native
```
    >useState()
    >useEffect()
    >useContext()

```

# useState()

### useState() function allows functional component to manage state of the application based on the changes or updation of state we can render the new changes 

### Example in React Native: 

```
    import {useState} from react;

    const examplefunction = ()=>{
        const [count , setCount ]= useState(0);
        const handlepress = ()=>{
            setCount(count+1);
        }
        render(
               <Button onPress={handlepress}>
               <Button /> 
        )
    }

    export default examplefunction;

```

