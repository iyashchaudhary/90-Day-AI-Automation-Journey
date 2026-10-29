# Week 2 Debugging Masterclass — JSON & API Errors

## Common Errors & Fixes
| Problem / Error | Why It Happens | How To Fix It |
|---|---|---|
| "Cannot GET /xyz" or blank response | Endpoint URL typo, trailing slash mismatch | Docs se exact copy karo; extra slash check karo |
| CORS error in browser console | Server browser direct call allow nahi karta | Browser band karo; Postman ya n8n use karo |
| JSON.parse() style errors | Response valid JSON nahi tha (HTML error page aaya) | Raw response print karke status code check karo |
| "undefined" in nested data | Key exist nahi karti ya path galat hai | Poora JSON print karo aur exact path trace karo |
| Request hangs / never responds | Wrong URL, internet issue, API temporarily down | Browser me URL daal kar check karo, thoda wait karo |
| Extra/missing comma in JSON | Syntax invalid ho gaya | VS Code red squiggle dekho ya jsonlint.com use karo |

## The 4-Step Debugging Method
1. READ: Error message ko dhyan se poora padho (90% answer message me hi hota hai).
2. CHECK: Exact URL, JSON brackets, commas, aur parameters character-by-character verify karo.
3. ISOLATE: Sabse chhota single piece (sirf ek endpoint) test karo poore flow ke bajaye.
4. SEARCH / ASK: Error copy-paste karke AI se ya docs me search karo.