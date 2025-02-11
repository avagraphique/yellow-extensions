<p align="right"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a> &nbsp; <a href="README-sv.md">Svenska</a></p>

# Draft 0.8.12

Stöd för draftsidor.

<p align="center"><img src="draft-screenshot.png?raw=true" width="795" height="836" alt="Skärmdump"></p>

## Hur man skapar en draftsida 

Ställ in `Status: draft` i [sidinställningar](https://github.com/datenstrom/yellow-extensions/tree/master/source/core/README-sv.md#inställningar-page) högst upp på en sida. Sidan kommer inte längre att visas. Du kan fortsätta att redigera sidan i [webbläsaren](https://github.com/datenstrom/yellow-extensions/tree/master/source/edit/README-sv.md) och filsystemet.

## Hur man hittar draftsidor

Alla draftsidor finns tillgängliga på din webbplats som `http://website/edit/drafts/`. Du kan också använda [search-tilläget](https://github.com/datenstrom/yellow-extensions/tree/master/source/search/README-sv.md). När du är inloggad med ditt användarkonto kan du söka efter `status:draft`. På så sätt kan du hitta alla draftsidor igen.

## Exempel

Innehållsfil med draft-status:

    ---
    Title: Exempelsida
    Status: draft
    ---
    Detta är ett exempelsida.

Innehållsfil med draft-status för wikin:

    ---
    Title: Wiki exempel
    Layout: wiki
    Tag: Exempel
    Status: draft
    ---
    Detta är ett exempel på en wikisida.

Innehållsfil med draft-status för bloggen:

    ---
    Title: Blogg exempel
    Published: 2013-04-07
    Author: Datenstrom
    Layout: blog
    Tag: Exempel
    Status: draft
    ---
    Detta är ett exempel på en bloggsida.

## Inställningar

Följande inställningar kan konfigureras i filen `system/extensions/yellow-system.ini`:

`DraftPaginationLimit` = antal inlägg att visa per sida  

Följande filer kan anpassas:

`system/layouts/draftpages.html` = layoutfil med översikt över draftsidor  

## Installation

[Ladda ner tillägg](https://github.com/datenstrom/yellow-extensions/raw/master/zip/draft.zip) och kopiera zip-fil till din `system/extensions` mapp. Högerklicka om du använder Safari.

## Utvecklare

Datenstrom. [Få hjälp](https://datenstrom.se/sv/yellow/help/).
