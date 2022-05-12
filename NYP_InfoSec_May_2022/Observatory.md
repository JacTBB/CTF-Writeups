# Obervatory
I have a website up for the public to view astronomical images from an observatory.
However, I heard that there are errors and the site is leaking some confidential information.

https://observatory.nypinfsecctf.tk

## Solution

1. Putting in any value except those which you can select will show you an error message above the default image. (May be hard to see, so highlight)
2. Make a requestbin
3. Remember to remove the https:// from your url. @ is to escape the default url. Input: @requestbin_url
4. Look at your requestbin body and you will find the flag.
```
Flag: NYP{eRr0r5_4rE_My_Fr1enD5}
```
