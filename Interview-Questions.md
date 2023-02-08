



Hi all good morning/afternoon/evening, I am Usman Shaikh and I am 26 years old. I completed my graduation from mumbai university.
Regarding my work profile i am having a total of 5.5 yr experience. I started as a forntend developer working on technoligic like Angular, Ionic and React My reponsiblities are creating template, components consuming resfulAPI and from last two year I have started working on backend MEAN and MERN stack tecnhonllogic.

-----------------------------------------------------------------------------------------------

Type Coercion
Type coercion is the automatic or implicit conversion of values from one data type to another (such as strings to numbers). 

const value1 = '10';
const value2 = 20;

let sum = Number(value1) + value2;

console.log(sum);

-----------------------------------------------------------------------------------------------


1. Pure Functions & “higher-order function

A Pure Function is a function (a block of code) that always returns the same result if the same arguments are passed.

A Higher order function is a function that accepts functions as parameters and/or returns a function.

const numbers = [1, 2, 4];
const doubles = numbers.map((number) => 2 * number );
doubles; // [2, 4, 8]

-----------------------------------------------------------------------------------------------

2. primitive and non-primitive
seven primitive data types - Number, String, Boolean, NULL, Undefined, Symbol & bigint  .
non-primitive data type - object.

-----------------------------------------------------------------------------------------------

JavaScript Operators

Aritmetic Operators
Assignment Operators
Comparison Operators
Logical Operators
Conditional Operators
Type Operators

-----------------------------------------------------------------------------------------------

1. Determine the largest and the smallest element of an array which is not sorted.

const numbers = [2, 4, 9, 2, 0, 16, 24];

const smallest_number = Math.min(...numbers);
const largest_number = Math.max(...numbers);

console.log('smallest_number: ' + smallest_number);
console.log('largest_number: ' + largest_number);

      OR 

var sorted = numbers.sort((a, b) => a - b);

console.log('smallest_number: ' + sorted[0]);
console.log('largest_number: ' + sorted[sorted.length - 1]);

-----------------------------------------------------------------------------------------------

2. Print missing number in a given integer array of 1 to 100

const numbers = [1, 3, 4, 5, 7, 8];

const n = Math.max(...numbers);  // get the maximum
let result = [];
for (var i=1 ; i<n ; i++) {
    if (numbers.indexOf(i) < 0) result.push(i)
}

console.log(result);

-----------------------------------------------------------------------------------------------

3. Print duplicate number from array.

const numbers = [1, 3, 4, 5, 7, 8, 1, 3, 4];

let duplicate = numbers.filter((a, b, c) => c.indexOf(a) !== b)

console.log(duplicate)

-----------------------------------------------------------------------------------------------

8. What is hosting in js

moving all the declarations at the top of the scope before code execution

-----------------------------------------------------------------------------------------------

9. why javascript is a single-threaded language?

Because of only one call stack.

-----------------------------------------------------------------------------------------------

10. What is async-await.

"async and await make promises easier to write"
async makes a function return a Promise
await makes a function wait for a Promise

-----------------------------------------------------------------------------------------------

11. Lazy loading

Lazy loading is a technique in Angular that allows you to load JavaScript components asynchronously when a specific route is activated

-----------------------------------------------------------------------------------------------

12. Observable

-----------------------------------------------------------------------------------------------

13. Decorators

NgModule ,Component ,Injectable ,Directive ,Pipe ,Input ,Output ,HostBinding ,HostListener ,ContentChild ,ContentChildren ,ViewChild ,ViewChildren

-----------------------------------------------------------------------------------------------


14. Eventloop

The event loop is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded

Multiple clients make multiple requests to the NodeJS server. NodeJS receives these requests and places them into the EventQueue .
NodeJS server has an internal component referred to as the EventLoop which is an infinite loop that receives requests and processes them. This EventLoop is single threaded. 

-----------------------------------------------------------------------------------------------


15. Middleware

Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next function in the application's

-----------------------------------------------------------------------------------------------

16. promises.all & Promise.allSettled

The Promise.all() method takes an iterable of promises as an input, and returns a single Promise that resolves to an array of the results of the input promises. 
In angular we can use Rxjs forkJoin.

Promise.all will reject as soon as one of the Promises in the array rejects.

Promise.allSettled will never reject - it will resolve once all Promises in the array have either rejected or resolved.

-----------------------------------------------------------------------------------------------


17. Print first n prime numbers,

const prime = (n) => {
  let primeNumber = [];
  for (let i = 2; i <= n; i++) {
    let flag = 0;
    for (let j = 2; j < i; j++) {
      if (i % j == 0) {
        flag = 1;
        break;
      }
    }
    if (flag == 0) {
      primeNumber.push(i);
    }
  }
  return primeNumber;
};
console.log(prime(20));

-----------------------------------------------------------------------------------------------

18. Promise
A Promise handles a single event when an async operation completes or fails.
Pending, Resolved, Rejected

Observable
An Observable is like a Stream (in many languages) and allows to pass zero or more events where the callback is called for each event.


Promises and Observables both handle the asynchronous call only.

