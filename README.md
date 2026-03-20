# Nowruz 1405 Countdown

Countdown timer for Persian New Year (Nowruz 1405) with voice countdown and fireworks.

## Test locally

Paste in browser Console to test with a 1 min countdown:

```js
var s=document.querySelector('script').textContent.replace('2026-03-20T14:45:59Z',new Date(Date.now()+60000).toISOString().split('.')[0]+'Z');document.querySelector('script').remove();document.querySelectorAll('#main,#message,#overlay,canvas').forEach(e=>e.remove());document.body.insertAdjacentHTML('beforeend','<div id="main"><div id="countdown"></div><div id="tahvil"></div></div><div id="message"><h1>سال ۱۴۰۵ مبارک</h1><br><p id="tahvil-time"></p></div><canvas id="fireworks"></canvas><div id="overlay"></div>');eval(s);
```
