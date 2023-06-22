# Mapping (149 Points)
### Category: Web
Looks like its time to find the treasure (flag). Can you find the flag with this treasure map?

https://mapping.nypinfosec.com

## Solution

![](https://i.gyazo.com/3501c3d30bce83875b59ec74ba7c2d38.png)
1. You get a Google Maps embed, I looked around in it too. Just a plain proper maps embed with nothing extra.
2. So you look at the URL and link it to sitemap.xml
![](https://i.gyazo.com/5786922643d4b3995fbdfaaee6706819.png)
3. You go to `https://mapping.nypinfosec.com/sitemap.xml`, it tells you to go to /someStupidFlag
4. You go there and got the flag.
5. You see the root directory now, and flag.txt.
```
Flag: NYP{s1tem3p_xm1}
```