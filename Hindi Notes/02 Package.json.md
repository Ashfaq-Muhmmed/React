
# Package.json Kya hota hai. 
**`package.json` React me ek important file hoti hai jo ki project ke dependencies (dependencies), scripts, metadata, aur configurations ko define karti hai. Ye file aapke React application ke root directory mein hoti hai.**

**Kuch important fields `package.json` mein hote hain:**

**1.** **name: Aapke project ka naam hota hai.**

**2.** **version: Aapke project ki current version hoti hai. Ye version numbers ke format mein hoti hai (e.g., "1.0.0").**

**3.** **dependencies: Ye field aapke project ke external dependencies ko list karta hai, jaise ki aapke project ke liye zaroori modules.**

**4.** **devDependencies: Ye field development mein use hone wali dependencies ko list karta hai. Yani ke ye dependencies aapke project ke development process mein important hai, lekin production build mein nahi.**

**5.** **scripts: Ye field aapke project ke liye predefined commands ko define karta hai. For example, aap "start" command se apne development server ko chala sakte hain, "build" command se production-ready code generate kar sakte hain, aur aise hi aur bhi commands define kar sakte hain.**

**6.** **main: Ye field aapke application ka main entry point file ka naam define karta hai. Generally, React applications mein ye file `src/index.js` hoti hai.**

**7.** **repository: Is field mein aap apne project ki repository ki information specify kar sakte hain.**

**8.** **author aur license: Ye fields aapke project ke author aur license ki details ko contain karte hain.**

**9.** **description: Aap apne project ki short description is field mein add kar sakte hain.**

**Ye sirf kuch important fields hain. Ek standard `package.json` file generally kuch iss tarah ka hota hai:**

```json
{
  "name": "my-react-app",
  "version": "1.0.0",
  "description": "A simple React application",
  "dependencies": {
    "react": "^17.0.2",
    "react-dom": "^17.0.2"
  },
  "devDependencies": {
    "babel": "^7.15.0",
    "webpack": "^5.50.0"
  },
  "scripts": {
    "start": "webpack-dev-server --mode development",
    "build": "webpack --mode production"
  },
  "main": "src/index.js",
  "author": "Your Name",
  "license": "MIT"
}
```

**`package.json` ki yeh information aapke project ko maintain karne aur build process ko automate karne mein madad karti hai.**


# `package.json`Install krna 

**jab bhi ek new developer ko `package.json` install krna ho to command prompt me type kro.**
```
npm start
```
**`package.json` install ho jayega.**


