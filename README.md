# Snippets
Useful (?) code snippets I might want to use someday.

### Adding outline with per-tag color to every element
Source: [Addy Osmani](https://gist.github.com/addyosmani/fd3999ea7fce242756b1)
```javascript
for(i=0;A=$$("*")[i++];)A.style.outline="solid hsl("+(A+A).length*9+",99%,50%)1px"
```
Or random color per element:
```javascript
[].forEach.call($$("*"),function(a){a.style.outline="1px solid #"+(~~(Math.random()*(1<<24))).toString(16)})
```

### Adding site icons to links to that site
Source: [Lea Verou](http://lea.verou.me/)
```css
a:before {
	vertical-align:-2px;
	margin-right:5px;
	width: 16px;
	height: 16px;
}

a[href^="http://twitter.com"]:before {
	content: url(favicons/twitter.png);
}

a[href^="https://github.com"]:before {
	content: url(favicons/github.png);
}

a[href^="http://css-tricks.com"]:before {
	content: url(http://css-tricks.com/favicon.ico);
}

```
