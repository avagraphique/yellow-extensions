<p align="right" role="navigation"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a></p>

Contact 0.8.13
==============
E-Mail-Kontaktseite.

<p align="center"><img src="contact-screenshot.png?raw=true" width="795" height="836" alt="Bildschirmfoto"></p>

## Wie man eine Kontaktseite benutzt

Die Kontaktseite ist auf deiner Webseite vorhanden als `http://website/contact/`. Der Webmaster erhält alle Kontaktnachrichten. Die E-Mail des Webmasters wird in der Datei `system/extensions/yellow-system.ini` festgelegt. Ganz oben auf einer Seite kannst du einen anderen `Author` und `Email` in den [Einstellungen](https://github.com/datenstrom/yellow-extensions/tree/master/source/core/README-de.md#einstellungen) festlegen. Bitte stelle sicher, dass die E-Mail mit dem Domainnamen deiner Website übereinstimmt.

Um ein Kontaktformular auf anderen Seiten anzuzeigen, benutze eine `[contact]`-Abkürzung. Du kannst auch einen Link zur Kontaktseite irgendwo auf deiner Webseite einbauen.

## Wie man eine Kontaktseite beschränkt

Falls du nicht willst dass Nachrichten an beliebige Person geschickt werden, beschränke E-Mails. Öffne die Datei `system/extensions/yellow-system.ini` und ändere `ContactEmailRestriction: 1`. Alle Kontaktnachrichten gehen dann direkt an den Webmaster.

Falls du nicht willst dass Nachrichten mit Links verschickt werden, beschränke Links. Öffne die Datei `system/extensions/yellow-system.ini` und ändere `ContactLinkRestriction: 1`. Kontaktnachrichten dürfen dann keine anklickbare Links enthalten, das blockiert viele unerwünschte Nachrichten. Du kannst ausserdem Stichwörter im Spamfilter einstellen, netterweise schicken viele Spammer die selbe Nachricht mehrfach.

## Beispiele


Kontaktseite mit Einstelungen:

    ---
    Title: Kontaktiere einen Menschen
    TitleSlug: Contact
    Layout: contact
    Email: webmaster@example.com
    ---

Inhaltsdatei mit Kontaktformular:

    ---
    Title: Beispielseite
    ---
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna pizza. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris 
    nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit 
    esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt 
    in culpa qui officia deserunt mollit anim id est laborum.

    [contact]

Inhaltsdatei mit Kontaktlink:

    ---
    Title: Über
    ---
    Für Menschen die kleine Webseiten machen. [Kontaktiere mich](/contact/).
    
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna pizza. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris 
    nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit 
    esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt 
    in culpa qui officia deserunt mollit anim id est laborum.
    
    Diese Webseite ist erstellt mit [Datenstrom Yellow](https://datenstrom.se/de/yellow/).

## Einstellungen

Die folgenden Einstellungen können in der Datei `system/extensions/yellow-system.ini` vorgenommen werden:

`Author` = Name des Webmasters  
`Email` = E-Mail des Webmasters  
`ContactLocation` = Ort der Kontaktseite  
`ContactEmailRestriction` = E-Mail-Beschränkung aktivieren, 1 oder 0  
`ContactLinkRestriction` = Linkbeschränkung aktivieren, 1 oder 0  
`ContactSpamFilter` = Spamfilter als regulärer Ausdruck, `none` um zu deaktivieren  

Die folgenden Dateien können angepasst werden:

`system/layouts/contact.html` = Layoutdatei für Kontaktseite  

## Installation

[Erweiterung herunterladen](https://github.com/datenstrom/yellow-extensions/raw/master/zip/contact.zip) und die Zip-Datei in dein `system/extensions`-Verzeichnis kopieren. Rechtsklick bei Safari.

## Entwickler

Datenstrom. [Hilfe finden](https://datenstrom.se/de/yellow/help/).
