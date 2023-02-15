# Built-in Data Structure in JavaScript

There are 4 built-in data structures in JavaScript, and understanding their pros and cons can help in building
custom data structures and making better decisions when working with simple data structures. Let's examine the
functionality that JavaScript provides for each of these 4 data structures.

# 1: Arrays

The most common data structure for a list of data in JS is array. The abil

1. Arrays can accept any type of data.
2. Elements always are accesible via their index.
3. Arrays are iterable (can use `for...of` loop).
4. Duplicate elements are allowed.
5. The size of the array is adjusted dynamically.
6. When an item is added to an array the insertation is memorized. The location of the specific element is
   constant.
7. The cost of the finding an element can easilly grow with the size of the array.
8. Deletion an element is a costly action in array. Cause if one element is delete the position of the other
   elements are changed!

```js
// create a new array:
const arr = ["Mobina", 26, true, {}, []];

// delete an element:
arr.splice(2, 1);

// edit and access an element:
const arr[2] = 'Sport';
```

# 2: Sets

Another data structure for a list of data in JavaScript is sets. Sets have the following characteristics:

1. Elements are accesible via the method `has()`.
2. Sets are iterable (can use `for...of` loop).
3. Duplicate elements are not allowed.
4. The size of the Sets is adjusted dynamically.
5. The insertation is not memorized.
6. Since the order is not matter in Sets, The cost of the finding and deleting an element is low.
7. Deletion an element is a fast action in Sets. Cause the elements do not have position in a first place So
   they do not need change their indexs.

```js
// create a new array:
const sets = new Set();
sets.add("John");
sets.add(1);

// delete an element:
sets.delete(1);

// access an element:
sets.has("Mobina");
```

# 3: Objects

The most popular data structure in JavaScript is objects. Objects have the following characteristics:

1. Unordered key-values pairs of data.
2. Values are accesible via their keys.
3. Keys are unique, values are not.
4. Keys have to be string, number or symbols.
5. Objects can have methods in them.
6. Objects are iterable only with the for...in loop.

```js
// create a new object:
const obj = {
  name: "Mobina",
  age: 26,
  isFunny: true,
  sayHello() {
    console.log("Hello " + this.name);
  },
};

//add properties
obj.lastname = "Khalilzade";
obj["gender"] = "female";

// delete a property:
delete obj.lastname;

// access a property:
obj.age;
```

# 4: Maps

The final data structure in JavaScript is maps. Maps have the following characteristics:

1. Ordered key-value pairs of data.
2. Values are accessible via their keys.
3. Maps are iterable (can use for...of loop).
4. Keys are unique, values are not.
5. Keys can be anything, even references like arrays.

```js
// create a new object:
const data = new Map();

//add properties
data.set("sum", 10);
const obj = { name: "pizza", quantity: 20 };
data.set(obj, "food");

// delete a property:
data.delete(obj);

// access a property:
data.get("sum");
```