Here are the differences between them:

Observable:
Emits multiple values over a period of time
Is not called until we subscribe to the Observable
Can be canceled by using the unsubscribe() method
Provides the map, forEach, filter, reduce, retry, and retryWhen operators

Promise:
Emits only a single value at a time
Calls the services without .then and .catch
Cannot be canceled
Does not provide any operators

-----------------------------------------------------------------------------------------------

19. What is DocType in HTML

The declaration is not an HTML tag. It is an "information" to the browser about what document type to expect.

<!DOCTYPE html>

-----------------------------------------------------------------------------------------------

20. Difference between local storage and session storage

localStorage doesn't expire, data in sessionStorage is cleared when the page session ends - 5MB

-----------------------------------------------------------------------------------------------

21. Directives

Components	Used with a template. This type of directive is the most common directive type.
Attribute directives	NgClass, NgStyle
Structural directives	NgIf, NgFor

-----------------------------------------------------------------------------------------------

22. .htaccess file usage
htaccess file that solves the route redirection issue. 

-----------------------------------------------------------------------------------------------

23. Find sum of individual number from a given number and output should be in single digit.

[1, 2, 3, 4].reduce((a, b) => a + b, 0)

-----------------------------------------------------------------------------------------------

24. Explain CORS?

Cross-Origin Resource Sharing known as CORS, allows you to request for different resources from a different domain outside of the domain where the resource is originally from.

-----------------------------------------------------------------------------------------------

25. interface or class in Typescript

class is essentially an object factory (a blueprint of what an object is supposed to look like)
interface is a structure used solely for type-checking.

-----------------------------------------------------------------------------------------------

26. What are callbacks?
A callback is a function passed as an argument to another function


A callback is a function that is passed into another function as an argument to be executed later. (Developers say you “call” a function when you execute a function, which is why callbacks are named callbacks).


function fullName(fullName) {
  console.log({ fullName });
}

function name(a, b, myCall) {
  let fn = a + b;
  myCall(fn);
}

name("usman", "shaikh", fullName);

-----------------------------------------------------------------------------------------------

27. slice & splice
slice returns a piece of the array but it doesn’t affect the original array. 
splice changes the original array by removing, replacing, or adding values and returns the affected values.

-----------------------------------------------------------------------------------------------

28. If array of objects, findIndex();
Else, indexOf().
https://stackoverflow.com/a/61884089

-----------------------------------------------------------------------------------------------

29. A "higher-order function" is a function that accepts functions as parameters and/or returns a function.

-----------------------------------------------------------------------------------------------

30. What are Indexes in MongoDB?

Indexes are special data structures that store a small portion of the collection's data to limit the number of documents to scan. otherwise it will scan every document in a collection.

Indexes support the efficient execution of queries in MongoDB. Without indexes, MongoDB must perform a collection scan, i.e. scan every document in a collection, to select those documents that match the query statement. If an appropriate index exists for a query, MongoDB can use the index to limit the number of documents it must inspect.

Indexes are special data structures that store a small portion of the collection's data set in an easy to traverse form.

