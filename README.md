# BubbleGasket theme for Hugo (Hugo.io)

https://github.com/danieljudd/bubblegasket

## Features:
- No Javascript
- Lightweight (around 7.5KB for main page)
- No tracking or 3rd party dependencies
- Works on a static web server
- Customizable via CSS and config.toml

Responsive page for browsers
![/images/preview1.jpg](/images/preview1.jpg)

Easy to read
![/images/preview2.jpg](/images/preview2.jpg)

---
### Changelog

2.1
(Nov 1st 2022)
* Date is right side of page now
* Font and line spacing changes
* No more lists on main page
* Headers more consistent (h1) and left justified (i.e., default)

2.0
* Started v2 + archived v1
* Added archive page, changed CSS and config option
* Initial release on Github

1.0
(archived)

---
### To do
- Better favicon options (choice of emoji or image)
- More themes in the form of CSS files
- ~~Pick a good default font~~
- ~~Tags and Archive should fit in better~~
- Cleaner or more readable CSS

---

## Setup for new Hugo users:

1. In terminal/command line, setup your website folder in Hugo as you like :

		hugo new site MyWebsiteFolder
	
2. Place **bubblegasket** folder and its contents in MyWebsiteFolder/themes/

		git clone https://github.com/danieljudd/bubblegasket.git

3. Add line **theme = 'bubblegasket'** to root file (MyWebsiteFolder/config.toml) or copy config below

## Configuration example (and config.toml)
### Website requires you to create your own 'content' folders under *yoursite.com* /content/EXAMPLEFOLDER
**...use any appropriate name and assign them under the config.toml**
**These will then appear under your website's navigation and point to your created folder.**

	baseURL = 'https://example.org/'
	languageCode = 'en-us'
	title = "BubbleGasket"
	theme = 'bubblegasket'

	# (menu) titles would end with "s" otherwise
	pluralizeListTitles = false
	Copyright = '©'

	[params]
		Email = 'example@example.com'
		Footer = 'example.com'
		Github = 'https://github.com/github'
		# Turn on or off tag cloud (true is on or false off)
		Tags = false
		# Turn on or off archive (true is on or false off)
		Archive = false
		# Emoji icons: https://emojipedia.org
		Icon = '☂️'
		numPosts = '3'
		Section1 = "blog"
		Section2 = "work"
	[menu]
		[[menu.main]]
			name = "☕ About"
			url = "/about"
			weight = 1
		[[menu.main]]
			name = "✒️ Blog"
			url = "/blog"
			weight = 2
		[[menu.main]]
			name = "👔 Work"
			url = "/work"
			weight = 3
		[[menu.main]]
			name = "📭 Donate"
			url = "/donate"
			weight = 4
		

1. Create hugo posts and (optionally) use tags
		hugo new blog/mypost.md
		
For tags (Tags = true), edit the file and add this line in header of mypost.md:

		tags = [changeme,topic,blog,category,etc]

2. Customize CSS options by searching for keywords "color" and "font-size" and "font-family"

## Example website
![/images/preview3.jpg](/images/preview3.jpg)

---

GNU License for Bubblegasket:

---

    Bubblegasket is a GPL software theme for Hugo (https://gohugo.io/)
    Copyright (C) 2022  Daniel Judd
	
	Original author's website: https://danieljudd.xyz | https://github.com/danieljudd

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.