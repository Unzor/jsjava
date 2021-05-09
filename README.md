# jsjava
JSJava is a JavaScript library that connects to a Java VM via WebSocket. I made it to mess around with Java in the browser, and not to use for big projects.

# API
To use the JSJava API, use this example script:

```
var jsjava=new JSJava();
jsjava.setFileName('Main.java');
jsjava.onCallback=function(output){
console.log('output');
}
jsjava.setCode(`
public class Main
{
    public static void main(String[] args) {
        System.out.println("Hello World! :)");
    }
}
`);
jsjava.run();
```
This script will log "Hello World!" in the console.


# Building
### Dependencies:
- Git

To build JSJava, use this (in cmd, terminal, powershell, etc):
```
git clone https://github.com/Unzor/jsjava/
```

Then you can use the ```jsjava.js``` file from the ```jsjava``` directory.







