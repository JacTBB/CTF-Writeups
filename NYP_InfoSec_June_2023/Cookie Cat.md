# Cookie Cat (50 Points)
### Category: Web
Song lyrics (adapted from Steven Universe: Gem Glow): Oohhhhh! He's a frozen treat with an all new taste! 'cause he came to this planet from outer space! A refugee of an interstellar war! But now he's at your local grocery store! Cookie Cat! He's a pet for your tummy! Cookie Cat! He's super duper yummy! Cookie Cat! He left his family behind! But oh no, where is cookie cat?

Find the secret number and get Steven his lost cookie cat.

https://cookiecat.nypinfosec.com

## Solution

![](https://i.gyazo.com/c4c772c79a2871baeb5bf4c280ecd6c2.png)
1. Identify the different coffee tabs go to different paths. 
`https://cookiecat.nypinfosec.com/index/1`
`https://cookiecat.nypinfosec.com/index/20`
2. Make a script to fetch every path in increasing number.
(I used Javascript + Node Fetch, Simple Loop)
3. You will get `https://cookiecat.nypinfosec.com/index/160` and the flag.
```
Flag: NYP{tHE_seCR3t_c00k1e_c@T}
```