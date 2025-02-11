<p align="right"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a> &nbsp; <a href="README-sv.md">Svenska</a></p>

# Contact 0.8.13

Email contact page.

<p align="center"><img src="contact-screenshot.png?raw=true" width="795" height="836" alt="Screenshot"></p>

## How to use a contact page

The contact page is available on your website as `http://website/contact/`. The webmaster receives all contact messages. The webmaster's email is defined in file `system/extensions/yellow-system.ini`. You can set a different `Author` and `Email` in the [page settings](https://github.com/datenstrom/yellow-extensions/tree/master/source/core#settings-page) at the top of a page. Please make sure that the email matches the domain name of your website.

To show a contact form on other pages use a `[contact]` shortcut. You can also add a link to the contact page somewhere on your website.

## How to restrict a contact page

If you don't want that messages are sent to anyone, then restrict emails. Open file `system/extensions/yellow-system.ini` and change `ContactEmailRestriction: 1`. All contact messages go directly to the webmaster.

If you don't want that messages with links are sent, then restrict links. Open file `system/extensions/yellow-system.ini` and change `ContactLinkRestriction: 1`. Contact messages must not contain clickable links, this blocks many unwanted messages. You can also configure keywords in the spam filter, fortunately, many spammers send the same message multiple times.

## Examples

Contact page with settings:

    ---
    Title: Contact a human
    TitleSlug: Contact
    Layout: contact
    Email: webmaster@example.com
    ---

Content file with contact form:

    ---
    Title: Example page
    ---
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna pizza. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris 
    nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit 
    esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt 
    in culpa qui officia deserunt mollit anim id est laborum.

    [contact]

Content file with contact link:

    ---
    Title: Example page
    ---
    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut 
    labore et dolore magna pizza. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris 
    nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit 
    esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt 
    in culpa qui officia deserunt mollit anim id est laborum.

    [Contact a human](/contact/).

## Settings

The following settings can be configured in file `system/extensions/yellow-system.ini`:

`Author` = name of the webmaster  
`Email` = email of the webmaster  
`ContactLocation` = contact page location  
`ContactEmailRestriction` = enable email restriction, 1 or 0  
`ContactLinkRestriction` = enable link restriction, 1 or 0  
`ContactSpamFilter` = spam filter as regular expression, `none` to disable  

The following files can be customised:

`system/layouts/contact.html` = layout file for contact page  

## Installation

[Download extension](https://github.com/datenstrom/yellow-extensions/raw/master/zip/contact.zip) and copy zip file into your `system/extensions` folder. Right click if you use Safari.

## Developer

Datenstrom. [Get help](https://datenstrom.se/yellow/help/).
