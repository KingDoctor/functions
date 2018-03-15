# A faster clear inventory function :)
```js
clearInventory = function() {
	for(var i = 0; i < 255; i++) Player.clearInventorySlot(i);
};
```
## Example
```js
clearInventory(); // use it when player might use a command or click a button
```
