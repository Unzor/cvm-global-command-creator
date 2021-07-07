# cvm-global-command-creator
API for creating global command in CollabVM.

# API Example
```javascript
var script=document.createElement('script');script.src="https://cdn.jsdelivr.net/gh/Unzor/cvm-global-command-creator/cmd.js";document.body.appendChild(script);

var e;

script.onload=function(){
e = new GlobalCommand({
onchat: function(content, username){
console.log(username + ' chatted' + content);
}});
}
```
Stop global command from being used:

```javascript
e.removeGlobalCommand();
```
