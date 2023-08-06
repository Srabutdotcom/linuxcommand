##deno command

## How to debug inspect remote server:
[How to debug remote server](https://stackoverflow.com/questions/50242557/how-to-debug-remote-node-js-app-using-chrome-devtools/50242558#50242558)
1. run server with `inspect` command i.e. deno run --inspect server.js
2. open browser with chrome://inspect
3. note: ensure ssh is already opened if not open with `ssh -L 9221:localhost:9229 user@remote.example.com`
  
