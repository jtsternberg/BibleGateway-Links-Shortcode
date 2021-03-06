# BibleGateway Links Shortcode

**Contributors:** jtsternberg  
**Plugin Name:** BibleGateway Links Shortcode  
**Plugin URI:** http://dsgnwrks.pro/plugins/biblegateway-search-shortcode  
**Tags:** shortcode, bible, biblegateway, editor, button, scripture, reference, search, youversion  
**Author URI:** http://about.me/jtsternberg  
**Author:** Jtsternberg  
**Donate link:** http://j.ustin.co/rYL89n  
**Requires at least:** 3.2  
**Tested up to:** 3.8  
**Stable tag:** 0.1.5  
**Version:** 0.1.5  
**License:** GPLv2 or later  
**License URI:** http://www.gnu.org/licenses/gpl-2.0.html  

Shortcode for linking Bible references to a BibleGateway page.

## Description

Shortcode for linking Bible references to a BibleGateway page. Links open in a small popup window. Adds a convenient editor button for inserting the shortcode.
New in 0.1.3: Settings page to set Bible version and Bible search service. Both can be overridden via filters.


## Installation

1. Upload the `biblegateway-search-shortcode` directory to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Add the shortcode to a WordPress entry: `[biblegateway passage="John 3:16" display="For God so loved the world..."]` or use the convenient editor buttons.

## Frequently Asked Questions

### ?? ###
* If you run into a problem or have a question, contact me ([contact form](http://j.ustin.co/scbo43) or [@jtsternberg on twitter](http://j.ustin.co/wUfBD3)). I'll add them here.

* To use YouVersion instead of BibleGateway, you can add this filter:
```php
add_filter( 'dsgnwrks_bible_service', 'dsgnwrks_use_youversion' );
function dsgnwrks_use_youversion() {
	return 'youversion';
}
```
* To use English Standard Version instead of NIV, you can add this filter:
```php
apply_filters( 'dsgnwrks_bible_version', 'dsgnwrks_use_version_kjv' )
function dsgnwrks_use_version_kjv() {
	return 'kjv';
}
```

## Screenshots ##

1. 1) Highlight reference, 2) Optionally enter alternate text for display, 3) OK!###
![1) Highlight reference, 2) Optionally enter alternate text for display, 3) OK!](https://github.com/jtsternberg/BibleGateway-Links-Shortcode/raw/master/screenshot-1.png)

2. 1) Place cursor where you want the reference, 2) Enter reference, 3) Optionally enter alternate text for display, 3) OK!###
![1) Place cursor where you want the reference, 2) Enter reference, 3) Optionally enter alternate text for display, 3) OK!](https://github.com/jtsternberg/BibleGateway-Links-Shortcode/raw/master/screenshot-2.png)


## Changelog ##

### 0.1.6
* Bug fix: Settings page was only visible to Network Admins. Changed to be visible to standard Admins.

### 0.1.5
* Bug fixes, and filters available for each option.

### 0.1.4
* Popup window is centered and YouVersion window is smaller (formatting is better).

### 0.1.3
* Now with settings page to set Bible version and Bible search service. Both can be overridden with filters.

### 0.1.2
* Added a filter to be able to change the Bible version. It defaults to NIV.

### 0.1.1
* Add filters to be able to change the Bible service and Bible service url. A YouVersion service is built in, but Bible Gateway is the default.

### 0.1.0
* Launch.


## Upgrade Notice ##

### 0.1.6
* Bug fix: Settings page was only visible to Network Admins. Changed to be visible to standard Admins.

### 0.1.5
* Bug fixes, and filters available for each option.

### 0.1.4
* Popup window is centered and YouVersion window is smaller (formatting is better).

### 0.1.3
* Now with settings page to set Bible version and Bible search service. Both can be overridden with filters.

### 0.1.2
* Added a filter to be able to change the Bible version. It defaults to NIV.

### 0.1.1
* Add filters to be able to change the Bible service and Bible service url. A YouVersion service is built in, but Bible Gateway is the default.

### 0.1.0
* Launch.
