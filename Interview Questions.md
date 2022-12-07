
## This is a collection of possible JavaScript interview questions with provided both short answers and detailed explanations. 
---
#interviewQuestions
#objects
### Q: Which are the most common ways to create an object in JS?

### *A: There are many ways to create objects in JS. The most common of them are to use:*
**Object literal syntax**, **Object.create() method**, **object constructor using "new" keyword**, **JS class syntax* 

### Details:

- Object literal syntax - a shorthand for creating objects with properties and methods
```javascript
const name = 'John Doe'
const person = {
	name: name
	greeting: function() {
		return `${this.name} says hello!`
	}
}

console.log(person.name) // John Doe
console.log(person..greering()) // John Doe says hello!
```

- Object.create() method - can be used for creating new object with specified prototype and defined properties. This way the newly created object inherits the prototype from the provided object and defines its own properties.
```javascript
const user = Object.create(person, propertiesObject)
```

- Object constructor - used for creating an object wrapper for a specific value or for creating a new empty object
```javascript
const name = new Object('John Doe') // wraps the provided string in an object

const user = new Object() // creates an empty object
```

- JS Class syntax - defining a class which is then used for creating an object from it.
```javascript
class User {
	constructor(name) {
		this.name = name
	}
	greeting () {
		return `${this.name} says hello!`
	}
}

const user = new User('John Doe')

console.log(person.name) // John Doe
console.log(person..greering()) // John Doe says hello!
```

---




