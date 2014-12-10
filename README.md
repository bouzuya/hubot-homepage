# hubot-homepage

A Hubot script for hosting your web page.

See [`src/homepage.coffee`](src/homepage.coffee) for full documentation.

## Installation

In hubot project repo, run:

`npm install hubot-homepage --save`

Then add **hubot-homepage** to your `external-scripts.json`:

```json
[
  "hubot-homepage"
]
```

## Sample Interaction

```
bouzuya> hubot homepage list

bouzuya> hubot homepage add bouzuya http://bouzuya.net/
  hubot> added bouzuya http://bouzuya.net/
bouzuya> hubot homepage add blog http://blog.bouzuya.net/
  hubot> added blog http://blog.bouzuya.net/
bouzuya> hubot homepage add google http://www.google.com/
  hubot> added google http://www.google.com/

bouzuya> hubot homepage list
  hubot> [0] bouzuya http://bouzuya.net/
         [1] blog http://blog.bouzuya.net/
         [2] google http://www.google.com/

bouzuya> hubot homepage rm 1
  hubot> removed blog http://blog.bouzuya.net/

bouzuya> hubot homepage list
  hubot> [0] bouzuya http://bouzuya.net/
         [1] google http://www.google.com/
```
