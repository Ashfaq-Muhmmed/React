## React me Components
**React main, "component" ek re-usable, self-contained, aur independent unit hota hai jo UI elements ko represent karta hai. React applications ko component-based architecture mein develop kiya jata hai, jisse code maintainability, reusability, aur readability improve hoti hai.**

**React components do prakar ke hote hain:**

**1.** **Functional Components:** **Ye functional programming concept par based hote hain. Ye JavaScript functions hote hain jo JSX (JavaScript XML) return karte hain. Functional components stateless hote hain, matlab ki unmein internal state nahi hota. Ye ek input (props) lete hain aur uske basis par UI render karte hain. Aap inhe "hooks" jaise useState aur useEffect ke sath use kar sakte hain.**

**Example of a functional component:**
```jsx
import React from 'react';

const FunctionalComponent = (props) => {
  return <div>Hello, {props.name}!</div>;
};

export default FunctionalComponent;
```

**2.** **Class Components:** **Ye traditional tareeka hai component definition ka, jismein ES6 classes ka use hota hai. Class components mein internal state aur lifecycle methods ka use hota hai. Ab react-hooks aane ke baad, functional components jyada popular ho gaye hain, lekin class components ka use purane projects mein ho sakta hai.**

**Example of a class component:**
```jsx
import React, { Component } from 'react';

class ClassComponent extends Component {
  render() {
    return <div>Hello, {this.props.name}!</div>;
  }
}

export default ClassComponent;
```

**Component ka use karte samay, aap unhe alag-alag components ko jodne ke liye aur complex UI ko banaane ke liye combine kar sakte hain. Isse aapke code ko modular banaya ja sakta hai, taki har component apne khud ke logic aur rendering responsibilities ke sath ho.**
