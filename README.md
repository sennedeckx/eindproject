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

- Clone deze repo `git clone https://github.com/pverhaert/1ITF_Sass_BS4_project.git <project naam>`
- Open een nieuw terminalvenster in de map **project naam** en installeer de node-modules: `npm install`
- Kopieer de **jQuery.min.js** en **bootstrap.bundle.min.js** naar de map **public_html/js**: `gulp js`
- Start de Sass-compiler: `gulp`

## CSS-bestand optimaliseren voor productie!

 Het CSS-bestand in dit project zijn nog niet geoptimaliseerd voor productie. 
 De code is immers nog geëxpandeerd en bevat een source-map om vlot te debuggen.
 
Om de bestanden sneller te laden moet je zeker de gegenereerde CSS-code minimaliseren. Dit doe je als volgt:

- Stop de default gulp-task: `Ctrl + c`
- Minimaliseer de CSS-code: `gulp build`
- Upload de CSS-bestanden naar de webserver
- Start de default gulp-task: `gulp`

Het originele CSS-bestand van **600 kB** is na optimalisatie nog naar **120 kB** groot!!!


# Stappenplan voor een nieuwe team website op basis van dit project

Werk je met twee of meer teamleden aan hetzelfde project, dan volg je best deze werkwijze. Begin alvast met een teamleader 🎓 aan te duiden en een naam voor het project te kiezen.

### Opzetten van een lokale repo door de teamleader 🎓

**De overige teamleden 👤👤 doen voorlopig nog niets!**

1. Clone deze repo `git clone https://github.com/pverhaert/1ITF_Sass_BS4_project.git projectNaam`
2. `cd projectNaam`
3. Wis de map **.git**
4. Initialiseer een nieuwe Git-repo `git init`
5. Voeg alle bestanden (uitgezonderd deze die zijn uitgesloten via **.gitignore**) uit deze map aan de staging area toe   `git add .`
6. Verplaats de bestanden van de staging area naar de lokale repo `git commit -m "First commit"`

### Opzetten van een remote repo door de teamleader 🎓

1. Maak een nieuwe, lege, (private) repo **projectNaam** op Github   
(dus zonder ***.gitignore*** en zonder ***README***!)
2. Verbind de lokale repo met de remote repo `git remote add <remote‐name> <remote‐url>`   
bv: `git remote add origin https://github.com/teamleader/projectNaam.git`
3. Push de lokale repo naar de remote repo `git push ‐u origin master`

### Teamleader 🎓 nodigt andere teamleden 👤👤 uit voor samenwerking

1. Klik op de pagina **https://github.com/teamleader/projectNaam** op ***settings***
2. Klik links in het menu op ***Collaborators***
3. Nodig overige teamleden 👤👤 uit

### Teamleden 👤👤 clonen van een remote repo

1. Elk teamlid maakt een exacte copy van de remote repo `git clone https://github.com/teamleader/projectNaam.git`

Proficiat! De samenwerking kan beginnen.

### Stagen en committen van lokaal gewijzigde bestanden 🎓👤👤

Maak regelmatig back-ups zodat de ander teamleden weten waar je mee bezig bent.   
Wacht dus niet te lang met wijzigingen op Github te plaatsen. 

1. Controleer de status `git status`
2. Voeg alle wijzigingen aan de staging area toe `git add .`
3. Verplaats de bestanden van de staging area naar de lokale repo `git commit -m "Comment"`
4. Push de lokale repo naar de remote repo `git push --rebase`






