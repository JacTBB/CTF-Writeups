# Ping pong (111 Points)
### Category: Web
Ping. Pong. Cats love to play it, but there are hiding a superweapon inside the ping pong table. Your mission is to find the killswitch code(flag) inside the table to deactivate the superweapon. Can you do it champ?

https://pingpong.nypinfosec.com

## Solution

![](https://i.gyazo.com/37d98e25b29a735c2fba0dc3aab289c2.png)
1. You find a ping form.
2. You input `; ls` to see if it is vulnerable to command injection.
3. You got the current directory, with main.py, static, templates.
4. So you do `; ls ..`.
5. You see the root directory now, and flag.txt.
6. So you run `; cat ../flag.txt` and got the flag.
```
Flag: NYP{iNJ3c+3d}
```