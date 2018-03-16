# A list of functions that have to do with Items.
```js
function removeItem() {
	Player.clearInventorySlot(Player.getSelectedSlotId());
};

function removeFromItem(amount) {
	Entity.setCarriedItem(Player.getEntity(), Player.getCarriedItemCount() - amount ? Player.getCarriedItem() : 512, Player.getCarriedItem(), Player.getCarriedItemCount() - amount, Player.getCarriedItemData());
};

function addToItem(amount) {
	Entity.setCarriedItem(Player.getEntity(), Player.getCarriedItem(), Player.getCarriedItemCount() + amount, Player.getCarriedItemData());
};

function itemSetName(id, damage, name) {
	if(Item.getName(id, damage, 1)) ModPE.langEdit(Item.getName(id, damage, 1) + ".name", name);
};

```
## Example
```js
addToItem(22); // If I was carrying 3 apples after this function I would have 25 apples.

removeFromItem(22); // If I was carrying 25 carrets after this function I would have 3 carrets.

removeItem(); // Removes the whole item from the hand you have.

itemSetName(276, 0, "Sharp Stick"); // Renames the item with you name you have provided.
```
