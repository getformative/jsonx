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
  "[0].padawan.id": "ahsoka@jedi.galaxy",
  "[0].padawan.firstName": "Ahsoka",
  "[0].padawan.lastName": "Tano",
  "[0].master": "anakin@jedi.galaxy",
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
