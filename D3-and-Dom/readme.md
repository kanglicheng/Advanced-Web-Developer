## Notes on D3.js ##

### D3.select, set attributes, inner text, and style on D3 selections, chaining methods to make changes to DOM, event listeners ###

Load d3 with a script tag in the html. d3.select("li") returns d3 selections, d3,selection.nodes() returns array of matching html elements. 

Can manipulate selections by chaining methods, i.e. d2.select("li").style(property [, newValue]). d3.select("li").style("color") works as a getter since only the property name is passed in.

Using callbacks, i.e. d3.selectAll("li").style("font-size", function(_, idx){
return Math.random*40 +"px";}, where idx is the index of the element in the selection. This assigns a random font size to each li element.

Event listener example: d3.select("h1").on("click", function(){ console.log("event listeners are sweet!"); } .on method attaches and removes an event listener. d3.event.preventDefault(); 
