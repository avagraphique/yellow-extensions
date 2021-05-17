<p align="right" role="navigation"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a></p>

Slider 0.8.11
=============
Image gallery with slider.

<p align="center"><img src="slider-screenshot.png?raw=true" width="795" height="836" alt="Screenshot"></p>

## How to add an image gallery

Create a `[slider]` shortcut.

The following arguments are available, all but the first argument are optional:
  
`Pattern` = file name as regular expression  
`Style` = gallery style, e.g. `flickity`  
`Size` = image size, pixel or percent  
`Autoplay` = play images automatically, delay time in milliseconds  

The image formats GIF, JPG, PNG and SVG are supported. All media files are located in the `media` folder. The `media/images` folder is the place to store your images. The `media/thumbnails` folder contains image thumbnails. You can also create additional folders and organise files as you like.

## Examples

Adding an image gallery:

    [slider photo.*jpg]
    [slider photo.*jpg - 20%]
    [slider photo.*jpg simple 20%]

Adding an image gallery, play automatically:

    [slider photo.*jpg - - 1000]
    [slider photo.*jpg - - 5000]
    [slider photo.*jpg - 20% 5000]

Adding an image gallery from a subfolder, play automatically:

    [slider photo-album/ - - 1000]
    [slider photo-album/ - - 5000]
    [slider photo-album/ - 20% 5000]

## Settings

The following settings can be configured in file `system/extensions/yellow-system.ini`:

`SliderStyle` = gallery style, e.g. `flickity`  
`SliderAutoplay` = play images automatically, delay time in milliseconds  

## Installation

[Download extension](https://github.com/datenstrom/yellow-extensions/raw/master/zip/slider.zip) and copy zip file into your `system/extensions` folder. Right click if you use Safari.

This extension uses [Flickity 2.0.9](https://github.com/metafizzy/flickity) by David DeSandro.

## Developer

Datenstrom. [Get help](https://datenstrom.se/yellow/help/).