collection.createIndex( { name : -1 }, function(err, result) {
   console.log(result);
   callback(result);
}

-----------------------------------------------------------------------------------------------

31. What are the types of Indexes available in MongoDB?

Single Field, Compound, Multikey, Geospatial, Text, Hashed Index

-----------------------------------------------------------------------------------------------

32. ascending & descending 

ascending = 1,2,3,4
descending = 4,3,2,1

db.people.createIndex( {age : 1} ) // creates an ascending index
db.people.createIndex( {age : -1} ) // creates a descending index

-----------------------------------------------------------------------------------------------

34. relationship in MongoDB

One-to-One, One-to-Many, Many-to-Many

-----------------------------------------------------------------------------------------------

35. embedding and referencing 

Embedding:
embed a document inside another document

Referencing:
referenced document's id inside other document

-----------------------------------------------------------------------------------------------

36. Pagination Query

find().sort({a:1, b:1}).skip(1).limit(2)

-----------------------------------------------------------------------------------------------

37. What is “Namespace” in MongoDB?

MongoDB stores BSON (Binary Interchange and Structure Object Notation) objects in the collection. The concatenation of the collection name and database name is called a namespace

-----------------------------------------------------------------------------------------------

38. Projection

projection means selecting only the necessary data rather than selecting whole of the data of a document.
If a document has 5 fields and you need to show only 3, then select only 3 fields from them.

db.inventory.find( { status: "A" }, { item: 1, status: 1, _id: 0 } ) 


-----------------------------------------------------------------------------------------------

40. Aggregate() Method

$project − Used to select some specific fields from a collection.

$match − This is a filtering operation and thus this can reduce the amount of documents that are given as input to the next stage.

$group − This does the actual aggregation as discussed above.

$sort − Sorts the documents.

$skip − With this, it is possible to skip forward in the list of documents for a given amount of documents.

$limit − This limits the amount of documents to look at, by the given number starting from the current positions.

$unwind − This is used to unwind document that are using arrays. When using an array, the data is kind of pre-joined and this operation will be undone with this to have individual documents again. Thus with this stage we will increase the amount of documents for the next stage.

-----------------------------------------------------------------------------------------------

41. Angular security practices

Prevent an application from Cross-Site Scripting (XSS)
Use Route guards when required
Up-to-date Angular Libraries


-----------------------------------------------------------------------------------------------

42. Nodejs security practices

Security: set security HTTP headers using helmet
Santizing: sanitize request data against xss and query injection
Protect Users' Passwords/Secrets using bcrypt 
Validate incoming JSON schemas
Support blocklisting JWTs

-----------------------------------------------------------------------------------------------

43. Authentication & Authorization

Authentication: login 
Authorization:  after login if user have acces to use particular route

-----------------------------------------------------------------------------------------------

44. reactjs-virtual-dom

https://www.geeksforgeeks.org/reactjs-virtual-dom/

Virtual DOM: React uses Virtual DOM exists which is like a lightweight copy of the actual DOM(a virtual representation of the DOM). So for every object that exists in the original DOM, there is an object for that in React Virtual DOM. It is exactly the same, but it does not have the power to directly change the layout of the document. Manipulating DOM is slow, but manipulating Virtual DOM is fast as nothing gets drawn on the screen. So each time there is a change in the state of our application, the virtual DOM gets updated first instead of the real DOM. 

-----------------------------------------------------------------------------------------------

45. Are you aware of the top DevOps tools?

The most popular DevOps tools are:

Jenkins: Continuous Integration tool
Docker: Containerization tool
Git: Version Control System tool

-----------------------------------------------------------------------------------------------

46. simple server in Node.js 

const express = require('express');
const app = express();

app.get('/', function (req, res) {
  res.send('Hello World!');
});

app.listen(3000, function () {
  console.log('App listening on port 3000!');
});

-----------------------------------------------------------------------------------------------

47. Call, Apply & Bind

Call invokes the function and allows you to pass in arguments one by one.
Apply invokes the function and allows you to pass in arguments as an array.
Bind returns a new function, allowing you to pass any number of arguments.

https://stackoverflow.com/a/46700616

-----------------------------------------------------------------------------------------------



React
the difference between functional component and class-based component in react

L1: css positions, props, virtual dom, functional components, class components, difference between them, Hoisting, promises, promises.all, es6 functions, props drilling, context api, redux, difference between class and functional, callback, diff let, var and const, css properties, git stash, cherrypick, reducers, setState, hooks, spread operator, rest operator, diff between both, react optimization, error boundaries, closures


Hands-on experience with DevOps, AWS/Google Cloud/Azure.

kafka 
feign client


How does the browser identify if the URL resource is XML/image/json? (content-type)
What does L stands for in SOLID principles?
What are the practical ways to apply coding principles in .net?
Write a program to check anagram in a string? What is the time complexity of this program?
How do you manage disaster recovery? What is the average time you completed the process in your company?
How to design a File System with directories, files, permissions? Give the class design with it's relationships? A directory can have multiple childs and it's child can have multiple sub-childs and so on. What data structure to choose from? What is the time complexity of insertion and deletion in the data structure?
Why did you choose NoSql database instead of SQL?
Why did you choose RavenDB instead of CouchDB, Cassandra, MongoDB etc.
Why did you choose microservices architecture instead of service oriented architecture?
Suppose you have to design and model an application that accepts feed, rss feeds and HTML view from other applications. How would you design the application? What classes will you use?
Why did you chose Microsoft stack for product development?
Explain the architecture of your current application?
What is the code coverage in your application?
How did you implement CI/CD in your application and which tool did you use for CI/CD? Which branches of git repository did you use for CI/CD?
What is the difference between props and state in React?
What did you use Redux for?
Why react instead of angular?


scrum/agile

Hands-on experience on Angular,CSS,Scripting,NodeJs / express
Strong experience in REST APIs
Experience in Responsive Web,Automation,CI / CD,Github,Microservices,Postgres (or any other RDBMS)
Experience in AWS (SQS,SNS,Cognito)
Experience in Quality Assurance, Code Optimization, Docker, Load Balancer, Kubernete
Experience in Scrum and agile methodalogies

Infosys
5+ years of experience developing full stack applications using frameworks like angular and nodejs (MEAN stack).
3+ years of experience working on any cloud platform like Azure, AWS, GCP etc. (Preferably Azure).
Good hands-on working knowledge of developing REST APIs and experience in building microservices that follow 12 factor app guidelines.
Good knowledge of UI/UX development with hands-on HTML/CSS/Javascript.
Good knowledge of Dev Sec Ops and CI/CD pipelines with Github Actions/Jenkins/Azure Devops etc.
Hands-on experience writing unit tests/integrations tests with frameworks like jest/karma/jasmine/protractor/cypress etc.
Basic Database engineering skills needed for a backend developer and good experience working on APIs integrations with Database.
Exposure to one or more of the following is preferable - Event Driven systems design, Serverless functions, Azure Data factory pipelines

-----------------------------------------------------------------------------------------------