
# State in React



React me, "state" ek important concept hai jo component ke data ko store karne aur update karne ke liye use hota hai. State, components ke internal data ko maintain karne mein madadgar hota hai. Jab state main koi change hota hai, React component automatically re-render hota hai, jisse UI update hoti hai.

React me, states ko class components mein aur functional components mein dono mein use kiya ja sakta hai. Lekin functional components me "useState" hook ka use hota hai state ko manage karne ke liye.

Ek simple example dekhte hain jahan hum ek counter component banayenge jise hum state ka use karke badha sakte hain:

Functional Component mein State ka use:

```jsx
import React, { useState } from 'react';

function Counter() {
  // 'count' state ko initialize karte hain aur ek function 'setCount' bhi milta hai, jo is state ko update karne ke liye use hota hai
  const [count, setCount] = useState(0);

  const increment = () => {
    // 'setCount' function ka use karke 'count' state ko ek se badhakar kar dete hain
    setCount(count + 1);
  };

  const decrement = () => {
    // 'setCount' function ka use karke 'count' state ko ek se kam kar dete hain
    setCount(count - 1);
  };

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={increment}>Increment</button>
      <button onClick={decrement}>Decrement</button>
    </div>
  );
}

export default Counter;
```

Is example mein, humne `useState` hook ka use kiya hai state ko initialize karne ke liye. `count` state ko increment aur decrement karne ke liye `setCount` function ka use kiya gaya hai. Jab bhi hum button par click karte hain, component re-render hota hai aur `count` state update hoti hai, jisse UI me count ka badlav dikhaya jata hai.

Is tarah se, React me state ka use karke components ko dynamic aur interactive bana sakte hain.
