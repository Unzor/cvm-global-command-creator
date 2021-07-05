# cvm-global-command-creator
API for creating global command in CollabVM.

# API Example
```javascript
var e = new GlobalCommand({
onchat: function(content, username){
console.log(username + ' chatted' + content);
}});
```
Stop global command from being used:

```javascript
e.removeGlobalCommand();
```
