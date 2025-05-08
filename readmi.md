<h1>Welcome to Personal Coding Solving Blog</h1>
<h2>Source  Link : https://github.com/devsamim/B5-L2-ASSIGNMENT-01</h2>
<p>Welcome to some Problem solving blog!</p>
<div>
 <h3>What are some differences between interfaces and types in TypeScript?</h3>
 <p>"<u>Interface</u> is a feature in TypeScript that helps define the structure of an object or an array. With interfaces, we can inherit properties from other objects using the extends keyword. Interfaces can also be implemented by classes. In short, interfaces help create a shape or blueprint for objects. When multiple interfaces are extended, they get merged together.</p>
  <p>"The type keyword is a feature in TypeScript that can be used to define not just objects, but also unions, intersections, tuples, and functions. Multiple types can be combined within a single type using intersection (&). Unlike interfaces, types cannot be redefined using the same name multiple times—doing so will result in an error. Additionally, types cannot be directly implemented by classes."</p>
  <ul>
  <h1>What is the use of the keyof keyword in TypeScript? Provide an example.</h1>
  <p>In TypeScript, using the keyof keyword, we can extract all the keys of an object and return them as a union type. These keys are treated as string literal unions, which increases type safety.

This means that whenever we pass a value or access a property, we can define exactly what type it should be. As a result, TypeScript will not allow any incorrect type to be used, providing a layer of protection during development.

In addition, this makes our code more reusable, as the same logic or function can be applied to different objects while still maintaining strict type rules.</p>

 <li>Example  </li>
 <p>
 function printProperty<T>(obj: T, key: keyof T) {
  console.log(`Value: ${obj[key]}`);
}
</p>

<p>const book = { id: 1, title: "Learn TypeScript", price: 499 }; </p>

<p>printProperty(book, "title"); // Output: Learn TypeScript</p>

 </ul>
</div>
