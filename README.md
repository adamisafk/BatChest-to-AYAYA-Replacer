<p align="center">
  <a href="" rel="noopener">
 <img width=400px height=200px src="https://i.imgur.com/I3loGs9.png" alt="Project logo"></a>
</p>

<h3 align="center">BatChest to AYAYA Replacer</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success)]()
[![GitHub Issues](https://img.shields.io/github/issues/adamisafk/BatChest-to-AYAYA-Replacer)](https://github.com/adamisafk/BatChest-to-AYAYA-Replacer/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![GitHub Forks](https://img.shields.io/github/forks/adamisafk/BatChest-to-AYAYA-Replacer)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![License](https://img.shields.io/github/license/adamisafk/BatChest-to-AYAYA-Replacer)](/LICENSE)

</div>

---

<p align="center"> Replaces BatChest emotes with AYAYA in Twitch chat. Works even if BTTV/FFZ is not installed, or the emote hasn't been added to the channel.
    <br> 
    <b>NOTE: 7TV BREAKS THE SCRIPT (UNSURE OF CAUSE OR SOLUTION YET)</b>
</p>

## 🧰 Prerequisites <a name = "prerequisites"></a>

- A browser with extension support and capable of handling userscripts
- A userscript management extension [E.g. Tampermonkey](https://www.tampermonkey.net/)

## 🎈 Usage <a name = "usage"></a>

Assuming Tampermonkey is used, you can either:

1. Click on userscript file in GitHub and click "Raw". [Or click here.](https://github.com/adamisafk/BatChest-to-AYAYA-Replacer/raw/main/BatChest%20to%20AYAYA.user.js)
2. [Open the gist.](https://gist.github.com/adamisafk/c880514b088b16d8fcee61e7cbf22391)
3. Use Tampermonkey interface to import gist, or copy the script contents and paste it in new script creation.

## 🔧 Configuration <a name = "configuration"></a>

You can customise the emote that will get replaced, and the emote which will be used as a replacement. The default is 'BatChest' to 'AYAYA'.

First, you must find the CDN links to the emotes you want to use.
- Can find this by Right Clicking -> Inspect Element on an emote. Copy the URL in `src` attribute in the `img` element.

[On lines 26-27](https://github.com/adamisafk/BatChest-to-AYAYA-Replacer/blob/main/Larger%20Twitch%20Emotes.user.js#L26-L27), set the `ayayaSrc` to the emote URL used to replace - remove the size number (e.g. /1) <b>but keep the end `/`</b>. And set `batChest` to name of emote to be replaced (case sensitive).

```
var ayayaSrc = "https://cdn.betterttv.net/frankerfacez_emote/162146/";
var batChest = "BatChest";
```



## 📝 TODO <a name = "todo"></a>

- [ ] Fix issue with 7TV
- [ ] Provide easier way to configure emotes
- [ ] Develop Chrome/Firefox extension
- [ ] Fix any unforeseen bugs

## 🎉 Acknowledgements <a name = "acknowledgements"></a>

- Foundation of script stolen from [Corrodias' Larger Twitch Emotes userscript](https://greasyfork.org/en/scripts/419584-larger-twitch-emotes)