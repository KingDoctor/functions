# This is to get colored Client message without having to write color code and the double 'S'.
```js
colorMessage = function(message, color){
	switch(color){
		case "RED":
			clientMessage(ChatColor.RED+""+message);
			break;
		case "BLACK":
			clientMessage(ChatColor.BLACK+""+message);
			break;
		case "DARK_BLUE":
			clientMessage(ChatColor.DARK_BLUE+""+message);
			break;
		case "DARK_GREEN":
			clientMessage(ChatColor.DARK_GREEN+""+message);
			break;
		case "DARK_AQUA":
			clientMessage(ChatColor.DARK_AQUA+""+message);
			break;
		case "DARK_RED":
			clientMessage(ChatColor.DARK_RED+""+message);
			break;
		case "DARK_PURPLE":
			clientMessage(ChatColor.DARK_PURPLE+""+message);
			break;
		case "GOLD":
			clientMessage(ChatColor.GOLD+""+message);
			break;
		case "GRAY":
			clientMessage(ChatColor.GRAY+""+message);
			break;
		case "DARK_GRAY":
			clientMessage(ChatColor.DARK_GRAY+""+message);
			break;
		case "BLUE":
			clientMessage(ChatColor.BLUE+""+message);
			break;
		case "GREEN":
			clientMessage(ChatColor.GREEN+""+message);
			break;
		case "AQUA":
			clientMessage(ChatColor.AQUA+""+message);
			break;
		case "LIGHT_PURPLE":
			clientMessage(ChatColor.LIGHT_PURPLE+""+message);
			break;
		 case "YELLOW":
			clientMessage(ChatColor.YELLOW+""+message);
			break;
		case "WHITE":
			clientMessage(ChatColor.WHITE+""+message);
			break;
	}
};
```
# Example
```js
colorMessage("This is an example of the colored message function", GOLD); //makes a colored clientMessage();
```
