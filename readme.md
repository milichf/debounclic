# 📄 debounclic

this is a smol-badly written-autohotkey script.... which simulates double clicks.....

---

it also has a.. web thingy; which is no different to what you see right no. its useless.  
[here if ur curious](https://milichf.github.io/debounclic/)

---

## what?

Your mouse button and it's inners work like such:  
The plastic button and it's inner's metal contacts touch to create a click... but they don't do it cleanly.  
And so, the contacts "bounce", registering multiple or double the clicks you performed, incorrectly.  
Modern mice handle this by adding a "debounce time", which is a minimum delay between registering clicks. Since doubleclicks happen REALLY fast, usually under 5-20ms, mice have the debounce time set to 30ms and above, so that any incorrect clicks this time do not occur. We can lower this time in your mouse's software to a lower number to get an.. unfair(?) advantage in video games...  
  
However, some mouse software do not have an option to turn down the debounce time.

---

## and?

> However, some mouse software do not have an option to turn down the debounce time.  
And as such I poorly hacked together this autohotkey script for people who cheat in video games... to make artificial double clicks.

Seriously?

## script

### 🔹 lmb

```ahk
~LButton::
{
    Click
    delay := Random(10, 20)
    Sleep delay
    Click
}
````

### 🔹 rmb

```ahk
~RButton::
{
    Click "Right"
    delay := Random(10, 20)
    Sleep delay
    Click "Right"
}
```

---

## how to use it...

1. Create a... `.ahk` file...  
  
2. paste the above rmb or lmb scripts into it...  
  
3. save it.. onto your desktop maybe..  
  
4. Press the windows key...  
  
5. type and start.. `ahk2exe`  
  
6. drag and drop your `.ahk` file onto this new ahk2exe window...  
  
7. click on the "base file" dropdown and select any version that goes something like v2.x.x...  

![ss one](https://github.com/user-attachments/assets/32f0fb19-05b9-4202-ac73-ad6a712e4295)

![ss two](https://github.com/user-attachments/assets/2c9bf244-4760-49b7-9219-b92559d932cb)

  
8. click convert...  
  
9. now you should have a .exe on your desktop.. or wherever you put the `.ahk` script.  

---

## a note

* you can paste **both scripts in one file** with a blank line in between just to be safe... if you want both LMB and RMB double-clicking, at once...  
* adjust the `delay` range if:

  * clicks aren't being registered: try `20–40` ms
  * too slow: tighten to `5–15` ms (it probably won't work this low but i havent tested idk)..  

---

## contribute?

idk, i would maybe see your pr.. but i don't think theres anything more we can do with this...  

---

## why..?

maybe you suck at stuff and want to double click to win in a game while others get their elo down...

---

# 🖱️
