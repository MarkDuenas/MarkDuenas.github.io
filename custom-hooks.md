# Custom Hooks

## Review, Research, and Discussion

### What does a component’s lifecycle refer to?

Mounting, updating and unmounting of components.

### Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect

avoids infinite loops, avoid certain re-renders when it's not needed.

### Why are functional components preferred over class components?

format is easier to write. Access to react hooks, and custome hooks. Better performance in the grand scheme of things.

### What is wrong with the following code?

```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

constant re-rendering will cause a crash because of the inifite loop in the for loop.

## Vocab

- state hook - allows use of state in a functional component.
- effect hook - allows to tap into react life cycle in a funcitonal component.
- reducer hook - can manage more complex state in a functional component.

