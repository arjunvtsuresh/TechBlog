---
title: "ReactJS"
category: "React"
date: "2022-07-17 12:00:00 +09:00"
desc: "React Hooks"
thumbnail: "./images/react/react.png"
alt: "apple and shaking hands"
---

# React Hooks

![React](./images/react/react.png)

## Hooks allow function components to have access to state and other React features

### Basic Hooks in react native
```
    useState()
    useEffect()
    useContext()

```

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

### useEffect() function takes in a function which runs first before other components mounts or renders to the client

#### useEffect( function() , [options])

#### the options field are the variables or state when changed triggers the function .

# Example:


```
function Timer() {
  const [time, setTime] = useState(0);
    
  useEffect(() => {
    let interval = setInterval(() => setTime(1), 1000); 

    return () => {
      // setInterval cleared when component unmounts
      clearInterval(interval);
    }
  }, []);
}

export default Timer;

```

# Hooks in React are top level components hence they are declared at the topmost level of the function 

## To learn more check [ReactNative docs]('https://reactnative.dev/')