# 📄 debounclic

this is a smol-badly written-autohotkey script.... which simulates double clicks.....

---

## What?

Your mouse button and it's inners work like such:  
The plastic button and it's inner's metal contacts touch to create a click... but they don't do it cleanly.  
And so, the contacts "bounce", registering multiple or double the clicks you performed, incorrectly.  
Modern mice handle this by adding a "debounce time", which is a minimum delay between registering clicks. Since doubleclicks happen REALLY fast, usually under 5-20ms, mice have the debounce time set to 30ms and above, so that any incorrect clicks this time do not occur. We can lower this time in your mouse's software to a lower number to get an.. unfair(?) advantage in video games...  
  
However, some mouse software do not have an option to turn down the debounce time.  
We use AHK's `Random` function to **simulate human variation** and avoid robotic patterns.

---

## And?

> However, some mouse software do not have an option to turn down the debounce time.  
And as such I poorly hacked together this autohotkey script for people who cheat in video games... to make artificial double clicks.

Seriously?

## The Script

### 🔹 Left Mouse Button (LMB) Double-Click

```ahk
~LButton::
{
    Click
    delay := Random(10, 20)
    Sleep delay
    Click
}
````

### 🔹 Right Mouse Button (RMB) Double-Click

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
