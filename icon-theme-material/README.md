# Material Icon Theme

* [Icon Set: Material Design Icons](https://material.io/icons/)
* Type: Font
* Version: 3.0.1
* Number of icons: 884
* [Documentation & Download](http://extensions.xwiki.org/xwiki/bin/view/Extension/Material%20Icon%20Theme/)
* [Issue Tracker](http://jira.xwiki.org/browse/ICONTHEMES/component/14844)
* Preview: 

![Material Set](http://extensions.xwiki.org/xwiki/bin/download/Extension/Material%20Icon%20Theme/WebHome/materialSet.png?width=550)

## Notes

Material set can provide the icon font, the images in format ``.png`` and ``.svg`` of ``18-24-36-48dp`` resolution, the images as ``css`` and ``svg`` sprites, in both black and white colors, etc.

The current mapping is for the **Icon Font** version, using:
```
xwiki.iconset.render.html = <span class="material-icons">$icon</span>
```

If you plan to provide the **Images** version, the mapping should be similar to: 
```
xwiki.iconset.render.html = <img src="$xwiki.getSkinFile("icons/material/.../ic_${icon}_black_24dp.png")" alt="Icon" />
```

If you plan to provide the **SVG Sprites** version, the mapping should be similar to:
```
xwiki.iconset.render.html = <svg class="svg-24px"><use href="http://.../svg-sprite-action-symbol.svg#ic_${icon}_24px"></use></svg>
```
