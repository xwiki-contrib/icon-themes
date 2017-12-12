# Glyphicons Icon Theme

* [Icon Set:  Glyphicons Halflings](https://getbootstrap.com/docs/3.3/components/)
* Type: Font
* [Documentation & Download](http://extensions.xwiki.org/xwiki/bin/view/Extension/Glyphicons%20Icon%20Theme/)
* [Issue Tracker](http://jira.xwiki.org/browse/ICONTHEMES/component/14843)
* Preview: 

![Glyphicons Set](http://extensions.xwiki.org/xwiki/bin/download/Extension/Glyphicons%20Icon%20Theme/WebHome/glyphiconsSet.png?width=550)

## Notes

Glyphicon set can provide both the icon font and the images in format ``.png`` of ``24px`` resolution.

The current mapping is for the **Icon Font** version, using:
```
xwiki.iconset.render.html = <span class="glyphicon glyphicon-$icon"></span>
```

If you plan to support the **Images** version the mapping should be similar to: 
```
xwiki.iconset.render.html = <img src="$xwiki.getSkinFile("icons/glyphicons/png/glyphicons-${icon}.png")" alt="Icon" />
```
