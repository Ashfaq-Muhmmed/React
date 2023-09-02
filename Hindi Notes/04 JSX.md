
# React me JSX 

***JSX (JavaScript XML) ek JavaScript extension hai, jo React me use hota hai UI elements create karne ke liye. JSX ek XML-like syntax provide karta hai, jo JavaScript code ke saath integrate hota hai. JSX ka use karke aap React components banate hain jo UI ke different parts ko represent karte hain.***

***Yahaan ek example hai jisse use karke aap JSX ka concept samjh sakte hain:***

***Suppose aapko ek React component banana hai jise "WelcomeMessage" ke naam se define kiya ja sakta hai. Is component ka kaam ek welcome message dikhana hai. JSX ka use karke is component ko create kiya ja sakta hai:***

```jsx
import React from 'react';

// JSX ka use karke component define karna
function WelcomeMessage() {
  return (
    <div>
      <h1>Welcome to our website!</h1>
      <p>We are excited to have you here.</p>
    </div>
  );
}

export default WelcomeMessage;
```

***Is example me, `<div>`, `<h1>`, aur `<p>` tags JSX ke andar hain. In tags ko React component ke UI ka hissa banane ke liye use kiya gaya hai.***

***Ab aap is component ko apne React application me use kar sakte hain:***

```jsx
import React from 'react';
import ReactDOM from 'react-dom';
import WelcomeMessage from './WelcomeMessage';

ReactDOM.render(
  <WelcomeMessage />,
  document.getElementById('root')
);
```

***Yahan, `ReactDOM.render` function ka use kiya gaya hai jisse hum WelcomeMessage component ko render kar sakte hain.***

***Is tarike se JSX ka use React me hota hai. Ye aapko HTML-like syntax provide karta hai jisse aap easily UI elements create kar sakte hain, lekin ye ultimately JavaScript code me compile hota hai.***
