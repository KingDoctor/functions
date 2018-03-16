# See if a specific player is online
```js
function serverGetPlayer(name) {
	return Server.getAllPlayers[Server.getAllPlayerNames().indexOf(name)];
};
```
## Example
```js
serverGetPlayer("KingDoctorX"); 
```
