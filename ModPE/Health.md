### Server Script that can enable mods on servers.

```js
function addHealth(amount) => {
		Entity.setHealth(getPlayerEnt(), Entity.getHealth(getPlayerEnt()) + amount);
	}
  
function removeHealth(amount) => {
		Entity.setHealth(getPlayerEnt(), Entity.getHealth(getPlayerEnt()) - amount);
	}
```
# Examples
```js
addHealth(5); // adds 4 and a half hearts to your player.

removeHealth(20); // remove all hearts from your player.
```
