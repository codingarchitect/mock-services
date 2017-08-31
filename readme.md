```
git clone https://github.com/codingarchitect/mock-services.git
cd mock-services
npm install
npm start
```

To test if the API endpoint is working, Open chrome or your favorite browser, 
In the developer tools type the following

sales order types endpoint, watch the case
```
fetch('http://localhost:3000/salesOrderTypes')
  .then(function(response) {
    return response.json()
  }).then(function(json) {
    console.log('parsed json: ', json)
  }).catch(function(ex) {
    console.log('parsing failed: ', ex)
  });
```

default sales order type endpoint, watch the case
```
fetch('http://localhost:3000/salesOrderTypes/default')
  .then(function(response) {
    return response.json()
  }).then(function(json) {
    console.log('parsed json: ', json)
  }).catch(function(ex) {
    console.log('parsing failed: ', ex)
  });
```

Both should run without any error