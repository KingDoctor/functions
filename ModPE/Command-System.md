```js
// Command System by @KingDoctorX. 

var MainActivity = com.mojang.minecraftpe.MainActivity.currentMainActivity.get();
var github = "https://github.com/KingDoctor/ModPE-School/tree/master/ModPE";
const prefix = "@";

function reply(text) {
	clientMessage(ChatColor.BLUE + "[" + ChatColor.RED + "CMD" + ChatColor.BLUE + "]" + ChatColor.YELLOW + " => " + text);
}

function chatHook(command) {
    let cmd = command.split(" ")
	if (cmd[0] == prefix + "help") {
		preventDefault();
		reply(prefix + "help");
		reply(prefix + "give");
		reply(prefix + "github");
	}
	if (cmd[0] == prefix + "give") {
		preventDefault();
		Player.addItemIventory(cmd[1], cmd[2], cmd[3]);
		reply("item: \"" + cmd[1] + "\" has been added to your inventory.");
	}
	if (cmd[0] == prefix + "github") {
		preventDefault();
		var url = new android.content.Intent(MainActivity);
		url.setAction(android.content.Intent.ACTION_VIEW);
		url.setData(android.net.Uri.parse(github));
		MainActivity.startActivity(url);
	}
}
```
