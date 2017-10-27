# Iteration With Built-In Methods

We now know that an array is a list.

We encounter lists all of the time in social media. On any platform, we have a list of friends or followers and a list of people who follow us. We could put those followers into an array:
```
var friendsArray = ["Bert", "Ernie", "Big Bird", "Oscar"]
```
Go ahead and define an array called friendsArray with the names of 4 of your favorite friends.

solution:
```
var friendsArray = ["Bert", "Ernie", "Big Bird", "Oscar"]
```
What if we were feeling a little down and wanted all of our friends to comment on a new photo we posted, telling us that we are awesome? It might make us feel a little better, right?

We can do this through a process called iteration. Iteration allows us to loop through the whole array and do something to each item within it. In this case, we want to take each name in our friends array and attach it to a string: "____ says you are awesome!"

Traditionally in Javascript, we were limited to what is called a for loop to achieve this:
```
for (var i = 0; i < numberArray.length; i++) {
console.log(numberArray[i]);
}
```
This starts at index[0] and loops through the entire array.

Write a for loop to print out all of the names of the friends in our array.

solution:
```
for (var i = 0; i < friendsArray.length; i++) {
    console.log(friendsArray[i]);
}
```
As of ES5, which is supported by roughly 98% of browsers, JavaScript supplies a number of built-in methods for array iteration. We have been gifted the magical .forEach method:
```
numberArray.forEach(function(number) {
console.log(number);
});
```
This method works just as our for loop with fewer characters, reducing the risk of typos and errors. We now have a cleaner, more readable method that describes exactly what is happening in our code. For each item in our array, a function will be executed.

Go ahead and attach the .forEach method to your friendsArray and include space for a function to be defined.

solution:
```
friendsArray.forEach(function()
```
Now, we want to create a function that will take each name in the array and concatenate it with a string that will give us that self-esteem boost on social media, telling us how awesome we are.

To your friendsArray iteration, define a function called awesomeFriends that takes in an argument called friends. 

solution:
```
friendsArray.forEach(function awesomeFriends(friends)
```
Now it's time to include the self-esteem boosting string. Inside of your .forEach loop, console.log() a statement that concatenates the friends variable with a string that states " says you are awesome!"

solution:
```
friendsArray.forEach(function awesomeFriends(friends) {
    console.log (friends + " says you are awesome!")
});
```
Run the code. Receive compliments from all of your friends. Sit back and smile.

