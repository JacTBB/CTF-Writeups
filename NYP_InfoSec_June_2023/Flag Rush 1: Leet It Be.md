# Flag Rush 1: Leet It Be (297 Points)
### Category: FlagRush
**Originally Appeared On:** https://flagthecapture.blogspot.com/2023/05/flagrush-1.html

**Infosec CTF Insight:**
Only the top 3 participants managed to solve this. Hmm.

This is Agent Will Hackett. I have reason to believe the Investigative Cybercrime Unit has been compromised.

I don't know who is behind this, or what their motives are, but lately there have been signs of unauthorized access within our networks. Therefore, I will encrypt all my findings.

The password for my next folder will be "FTC{it_would_be_cool_if_can_you_make_this_flag_leet_thanks}". Of course, per the ICU rules, all passwords have to be converted into LeetSpeak first.

Hint: tjmlwxgjuw? You may use the 7z file provided to check your answers.

Note: Flag format is FTC{xxxxx}

> This challenge originally appeared as part of the FlagRush event. You may find certain helpful files in this [Documents](https://github.com/MarkB-NYP/FlagRushCTF_1/tree/main/FlagRush%201%20Documents) folder.

## Solution 1 (As Intended In Infosec June 2023 CTF)

1. You are given a requirements.txt, not helpful, and a zip file.
2. With no other information, you brute force this long zip file password (That is also the flag).
3. Honestly no idea who would even try to brute force this.
```
Flag: NYP{Do_It_Yourself}
```

## Solution 2 (As Intended In FlagRush CTF, I think)

1. Going to the Github repo, you get random files.
2. Download `possibilities.zip` and the `Level 2.7z`
3. Use the wordlist and brute force the zip.
```
Flag: NYP{Do_It_Yourself}
```

## Solution 3 (Abuse FlagRush CTF Flag Submission Portal)

1. Going to https://markb-nyp.github.io/FlagRush/portal.html
2. You inspect the code and see the flag hash checker inside in SHA-256.
```
const hashes = ['6b63d9e767392ae6dffee6be16c09a216568c6adbf10e047c5f68865891a1018','6a0ced29e628937c9364a3bf94d298fd80d10e8672e49262ed8e5ece6da57c59','54df1c8842c0da42dda7bcbf9e35dc417ce2289e0f04176c9652e07f536d24a8','bc2b89ef09e723cf4da1e1cbb33defc1eea90f3467cb1294aff86ce6da4c12b4','0ce71a96546da8018d724fc79f3acdc5c0146473db644ad5efab69adf71f8edb','b073c9ee7e6169393208302b17c4e5f5bec2b6dadeaca208b09e442a7b20ce6a','873e1aeb9d0e297bf983407e8050e5a7a20711cfc26fc184603ca75e2df9a378']
```
        
2. So you use the `possibilities.zip` wordlist on the 1st hash but you use Python / Javascript instead, wayyy faster than me trying John for 6 hours.
3. Got it in a few seconds.
```
Flag: NYP{Do_It_Yourself}
```