# hkube-js-algorithm
to start algorithm 
```json
{"action":"startAlg","algName":"green-alg","input":[1]}
```
to start pipeline 
```json
{"action":"startStored","pipeName":"simple","input":{"inp":"5"}}
```
to start raw pipeline
```json
{"action":"startRaw","pipeName":"raw","pipNodes":"[
    {
      \"algorithmName\": \"green-alg\",
      \"input\": [
        \"@flowInput.bar\"
      ],
      \"nodeName\": \"a\"
    },
    {
      \"algorithmName\": \"yellow-alg\",
      \"input\": [
        \"#@a\"
      ],
      \"nodeName\": \"b\"
    }
  ]","input":{"bar":{"size":"3","batch":"4"}}}
```
if you need to debug package.json dependencies should be -  dependencies": {
    "@hkube/nodejs-wrapper": "^2.0.25",
    "i": "^0.3.6",
    "npm": "^6.14.9"
  }
