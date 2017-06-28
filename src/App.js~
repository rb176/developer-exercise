import React, { Component } from 'react';
import data from './data/data.json';
import './App.css';

const message = data.placements[0].message;
const products = data.placements[0].items;

class App extends Component {
  render() {
    return (
      <div className="gallery">
        <div className="gallery-header">
          <h1>{message}</h1>
        </div>
        <main className="flex-container">        		
        		 {products.map((item) => 
					<div className="flex-item" key={item.ID}>
						<a href={item.linkURL}>
							<img src={item.imageURL} alt={item.name} width="100%"/>
							<h2>{item.name}</h2>
							<span>£{item.price}</span>
						</a>			
					</div>        		 
        		 )}
        </main>
      </div>
    );
  }
}

export default App;
