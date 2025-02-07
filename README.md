# Iteration - While loops P5JS (add to your notebook)

**While Loop**- a control structure that repeats a block of code as long as a specified condition is true.  
**Repeat Condition** - a boolean expression that tells when a block of code should be repeated.  
**Infinite loop** - a loop that repeats forever. Usually not a good thing…  
**Increment** - to increase (most commonly with addition or the `+=` symbol).  
**Decrement** - to decrease (most commonly with subtraction or the `-=` symbol). 

## Syntax
The syntax for a while loop is shown below. 
```javascript
while( repeatCondition )
{  
	// Execute this block of commands
	doThis()
	andThisOtherThing()
}
```
### Example 1 - Horizontal ellipses 
```javascript
    let x = 50;
    while(x < 400)
    { 
        ellipse(x, 200, 20, 20);
        // Increment the x variable so the repeat 
        // condition eventually becomes false.
        x = x + 100; 	
        
    }
```
**Write example 1 in your notebook and step through the code by hand.**

### Example 2 - Vertical ellipses 
```javascript
    let y = 400;
    while(y > 0)
    { 
    	ellipse(200, y, 20, 20);
        // decrement the variable
    	y = y - 100;		
    }
```

### Example 3 - Vertical lines.  
```javascript
    let x = 50;	//declare and initialize a variable
    while(x < 200)
    { 
    	line(x, 0, x, 400);
        //Increment x. += is a shortcut for x = x + 20
    	x += 20;	
    }
```

Modify the code so that the vertical lines span the entire canvas.

### Example 3 part 2
Add code to example 3 to create horizontal lines. This will require you to declare and initialize a second variable and increment that variable. The result should be graph paper with 20x20 grids.

### Example 4 - Looping a set number of times. This will draw 10 rectangles…
```javascript
    let count = 0;	//declare and initialize a counter variable
    while(count < 10)
    { 
    	rect(random(width), random(height), 10, 10);
    	count += 1;	//increment count
    }
```
What was the result? How could this be avoided?

### Example 5 - Starry sky
```javascript
    let count = 0;	//declare and initialize a counter variable
    background(0,0,0,10); //black with some transparancy
    while(count < 50)
    { 
        stroke(255);	//white
        point(random(width), random(height));
        count += 1;	//increment count
    }
```

### Example 6
```javascript
    let x = 0; 
    while (x < 400)
    {
        line(0, x, x, 400);
        x += 20;
    }
```

### Your turn
Experiment with creating while loops. **Don't forget to increment the variable so that the loop eventually ends.** 

Need ideas? 

* Use the `random` function inside a loop.
* Draw a centipede with 100 legs.
* Draw a checkerboard.
* Draw grass blades all along the bottom of the canvas.
* Draw rain falling (this one is harder). 

