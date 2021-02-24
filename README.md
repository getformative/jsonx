# JSONx

Expanded JSON.

JSONx allows predictable expansion and flattening of JSON structures into single key-value representations.

**Flat**

```json
{
  "[0].padawan.id": "anakin@jedi.galaxy",
  "[0].padawan.firstName": "Anakin",
  "[0].padawan.lastName": "Skywalker",
  "[0].master": "obi@jedi.galaxy",
  "[1].padawan.id": "ahsoka@jedi.galaxy",
  "[1].padawan.firstName": "Ahsoka",
  "[1].padawan.lastName": "Tano",
  "[1].master": "anakin@jedi.galaxy",
}
```

**Deep**

```json
[
  {
    "padawan": {
      "id": "anakin@jedi.galaxy",
      "firstName": "Anakin",
      "lastName": "Skywalker"
    },
    "master": "obi@jedi.galaxy"
  },
  {
    "padawan": {
      "id": "ahsoka@jedi.galaxy",
      "firstName": "Ahsoka",
      "lastName": "Tano"
    },
    "master": "anakin@jedi.galaxy"
  }
]
```
