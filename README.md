# 🔗 Fun Bookmarklets Hub

A tiny collection of safe, fun bookmarklets you can drop into your bookmarks bar and run on any page.  
Save them as bookmarks (drag the link to your bookmarks bar or create a new bookmark and paste the `javascript:` URL into the URL field).

---

## How to use

1. Right-click your bookmarks bar → **Add page** (or drag the `javascript:` link into the bar).  
2. Give it a name (example: `Rainbow Mode`).  
3. Paste the `URL` value from the list below (starts with `javascript:`).  
4. Visit any page and click the bookmarklet to run it.

> **Note:** Some pages with very strict CSP (Content Security Policy) may block bookmarklets. These scripts are purely client-side and safe — they only modify things in your browser.

---

## Bookmarklets

> Click the code to copy it (or copy from the triple-backtick blocks).

### 🎨 Rainbow Mode — animate page background
A playful background color cycle.

```text
javascript:(function(){let i=0;const el=document.documentElement, id=setInterval(()=>{el.style.background=`hsl(${i%360} 60% 85%)`; i+=10;},120); setTimeout(()=>clearInterval(id),15000);})();
