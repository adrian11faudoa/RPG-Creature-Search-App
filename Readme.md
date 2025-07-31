Subject:

To tell the code to wait for the response from the server:
```
  const getCreature = async () => {
    try {
      const creatureNameOrId = searchInput.value.toLowerCase();
      const response = await fetch(
        `https://rpg-creature-api.freecodecamp.rocks/api/creature/${creatureNameOrId}`
      );
      const data = await response.json();

  } catch (err) { }
  };
```

To stop the page to reload when submit the form:
```
  searchForm.addEventListener('submit', e => {
    e.preventDefault();
  });
```
