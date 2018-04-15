# 1ITF Sass-BS4-project
Dit is een basiswebsite voor de les **Sass** met **Bootstrap 4** in 1ITF van de Thomas More Hogeschool (campus Geel).

<p align="center">
    <img src="https://www.thomasmore.be/themes/wundertheme/logo.svg" alt="Thomasm More Kempen" width="300" />
</p>

## Basisvereisten (eenmalig te installeren)

Volgende tools hoef je maar eenmalig te installeren:

- De hoogste versie van [**Node**](https://nodejs.org/en/)
- [**Git**](https://git-scm.com/)
- [**gulp-cli**](https://gulpjs.com/): `npm install -g gulp-cli`

## Een nieuw Sass-BS4-project starten

- Download of clone deze repo `git clone https://github.com/pverhaert/1ITF_Sass_BS4_project.git <project naam>`
- Open een nieuw terminalvenster in de map **project naam** en installeer de node-modules: `npm install`
- Kopieer de **jQuery.min.js** en **bootstrap.bundle.min.js** naar de map **public_html/js**: `gulp js`
- Start de Sass-compiler: `gulp`

## CSS-bestanden optimaliseren voor productie!

 Het CSS-bestand in dit project zijn nog niet geoptimaliseerd voor productie. 
 De code is immers nog geëxpandeerd en bevat een source-map om vlot te debuggen.
 
Om de bestanden sneller te laden moet je zeker de gegenereerde CSS-code minimaliseren. Dit doe je als volgt:

- Stop de default gulp-task: `Ctrl + c`
- Minimaliseer de CSS-code: `gulp build`
- Upload de CSS-bestanden naar de webserver
- Start de default gulp-task: `gulp build`

Het originele CSS-bestand van **600 kB** is na optimalisatie nog naar **120 kB** groot!!!
