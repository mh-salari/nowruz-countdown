# Nowruz 1405 Countdown

Countdown timer for Persian New Year (Nowruz 1405) with voice countdown and fireworks.

## Test locally

Paste in browser Console to test with a 1 min countdown:

```js
var s=document.querySelector('script').textContent.replace('2026-03-20T14:45:59Z',new Date(Date.now()+60000).toISOString().split('.')[0]+'Z').replace('var audioUnlocked = false','var audioUnlocked = true');document.querySelector('script').remove();document.querySelectorAll('#main,#message,#overlay,canvas,#audio-prompt').forEach(e=>e.remove());document.body.insertAdjacentHTML('beforeend','<div id="main"><div id="countdown"></div><div id="tahvil"></div></div><div id="message"><h1>سال ۱۴۰۵ مبارک</h1><br><p id="tahvil-time"></p></div><canvas id="fireworks"></canvas><div id="overlay"></div><div id="audio-prompt" class="hidden"></div>');eval(s);
```

Note: on Safari/iOS you may still need to click the page once after running this for audio to work.

## Credits

Favicon icon by [Maryam Khoshbakht](https://dribbble.com/shots/23615077-Happy-Nowruz) on Dribbble.
