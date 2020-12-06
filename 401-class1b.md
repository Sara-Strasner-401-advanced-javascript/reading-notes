# Node Ecosystem, TDD, CI/CD

1. Describe (in plain English) what Array.map() does:

Array.map() loops over an array and makes a new one with the results of calling a provided function on every element of the array
1. Describe (in plain English) what Array.reduce() does:

Array.reduce() executes a provided function on each value in an array and returns a single output. To learn more about the many uses of array.reduce() see [5 Use Cases for reduce() in JavaScript](https://medium.com/javascript-in-plain-english/5-use-cases-for-reduce-in-javascript-61ed243b8fef)
1. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result:
- With normal Promise .then() syntax

```
const getCharacters = (request, response)=> {
  let url = 'https://swapi.dev/api/people/';

  superagent.get(url)
    .then(data => {
      const starWarsArray = data.body.results;
      console.log(starWarsArray);
      const finalStarWarsArray = starWarsArray.map(person => new StarWars(person));
      console.log(finalStarWarsArray);
      // response.render(finalStarWarsArray);
    })
    .catch(error =>{
      console.log(error);
    })

function StarWars(person){
  this.name = person.name;
  this.url = person.url;
}
```

- Again with async / await syntax

```
async function getCityData(city) {
  try {
    const response = await superagent.get(`https://geocode.xyz/${city}?json=1`)
    console.log(response.body.latt, response.body.longt);
  } catch (error) {
    console.log(error.response.body);
  }
}

getCityData('Denver');
```

1. Explain promises as though you were mentoring a Code 301 level student

Promises are an object that may produce a single value sometime in the future. Promises have three states, resolved, rejected, and pending. They are often compared to envelopes since they may or may not return with a value. For examples of its usage, see [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise).
1. Are all callback functions considered to be Asynchronous? Why or Why Not?

No, not **all** callback functions are considered asynchronous. Typically, callback functions that involve requests for external resources (ajax calls, API calls, etc.) are asynchronous, and others may or may not be. Callbacks that you call yourself are regular function calls, which are always synchronous. For more information, see [Does taking a callback make a function asynchronous?](https://bytearcher.com/articles/does-taking-a-callback-make-a-function-asynchronous/).