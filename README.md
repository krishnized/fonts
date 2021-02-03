# fonts

Fonts with enhanced unicode combinations support, specifically cyrillics.
See [demo](https://krishnized.com/fonts).

> дхр̣тара̄шт̣ра ува̄ча<br>
> дхарма-кшетре куру-кшетре<br>
> самавета̄ йуйутсавах̣<br>
> ма̄мака̄х̣ па̄н̣д̣ава̄ш́ чаива<br>
> ким акурвата сан̃джайа

## Usage

#### Option 1.

Download font file and use font directly as replacement to original font:

```html
<style>
  @font-face {
    font-family: 'Noto Serif';
    font-style: italic;
    font-display: swap;
    src: url(./NotoSerif-Italic.otf);
  }
</style>
```

#### Option 2 (cyrillic combinations only).

Include combinations-only font file to extend original font in font stack:

```html
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif:ital@1&display=swap" rel="stylesheet">
<style>
  @font-face {
    font-family: 'VedabaseIO Noto Serif Italic';
    font-style: italic;
    font-display: swap;
    src: url(./NotoSerif-Italic-combinations.otf);
  }
  .noto-italic {
    font-family: 'VedabaseIO Noto Serif Italic', 'Noto Serif', serif;
  }
</style>
```

## Disclaimer

This repo is a fix for [google/fonts#2974](https://github.com/google/fonts/issues/2974) and alike.
Once the listed fonts get unicode cyrillic combinations support, it is recommended to switch back to original version.


<p align="center"><a href="https://github.com/krishnized">ॐ</a></p>
