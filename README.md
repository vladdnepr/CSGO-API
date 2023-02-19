# Introduction

An unofficial JSON API for Counter-Strike: Global Offensive.

All data are retrieved from [items_game.txt](https://github.com/SteamDatabase/GameTracking-CSGO/blob/master/csgo/scripts/items/items_game.txt) and [csgo_english.txt](https://github.com/SteamDatabase/GameTracking-CSGO/blob/master/csgo/resource/csgo_english.txt). These files use Valve's KeyValue text file format and have to be parsed with [vdf-parser](https://github.com/p0358/vdf-parser).

## Usage

By default the data is in english, if you want to get the data in another language, you can add the language to the BASE URL.

```bash
https://bymykel.github.io/CSGO-API/api/{language?}
```

### List skins

GET [/skins.json](https://bymykel.github.io/CSGO-API/api/skins.json)

<table align="center">
  <tr>
    <td colspan="2" color="yellow">array[object]</td>
  </tr>
  <tr>
    <td width="400">id</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">name</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">description</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">weapon</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">pattern</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">min_float</td>
    <td width="400">number</td>
  </tr>
  <tr>
    <td width="400">max_float</td>
    <td width="400">number</td>
  </tr>
  <tr>
    <td width="400">rarity</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">stattrak</td>
    <td width="400">boolean</td>
  </tr>
  <tr>
    <td width="400">image</td>
    <td width="400">string</td>
  </tr>
</table>

### List stickers

GET [/stickers.json](https://bymykel.github.io/CSGO-API/api/stickers.json)

<table align="center">
  <tr>
    <td colspan="2" color="yellow">array[object]</td>
  </tr>
  <tr>
    <td width="400">id</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">name</td>
    <td width="400">string</td>
  </tr>
  <tr>
    <td width="400">description</td>
    <td width="400">string or null</td>
  </tr>
  <tr>
    <td width="400">rarity</td>
    <td width="400">string or null</td>
  </tr>
  <tr>
    <td width="400">image</td>
    <td width="400">string</td>
  </tr>