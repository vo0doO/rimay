# Rimay free theme for [Ghost](https://github.com/tryghost/ghost/)

[![Ghost version](https://img.shields.io/badge/Ghost-3.x-brightgreen.svg)](https://github.com/TryGhost/Ghost)
[![Donate](https://img.shields.io/badge/donate-paypal-blue.svg)](https://www.paypal.me/godofredoninja)
[![Buy Me A Coffee](https://img.shields.io/badge/-Buy%20Me%20A%20Coffee-%23FF813F)](https://www.buymeacoffee.com/GodoFredoNinja)

Hello :smile: , I created this theme for ghost especially for you. It is available for free so you can use on your site. If you have any suggestions to improve the theme send me a Tweet [@GodoFredoNinja](https://twitter.com/GodoFredoNinja)

## :monkey_face: I will leave my [PayPal donation link here](https://www.paypal.me/godofredoninja) and slowly move away to work on beautiful themes for Ghost

[![donate](./donate.gif)](https://www.paypal.me/godofredoninja)

[![Rimay free theme for ghost](./screenshot.jpg)](https://www.behance.net/gallery/93133463/Rimay)

## Demo

You can see Rimay in action on my Page [Demo](https://godofredo.ninja)

If for some reason I'm using a theme other than Rimay. then you can see the screenshots in [behance](https://www.behance.net/gallery/93133463/Rimay)

## Featured

- Supports English and Spanish language
- [AMP](https://github.com/godofredoninja/Hodor-AMP-Ghost) Template
- Very fast search
- Related Articles (6 articles)
- Social Media
- Page for Tags
- Support Disqus comments
- Buttons to share Post
- YouTube, Vimeo, kickstarter, dailymotion => Responsive
- Lazy load Image for better performance
- Code syntax [Prismjs](http://prismjs.com/index.html#languages-list) Supported all syntax.

## Table of Contents

- [Web Browser Support for Rimay](#web-browser-support-for-rimay)
- [Ghost Settings](#ghost-settings)
- [Rimay Settings](#rimay-settings)
  - [1. Social Media](#1-social-media)
  - [2. Footer Menu](#2-footer-menu)
  - [3. Comments](#3-comments)
  - [4. Search](#4-search)
- [Post](#post-format)
  - [Default Post](##post-format)
  - [Post Image](##post-format)
- [Archive](#tags-page)
  - [Tags](#tags-page)
- [AMP](#amp)
- [Theme Translation](#theme-translation)
- [PrismJS code syntax](#prismjs-code-syntax)

## Web Browser Support for Rimay

Rimay supports the following web [browsers](http://caniuse.com/#search=flexbox).

## Ghost Settings

Enable the following checkbox on the Labs page in the Ghost admin panel.

![ghost labs](./documentation/ghost-settings.jpg)

## Rimay Settings

> You don't have to add all the Rimay configurations. only the ones you need

### 1. Social Media

> Facebook and Twitter is not necessary because I use them from the ghost settings

Add the Social Links only for the services you want to appear in the header section of your website. Pay attention as enabling too many services will cause menu problems.

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
var followSocialMedia = {
  'youtube': ['YOUR_URL','YOUR_TITLE'],
  'instagram': ['YOUR_URL','YOUR_TITLE'],
  'github': ['YOUR_URL','YOUR_TITLE'],
  'pinterest': ['YOUR_URL','YOUR_TITLE'],
  'linkedin': ['YOUR_URL','YOUR_TITLE'],
  'rss': ['YOUR_URL','YOUR_TITLE'],

  /*
  'snapchat': ['YOUR_URL','YOUR_TITLE'],
  'dribbble': ['YOUR_URL','YOUR_TITLE'],
  'spotify': ['YOUR_URL','YOUR_TITLE'],
  'codepen': ['YOUR_URL','YOUR_TITLE'],
  'behance': ['YOUR_URL','YOUR_TITLE'],
  'flickr': ['YOUR_URL','YOUR_TITLE'],
  'telegram': ['YOUR_URL','YOUR_TITLE'],
  'vimeo': ['YOUR_URL','YOUR_TITLE'],
  'twitch': ['YOUR_URL','YOUR_TITLE'],
  'vk': ['YOUR_URL','YOUR_TITLE'],
  'slack': ['YOUR_URL','YOUR_TITLE'],
  'tumblr': ['YOUR_URL','YOUR_TITLE'],
  'discord': ['YOUR_URL','YOUR_TITLE'],
  */
};
</script>
```

:point_right: For those who are commented it is necessary to add those icons through `SVG`

It is not necessary to add all the icons. Only the icons you need.

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<svg aria-hidden="true" style="position: absolute; width: 0; height: 0; overflow: hidden;" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <defs>
        <!-- discord -->
        <symbol id="icon-discord" viewBox="0 0 24 24">
        <title>discord</title>
        <path d="M20.222 0c1.406 0 2.54 1.137 2.607 2.475v21.525l-2.677-2.273-1.47-1.338-1.604-1.398 0.67 2.205h-14.038c-1.402 0-2.54-1.065-2.54-2.476v-16.24c0-1.338 1.14-2.477 2.545-2.477l16.507-0.003zM14.104 5.683h-0.030l-0.202 0.2c2.073 0.6 3.076 1.537 3.076 1.537-1.336-0.668-2.54-1.002-3.744-1.137-0.87-0.135-1.74-0.064-2.475 0h-0.2c-0.47 0-1.47 0.2-2.81 0.735-0.467 0.203-0.735 0.336-0.735 0.336s1.002-1.002 3.21-1.537l-0.135-0.135s-1.672-0.064-3.477 1.27c0 0-1.805 3.144-1.805 7.020 0 0 1 1.74 3.743 1.806 0 0 0.4-0.533 0.805-1.002-1.54-0.468-2.14-1.404-2.14-1.404s0.134 0.066 0.335 0.2h0.060c0.030 0 0.044 0.015 0.060 0.030v0.006c0.016 0.016 0.030 0.030 0.060 0.030 0.33 0.136 0.66 0.27 0.93 0.4 0.466 0.202 1.065 0.403 1.8 0.536 0.93 0.135 1.996 0.2 3.21 0 0.6-0.135 1.2-0.267 1.8-0.535 0.39-0.2 0.87-0.4 1.397-0.737 0 0-0.6 0.936-2.205 1.404 0.33 0.466 0.795 1 0.795 1 2.744-0.060 3.81-1.8 3.87-1.726 0-3.87-1.815-7.020-1.815-7.020-1.635-1.214-3.165-1.26-3.435-1.26l0.056-0.020zM14.272 10.096c0.703 0 1.27 0.6 1.27 1.335 0 0.74-0.57 1.34-1.27 1.34s-1.27-0.6-1.27-1.334c0.002-0.74 0.573-1.338 1.27-1.338zM9.729 10.096c0.7 0 1.266 0.6 1.266 1.335 0 0.74-0.57 1.34-1.27 1.34s-1.27-0.6-1.27-1.334c0-0.74 0.57-1.338 1.27-1.338z"></path>
        </symbol>
        <!-- flickr -->
        <symbol id="icon-flickr" viewBox="0 0 21 24">
        <title>flickr</title>
        <path d="M16.714 1.714c2.129 0 3.857 1.728 3.857 3.857v12.857c0 2.129-1.728 3.857-3.857 3.857h-12.857c-2.129 0-3.857-1.728-3.857-3.857v-12.857c0-2.129 1.728-3.857 3.857-3.857h12.857zM9.348 12c0-1.567-1.272-2.839-2.839-2.839s-2.839 1.272-2.839 2.839 1.272 2.839 2.839 2.839 2.839-1.272 2.839-2.839zM16.902 12c0-1.567-1.272-2.839-2.839-2.839s-2.839 1.272-2.839 2.839 1.272 2.839 2.839 2.839 2.839-1.272 2.839-2.839z"></path>
        </symbol>
        <!-- tumblr -->
        <symbol id="icon-tumblr" viewBox="0 0 15 24">
        <title>tumblr</title>
        <path d="M12.643 17.799l1.071 3.174c-0.402 0.603-2.223 1.286-3.857 1.313-4.862 0.080-6.696-3.455-6.696-5.946v-7.286h-2.25v-2.879c3.375-1.219 4.192-4.272 4.379-6.013 0.013-0.107 0.107-0.161 0.161-0.161h3.268v5.679h4.46v3.375h-4.473v6.938c0 0.938 0.348 2.237 2.143 2.196 0.589-0.013 1.379-0.188 1.795-0.388z"></path>
        </symbol>
        <!-- dribbble -->
        <symbol id="icon-dribbble" viewBox="0 0 21 24">
        <title>dribbble</title>
        <path d="M13.714 20.089c-0.134-0.777-0.643-3.455-1.875-6.67-0.013 0-0.040 0.013-0.054 0.013 0 0-5.21 1.821-6.897 5.491-0.080-0.067-0.201-0.147-0.201-0.147 1.527 1.246 3.469 2.009 5.598 2.009 1.219 0 2.371-0.254 3.429-0.696zM11.237 11.96c-0.214-0.496-0.455-0.991-0.71-1.487-4.527 1.353-8.866 1.246-9.013 1.246-0.013 0.094-0.013 0.188-0.013 0.281 0 2.25 0.857 4.313 2.25 5.866v0c2.397-4.272 7.138-5.799 7.138-5.799 0.121-0.040 0.241-0.067 0.348-0.107zM9.804 9.121c-1.527-2.705-3.147-4.902-3.268-5.063-2.451 1.152-4.272 3.415-4.848 6.134 0.228 0 3.897 0.040 8.116-1.071zM18.964 13.393c-0.188-0.054-2.638-0.83-5.478-0.388 1.152 3.174 1.621 5.759 1.714 6.281 1.969-1.326 3.362-3.442 3.763-5.893zM8.183 3.469c-0.013 0-0.013 0-0.027 0.013 0 0 0.013-0.013 0.027-0.013zM16.085 5.411c-1.54-1.366-3.576-2.196-5.799-2.196-0.71 0-1.406 0.094-2.076 0.254 0.134 0.174 1.795 2.357 3.295 5.116 3.308-1.232 4.554-3.134 4.58-3.174zM19.071 11.906c-0.027-2.076-0.763-3.991-1.996-5.491-0.027 0.027-1.433 2.063-4.902 3.482 0.201 0.415 0.402 0.844 0.589 1.272 0.067 0.147 0.121 0.308 0.188 0.455 3.027-0.388 6.013 0.268 6.121 0.281zM20.571 12c0 5.679-4.607 10.286-10.286 10.286s-10.286-4.607-10.286-10.286 4.607-10.286 10.286-10.286 10.286 4.607 10.286 10.286z"></path>
        </symbol>
        <!-- vk -->
        <symbol id="icon-vk" viewBox="0 0 26 24">
        <title>vk</title>
        <path d="M25.674 6.964c0.201 0.549-0.429 1.835-2.009 3.938-2.598 3.455-2.879 3.134-0.737 5.129 2.062 1.915 2.491 2.839 2.558 2.96 0 0 0.857 1.5-0.951 1.513l-3.429 0.054c-0.737 0.147-1.714-0.522-1.714-0.522-1.286-0.884-2.491-3.174-3.429-2.879 0 0-0.964 0.308-0.938 2.371 0.013 0.442-0.201 0.683-0.201 0.683s-0.241 0.254-0.71 0.295h-1.54c-3.388 0.214-6.375-2.906-6.375-2.906s-3.268-3.375-6.134-10.112c-0.188-0.442 0.013-0.656 0.013-0.656s0.201-0.254 0.763-0.254l3.67-0.027c0.348 0.054 0.589 0.241 0.589 0.241s0.214 0.147 0.321 0.429c0.603 1.5 1.379 2.866 1.379 2.866 1.339 2.759 2.25 3.228 2.772 2.946 0 0 0.683-0.415 0.536-3.75-0.054-1.205-0.388-1.754-0.388-1.754-0.308-0.415-0.884-0.536-1.138-0.576-0.201-0.027 0.134-0.509 0.576-0.723 0.656-0.321 1.821-0.335 3.201-0.321 1.085 0.013 1.393 0.080 1.808 0.174 1.272 0.308 0.844 1.487 0.844 4.326 0 0.911-0.174 2.183 0.482 2.598 0.281 0.188 0.978 0.027 2.692-2.893 0 0 0.804-1.393 1.433-3.013 0.107-0.295 0.335-0.415 0.335-0.415s0.214-0.121 0.509-0.080l3.857-0.027c1.165-0.147 1.353 0.388 1.353 0.388z"></path>
        </symbol>
        <!-- slack -->
        <symbol id="icon-slack" viewBox="0 0 22 24">
        <title>slack</title>
        <path d="M20.344 10.393c1.098 0 1.942 0.804 1.942 1.902 0 0.857-0.442 1.46-1.246 1.741l-2.304 0.79 0.75 2.237c0.067 0.201 0.094 0.415 0.094 0.629 0 1.058-0.857 1.942-1.915 1.942-0.844 0-1.594-0.522-1.862-1.326l-0.737-2.21-4.152 1.42 0.737 2.196c0.067 0.201 0.107 0.415 0.107 0.629 0 1.045-0.857 1.942-1.929 1.942-0.844 0-1.58-0.522-1.848-1.326l-0.737-2.183-2.049 0.71c-0.214 0.067-0.442 0.121-0.67 0.121-1.085 0-1.902-0.804-1.902-1.888 0-0.83 0.536-1.58 1.326-1.848l2.089-0.71-1.406-4.192-2.089 0.723c-0.214 0.067-0.429 0.107-0.643 0.107-1.071 0-1.902-0.817-1.902-1.888 0-0.83 0.536-1.58 1.326-1.848l2.103-0.71-0.71-2.129c-0.067-0.201-0.107-0.415-0.107-0.629 0-1.058 0.857-1.942 1.929-1.942 0.844 0 1.58 0.522 1.848 1.326l0.723 2.143 4.152-1.406-0.723-2.143c-0.067-0.201-0.107-0.415-0.107-0.629 0-1.058 0.871-1.942 1.929-1.942 0.844 0 1.594 0.536 1.862 1.326l0.71 2.156 2.17-0.737c0.188-0.054 0.375-0.080 0.576-0.080 1.045 0 1.942 0.777 1.942 1.848 0 0.83-0.643 1.527-1.393 1.781l-2.103 0.723 1.406 4.232 2.196-0.75c0.201-0.067 0.415-0.107 0.616-0.107zM9.71 13.902l4.152-1.406-1.406-4.219-4.152 1.433z"></path>
        </symbol>
        <!-- behance -->
        <symbol id="icon-behance" viewBox="0 0 21 24">
        <title>behance</title>
        <path d="M16.714 1.714c2.129 0 3.857 1.728 3.857 3.857v12.857c0 2.129-1.728 3.857-3.857 3.857h-12.857c-2.129 0-3.857-1.728-3.857-3.857v-12.857c0-2.129 1.728-3.857 3.857-3.857h12.857zM6.683 6.629h-4.969v10.54h5.116c1.915 0 3.71-0.911 3.71-3.054 0-1.326-0.629-2.304-1.915-2.679 0.938-0.455 1.433-1.138 1.433-2.196 0-2.103-1.567-2.612-3.375-2.612zM6.388 10.888h-2.357v-2.464h2.183c0.83 0 1.594 0.228 1.594 1.205 0 0.897-0.589 1.259-1.42 1.259zM6.509 15.375h-2.478v-2.906h2.531c1.018 0 1.661 0.442 1.661 1.513s-0.763 1.393-1.714 1.393zM15.214 15.804c-1.232 0-1.875-0.723-1.875-1.942h5.504c0.013-0.134 0.013-0.268 0.013-0.402 0-2.25-1.326-4.138-3.723-4.138-2.317 0-3.911 1.754-3.911 4.045 0 2.384 1.5 4.004 3.911 4.004 1.835 0 3.013-0.817 3.576-2.558h-1.848c-0.201 0.643-1.018 0.991-1.647 0.991zM15.080 10.902c1.045 0 1.567 0.629 1.661 1.634h-3.402c0.067-1.004 0.737-1.634 1.741-1.634zM12.911 7.339h4.272v1.031h-4.272v-1.031z"></path>
        </symbol>
        <!-- spotify -->
        <symbol id="icon-spotify" viewBox="0 0 21 24">
        <title>spotify</title>
        <path d="M15.094 16.205c0-0.375-0.147-0.522-0.402-0.683-1.728-1.031-3.737-1.54-5.987-1.54-1.313 0-2.571 0.174-3.844 0.455-0.308 0.067-0.563 0.268-0.563 0.696 0 0.335 0.254 0.656 0.656 0.656 0.121 0 0.335-0.067 0.496-0.107 1.045-0.214 2.143-0.362 3.254-0.362 1.969 0 3.83 0.482 5.317 1.379 0.161 0.094 0.268 0.147 0.442 0.147 0.335 0 0.629-0.268 0.629-0.643zM16.379 13.326c0-0.362-0.134-0.616-0.469-0.817-2.049-1.219-4.647-1.888-7.339-1.888-1.728 0-2.906 0.241-4.058 0.563-0.429 0.121-0.643 0.415-0.643 0.857s0.362 0.804 0.804 0.804c0.188 0 0.295-0.054 0.496-0.107 0.938-0.254 2.063-0.442 3.362-0.442 2.545 0 4.862 0.67 6.536 1.661 0.147 0.080 0.295 0.174 0.509 0.174 0.455 0 0.804-0.362 0.804-0.804zM17.826 10.004c0-0.496-0.214-0.75-0.536-0.938-2.317-1.353-5.491-1.982-8.518-1.982-1.781 0-3.415 0.201-4.875 0.629-0.375 0.107-0.723 0.429-0.723 0.991 0 0.549 0.415 0.978 0.964 0.978 0.201 0 0.388-0.067 0.536-0.107 1.299-0.362 2.705-0.496 4.112-0.496 2.786 0 5.679 0.616 7.54 1.728 0.188 0.107 0.321 0.161 0.536 0.161 0.509 0 0.964-0.402 0.964-0.964zM20.571 12c0 5.679-4.607 10.286-10.286 10.286s-10.286-4.607-10.286-10.286 4.607-10.286 10.286-10.286 10.286 4.607 10.286 10.286z"></path>
        </symbol>
        <!-- codepen -->
        <symbol id="icon-codepen" viewBox="0 0 24 24">
        <title>codepen</title>
        <path d="M2.893 15.656l8.076 5.384v-4.808l-4.473-2.987zM2.063 13.728l2.585-1.728-2.585-1.728v3.455zM13.031 21.040l8.076-5.384-3.603-2.411-4.473 2.987v4.808zM12 14.438l3.643-2.438-3.643-2.438-3.643 2.438zM6.496 10.754l4.473-2.987v-4.808l-8.076 5.384zM19.353 12l2.585 1.728v-3.455zM17.504 10.754l3.603-2.411-8.076-5.384v4.808zM24 8.344v7.313c0 0.335-0.174 0.67-0.455 0.857l-10.969 7.313c-0.174 0.107-0.375 0.174-0.576 0.174s-0.402-0.067-0.576-0.174l-10.969-7.313c-0.281-0.188-0.455-0.522-0.455-0.857v-7.313c0-0.335 0.174-0.67 0.455-0.857l10.969-7.313c0.174-0.107 0.375-0.174 0.576-0.174s0.402 0.067 0.576 0.174l10.969 7.313c0.281 0.188 0.455 0.522 0.455 0.857z"></path>
        </symbol>
        <!-- twitch -->
        <symbol id="icon-twitch" viewBox="0 0 24 24">
        <title>twitch</title>
        <path d="M12 5.813v5.813h-1.942v-5.813h1.942zM17.33 5.813v5.813h-1.942v-5.813h1.942zM17.33 15.991l3.388-3.402v-10.647h-15.991v14.049h4.366v2.906l2.906-2.906h5.33zM22.661 0v13.567l-5.813 5.813h-4.366l-2.906 2.906h-2.906v-2.906h-5.33v-15.509l1.46-3.871h19.862z"></path>
        </symbol>
        <!-- vimeo -->
        <symbol id="icon-vimeo" viewBox="0 0 24 24">
        <title>vimeo</title>
        <path d="M22.888 6.938c-0.094 2.116-1.58 5.022-4.446 8.719-2.973 3.844-5.464 5.772-7.527 5.772-1.272 0-2.344-1.179-3.214-3.522-0.589-2.143-1.179-4.299-1.768-6.455-0.643-2.344-1.353-3.509-2.103-3.509-0.161 0-0.723 0.335-1.701 1.018l-1.031-1.313c1.071-0.951 2.129-1.915 3.188-2.839 1.42-1.259 2.504-1.888 3.228-1.955 1.701-0.161 2.732 0.991 3.134 3.469 0.415 2.679 0.723 4.353 0.884 4.996 0.496 2.223 1.018 3.335 1.607 3.335 0.455 0 1.138-0.71 2.063-2.156 0.911-1.446 1.393-2.545 1.46-3.295 0.121-1.246-0.362-1.862-1.46-1.862-0.522 0-1.058 0.121-1.621 0.348 1.071-3.509 3.121-5.21 6.147-5.116 2.237 0.067 3.295 1.527 3.161 4.366z"></path>
        </symbol>
        <!-- snapchat -->
        <symbol id="icon-snapchat" viewBox="0 0 22 24">
        <title>snapchat</title>
        <path d="M11.357 1.714c2.411-0.027 4.406 1.326 5.411 3.496 0.308 0.656 0.362 1.674 0.362 2.397 0 0.857-0.067 1.701-0.121 2.558 0.107 0.054 0.254 0.094 0.375 0.094 0.482 0 0.884-0.362 1.366-0.362 0.455 0 1.112 0.321 1.112 0.857 0 1.286-2.692 1.045-2.692 2.17 0 0.201 0.080 0.388 0.161 0.576 0.643 1.406 1.862 2.759 3.308 3.362 0.348 0.147 0.696 0.228 1.071 0.308 0.241 0.054 0.375 0.228 0.375 0.469 0 0.911-2.317 1.286-2.933 1.379-0.268 0.415-0.067 1.393-0.777 1.393-0.549 0-1.098-0.174-1.688-0.174-0.281 0-0.563 0.013-0.83 0.067-1.594 0.268-2.129 1.982-4.741 1.982-2.518 0-3.121-1.714-4.674-1.982-0.281-0.054-0.563-0.067-0.844-0.067-0.603 0-1.179 0.201-1.661 0.201-0.75 0-0.522-0.991-0.804-1.42-0.616-0.094-2.933-0.469-2.933-1.379 0-0.241 0.134-0.415 0.375-0.469 0.375-0.080 0.723-0.161 1.071-0.308 1.433-0.589 2.679-1.955 3.308-3.362 0.080-0.188 0.161-0.375 0.161-0.576 0-1.125-2.705-0.911-2.705-2.156 0-0.522 0.616-0.857 1.085-0.857 0.415 0 0.83 0.348 1.353 0.348 0.147 0 0.295-0.027 0.429-0.094-0.054-0.844-0.121-1.688-0.121-2.545 0-0.723 0.054-1.754 0.362-2.411 1.179-2.545 3.174-3.469 5.839-3.496z"></path>
        </symbol>
        <!-- telegram -->
        <symbol id="icon-telegram" viewBox="0 0 24 24">
        <title>telegram</title>
        <path d="M15.924 17.504l1.969-9.281c0.174-0.817-0.295-1.138-0.83-0.938l-11.571 4.46c-0.79 0.308-0.777 0.75-0.134 0.951l2.96 0.924 6.871-4.326c0.321-0.214 0.616-0.094 0.375 0.121l-5.558 5.022-0.214 3.054c0.308 0 0.442-0.134 0.603-0.295l1.446-1.393 3 2.21c0.549 0.308 0.938 0.147 1.085-0.509zM24 12c0 6.629-5.371 12-12 12s-12-5.371-12-12 5.371-12 12-12 12 5.371 12 12z"></path>
        </symbol>
    </defs>
</svg>
```

### 2. Footer Menu

You can add an additional menu bar at the footer of the page

:arrow_right: `Dashboard -> Design -> Secondary Navigation`

### 3. Comments

Rimay supports Disqus comments as well as comment counting

— First, you will need to get your account `disqusShortName`

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
var disqusShortName = 'YOUR_DISQUS_SHORTCUT_HERE';
</script>
```

### 4. Search

> The default search engine will only search the titles of the post

**Setup a Custom integration**

1. Go in your Ghost's `dashboard -> Integrations -> Add custom integration`
2. Set a name: `GodoFredo Themes Search`
3. Get the Content API Key and replace the demo key with this one
4. Get the admin domain. This will be different in some cases

![ghost api](./documentation/ghost-api.jpg)

:arrow_right: `Dashboard -> Code injection -> Site Footer`

```html
<script>
  var searchSettings = {
    key: 'ADD_YOUR_API_KEY',
    url: 'https://demo.ghost.io',
  };
</script>
```

OR - Adding parameters to the search

```html
<script>
var searchSettings = {
  key: 'ADD_YOUR_API_KEY',
  url: 'https://demo.ghost.io',
  /* This is optional */
  options: {
    keys: [
        'title',
    ],
    limit: 10,
  },
  /* This is optional to perform filtering of the ghost api */
  api: {
    resource: 'posts',
    parameters: {
      limit: 'all',
      fields: ['title', 'slug'],
      filter: '',
      include: '',
      order: '',
      formats: '',
    },
  },
}
</script>
```

The search engine that includes Rimay is very powerful, supports almost all languages and you can customize to your liking.

Read more about the search engine [Read More](https://github.com/HauntedThemes/ghost-search)

## Post Format

 > Rimay has different templates for post formats. I will mention some of them.

 1. **Default Post** — Includes the featured image at the top.

 2. **Post Image** — This template will have a very large featured image and the header background will also be transparent.

### Tags Page

> A page will be displayed with all tags sorted from highest to lowest number of articles.

- Create a new page
- Choose your favorite url and title
- Template dropdown -> Select `Archive Tags`
- Publish the page
- To add the page to the navigation

## AMP

— *Rimay has a nice page for **AMP***

- Navigation
- links to followers in social media
- Tags
- Related Articles (6 articles)
- Buttons to share the article (Facebook - Twitter - Whatsapp)

To customize the AMP page [read here](https://github.com/godofredoninja/Hodor-AMP-Ghost)

## Theme Translation

**Rimay supports:**

- `en` — English default language
- `es` — Spanish

![Publication Language for ghost](./documentation/language.jpg)

if you want to have in another language you just have to copy `locales>en.json` and rename the file then translate to your favorite language:

Just enter the [language/locale tag](https://www.w3schools.com/tags/ref_language_codes.asp) of the files to use (e.g.: `fr.json` for French, `zh.json` for Chinese, `ja.json` for Japanese)


### PrismJS code syntax

Make your code stand out. WIth the PrismJS code highlighter. PrismJS allows you to select which languge you embeded and performs code highlighting according to the language. Neat!

Take a look at the [Prismjs Supported Language List](http://prismjs.com/#languages-list) to find your coding language.

### Credits

- [Hodor AMP](https://github.com/godofredoninja/Hodor-AMP-Ghost)
- [Normalize](https://necolas.github.io/normalize.css/)
- [Ghost Search](https://github.com/HauntedThemes/ghost-search)
- [Prismjs](http://prismjs.com/)
- [Medium Zoom](https://github.com/francoischalifour/medium-zoom)
- [Lazysizes](https://github.com/aFarkas/lazysizes)
- [Fonts](https://fonts.google.com/?query=domine&selection.family=Rubik)
- [Safari Light - Mockup](https://www.uplabs.com/posts/safari-light-version)

## Copyright & License

Copyright (c) 2020 GodoFredo - Released under the [GPLv3 license](LICENSE)
