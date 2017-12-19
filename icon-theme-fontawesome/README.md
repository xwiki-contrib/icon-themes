# Font Awesome Icon Theme

* [Icon Set: Font Awesome Icons](https://fontawesome.com)
* Type: Mixed
* Version: 5.0.1
* Number of icons: 464
* [Documentation & Download](http://extensions.xwiki.org/)
* [Issue Tracker](https://jira.xwiki.org/browse/ICONTHEMES/component/14845)

## Notes

Font Awesome 5+ set provides multiple ways to use the icons: Web Font with CSS, SVG with JS, SVG Sprites or SVG files in raw format. Also Font Awesome 5 icons are available in 3 different styles: ``Solid`` (464 free icons), ``Regular`` (115 free icons), ``Light`` (0 free icons). The provided mappings are done for the ``Solid`` style. 

The mapping for the **Web Font** and **SVG JS** versions, is:
```
xwiki.iconset.render.html = <span class="fas fa-$icon"></span>
```

The mapping for the **SVG Raw** version should be similar to: 
```
<object class="fa-svg" type="image/svg+xml" data=$xwiki.getSkinFile("icons/fontawesome/solid/${icon}.svg")></object>
```

The mapping for the **SVG Sprite** version is:
```
xwiki.iconset.render.html = <svg class="fa-svg"><use href="$xcontext.getURLFactory().createAttachmentURL('fa-solid.svg', 'IconThemes.FontAwesome', 'SVGSprite', 'download', '', $context.context)#${icon}"></use></svg>
```
