# Types Done:

A checklist for which types have been manually tested.

* [x] schemas
* [x] responses
* [x] parameters
* [x] examples
* [x] requestBodies
* [x] headers
* [x] securitySchemes
* [x] links
* [x] callbacks
* [x] pathItems

## schemas (4)

### Test 1 (3)
```
parameterObject.schema -> Schema Object
requestBody.content[x].schema -> Schema Object
response.content[x].schema -> Schema Object
```
Input
```
http://localhost:5500/package/testFiles/callbackTest.yaml
```
Output
```
Correct
```

### Test 2 (1)
```
headerObject[x].schema -> Schema Object
```
Input
```
http://localhost:5500/package/testFiles/headerTest1.yaml
http://localhost:5500/package/testFiles/headerTest2.json
```
Output
```
Correct
```
Done

## responses (1)
```
pathItemObject[x].responses.y -> {Status Code/ "default" : Response Object | Reference Object}
```
Input
```
https://api.apis.guru/v2/specs/xkcd.com/1.0.0/openapi.json
```
Output
```
Correct
```
Done
***

## parameters (2)

### Test 1
```
pathItem[x].parameters[y] -> Parameter Object | Reference Object 
```
Input
```
http://localhost:5500/package/testFiles/parameterTest.yaml
```
Output
```
Correct
```

### Test 2
```
pathItem[x][y].parameters[z] -> Parameter Object | Reference Object
```
Input
```
https://api.apis.guru/v2/specs/xkcd.com/1.0.0/openapi.yaml
```
Output
```
Correct
```
Done

## examples (4)

### Test 1
```
requestBody.content[x].examples.y -> {name: Example Object}
```
Input
```
http://localhost:5500/package/testFiles/callbackTest.yaml
```
Output
```
Correct
```

### Test 2
```
response[x].content[y].examples.z -> {name: Example Object}
```
Input
```
http://localhost:5500/package/testFiles/exampleTest2.json
```
Output
```
Correct
```

### Test 3
```
parameterObject.examples.x -> Example Object {name: Example Object}
```
Input
```
http://localhost:5500/package/testFiles/parameterTest.yaml
```
Output
```
Correct
```
### Test 4
```
headerObject[x].examples.y -> {name: Example Object}
```
Input
```
http://localhost:5500/package/testFiles/headerTest2.json
```
Output
```
Correct
```
## requestBodies (1)

### Test 1
```
pathItemObject[x].requestBody -> Request Body Object | Reference Object 
```
Input
```
https://oai.github.io/Documentation/examples/tictactoe.yaml
```
Output
```
Correct
```
Done

## headers (2)

### Test 1
```
requestBody.content[x].encoding[y].headers.z ->{name: Header Object | Reference Object}
```
Input
```
http://127.0.0.1:5500/package/testFiles/headerTest1.yaml
```
Output
```
Input
```

### Test 2
```
responseObject[x].headers.y -> {name: Header Object | Reference Object }
```
Input
```
http://127.0.0.1:5500/package/testFiles/headerTest2.json
```
Output
```
Correct
```
***
Done

## securitySchemes (1)

### Test 1
```
document.components.securitySchemes.x -> { name : Security Scheme Object | Reference Object}
```
Input
```
http://127.0.0.1:5500/package/testFiles/securitySchemeTest.yaml
```
Output
```
Correct
```
Done
***

## links (1)

### Test 1
```
response[x][y].links.z -> {name: Link Object | Reference Object}
```
Input
```
http://127.0.0.1:5500/package/testFiles/linkTest.yaml
```
Output
```
Correct
```
***
Done

## callbacks (1)

### Test 1
```
pathItem[x][y].callbacks.z -> {name: Callback Object | Reference Object}
```
Input
```
http://127.0.0.1:5500/package/testFiles/callbackTest.yaml
```
Output
```
Correct
```
Done
***


## pathItems (3)

### Test 1
```
document.paths.x -> {path:Path Item Object | Reference Object}
```
Input
```
https://api.apis.guru/v2/specs/xkcd.com/1.0.0/openapi.yaml
```
Output
```
Correct
```

### Test 2
```
callbacks[x].y -> {path:Path Item Object | Reference Object} 
```
Input
```
http://127.0.0.1:5500/package/testFiles/callbackTest.yaml
```
Output
```
Correct
```

### Test 3
```
document.webhooks.x -> {path:Path Item Object | Reference Object}
``` 
Input
```
http://127.0.0.1:5500/package/testFiles/pathItemTest.yaml
```
Output
```
Correct
```
Done
***
