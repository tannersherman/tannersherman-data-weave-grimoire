# tannersherman-data-weave-grimoire

Uses the default Main.dwl provided in mulesoft-labs/data-weave-native but accepts the payload as a port number. Add the following bash function to your `~/.bash_profile` 
for bash or `~/.zshrc` for Z shell for easy spin up on a provided port. Default port will be 8081. 

```
function dw_pg() {
  local port=${1:-"8081"}
  echo ${port} | dw --eval --spell tannersherman/dw_playground  

}
```
