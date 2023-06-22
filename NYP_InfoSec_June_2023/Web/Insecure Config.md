# Ping pong (119 Points)
### Category: Web
Looks like someone screwed up a server configuration again.

https://insecurecfg.nypinfosec.com

## Solution

![](https://i.gyazo.com/03b71bfa2bd98f36d2799526ba065b52.png)
1. You find a bunch of text, 0.01 points if you stuck it into Cyberchef. You got nothing.
2. So you try `https://insecurecfg.nypinfosec.com/flag.txt` and got a Jinja Template Not Found.
![](https://i.gyazo.com/23e618d789804ca9655f412c3e1fb6b8.png)
3. You conveniently find a `/logs` route that exposes the debugger pin `899-437-513`.
4. You go back to flag.txt and pop open the debugger.
![](https://i.gyazo.com/0b00f8fcdbc1d3bd6dcac4f4dbca6fa6.png)
5. You run these commands: `import os` and `os.popen("ls").read()`, you see a flag.txt file.
6. You output it `os.popen("cat flag.txt").read()` and got the flag.
```
Flag: NYP{d3bug_c0nso1e}
```