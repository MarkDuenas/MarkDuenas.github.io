# Node Ecosystem, TDD, CI/CD

## Describe (in plain English) what Array.map() does

  - .map() method returns a new array as it iterrates through the array.

## Describe (in plain English) what Array.reduce() does

  - .reduce() method uses a **reducer** function on each element of the array, returns a single output value.
  
## Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

### Promise using `.then()` syntax.
```
  let getCharacters = () => {
    superagent.get('https://swapi.dev/api/people/1/')
      .then( data => {
        let name = data.body.name;
        let char = {[name]: data.body.url};
        console.log(char);
      })
      .catch(err => console.error(err));
  }
```

### Promise using `async` and `await` function.
```
  async function getLocation(city) {
    let data = await superagent.get(`https://geocode.xyz/${city}?json=1`);
    console.log(`${city}`, 'longitude:', data.body.longt, 'latitude:', data.body.latt);
  }
```

## Explain promises as though you were mentoring a Code 301 level student

Promises are just that, a promise. It's a condition that you said will happen **eventually** so you set up the promise by saying "hey this is my promise, it will be fulfilled later".
Once the promise is fulfilled, then you have that **data** or whatever results from that to do whatever it is you want with it. The promise is either fulfilled or rejected and it is just like that.

## Are all callback functions considered to be Asynchronous? Why or Why Not?

Callback functions are normally not Asynchronous, but it can be. Callbacks are sycnhronous most times because the functions executes as its called and waits till the functions finishes until it moves to the next line.

