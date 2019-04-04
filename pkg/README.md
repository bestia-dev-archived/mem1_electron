# mem1

Learning to use Dodrio virtual DOM on a simple memory game for kids.  
The images are funny cartoon characters from the alphabet.  
The cards grid is only 4x4.  
You can play it here:  
[https://lucianobestia.github.io/mem1_website/index.html](https://lucianobestia.github.io/mem1_website/index.html)  
The github page files are here:  
[https://github.com/LucianoBestia/mem1_website](https://github.com/LucianoBestia/mem1_website)

## Source

Absolutely everything manually coded is in Rust language in the file `/src/lib.rs`.  
No manual javascript or HTML needed.  
The index.html file is a standard scafold.  
The pkg/mem.js file is generated by wasm-bindgen.  
I prepared a small simple mem1.css with flex objects for styling.   
No need for npm or web-pack.

## Build
Run in mem1/ folder

```
wasm-pack build --target no-modules
```

## Serve

Run the html server in mem1/ folder in a second terminal.
So it can continuosly run while you incrementaly build your changes in the first terminal.

```
basic-http-server
```
If you don't have it yet on your machine, install it with:
```
cargo install basic-http-server
```
Open the default URI in your browser

[http://localhost:4000/](http://localhost:4000/)

# Memory game rules

The game starts with a grid of 8 randomly shuffled card pairs face down - 16 cards in all.  
The first player flips over two cards with two clicks.  
If the cards do not match, the next player starts his turn with a click to turn both cards back face down. Then two clicks to flip over two cards.  
If the cards match, they are left face up and the player receives a point and continues with the next turn. No additional third click needed in that case.  
This is a programming example for Rust Webassembly Virtual Dom application. 
For the sake of simplicity, it is made as for single player mode. 

# Programming references
Everything is changing fast. This situation is on 2019-04-03.  
https://doc.rust-lang.org/book/  
https://github.com/fitzgen/dodrio  
https://github.com/brson/basic-http-server    
https://rust-lang-nursery.github.io/rust-cookbook/    
https://github.com/anderejd/wasm-bindgen-minimal-example  
https://www.w3schools.com/w3css/  

Clarified the "rand" problem and solution for wasm-bindgen:  
https://medium.com/@rossharrison/generating-sudoku-boards-pt-3-rust-for-webassembly-85bd7294c34a  
In this book I didn't find a clear explanation for rand and wasm:  
https://rust-random.github.io/book/  

Images included free cartoon characters:  
https://vectorcharacters.net/alphabet-vectors/alphabet-cartoon-characters  
