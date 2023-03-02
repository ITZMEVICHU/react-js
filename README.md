# react-js
React js assignment 
Answer;


import React from 'react';
import Product from './Product';

function App() {
  return (
    <div>
      <h1>My Demo Shop</h1>
      <Product 
        title="Product 1"
        price={10}
        description="First product"
      />
      <Product 
        title="Product 2"
        price={20}
        description="Second product"
      />
    </div>
  );
}

export default App;


//Then, in you Product.js file, you can access these props using the props object


import React from 'react';

function Product(props) {
  return (
    <div>
      <h2>{props.title}</h2>
      <p>Price: {props.price}</p>
      <p>Description: {props.description}</p>
    </div>
  );
}

export default Product;
