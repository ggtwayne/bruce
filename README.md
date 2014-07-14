# bruce

Simple, reponsive story template created for [registerguard.com](http://registerguard.com) by [Rob Denton](http://github.com/robertdenton). 

This is meant to be built off of for special stories. It's not to be taken as is because without a spectacular story, it doesn't mean much. It's a tool. It's a means of storytelling. It's not whats underneath but what we do with it that defines us.

![batman_returns3](https://cloud.githubusercontent.com/assets/4853944/3446952/fa6fbaa2-0147-11e4-8bd9-e9b748ea15b8.gif)
([credit](http://i26.photobucket.com/albums/c117/shocktrooper327/batman_returns3.gif))

## Demos

* [Assorted media](http://pages.registerguard.com/bruce/)
* [WWII story](http://pages.registerguard.com/bruce/wwii)

## Notes

* This theme is build using [Normalize.ccs](http://necolas.github.io/normalize.css/) and [PureCSS](http://purecss.io).
* Also used is [d3.js](http://d3js.org) but that is not necessary.
* This theme excels with a lot of different media. Supported media:
  * Hi-res images - still and gif
    * Full width (.bat_full)
    * Side embed (.bat_media)
    * Vertical (.bat_media && width:70%;)
  * Video (.bat_media)
  * Audio (.bat_media)
    * HTML5
    * Soundcloud embed
  * Maps (.bat_full && .bat_media)
  * Block quotes (.bat_quote)
  * Charts - d3.js (.bat_media)
  * HTML tables (.bat_media)
  * Twitter embeds (.bat_media)
  * Info boxes (.bat_media > .bat_info)
* All media in `<figure>` tags should have `<figcaption>` tags.
* Preferred viewing size:
  * Mobile
  * 1320px wide desktop
* d3.js cannot be previewed in Chrome. Use Firefox for local dev.


#### Verical images

To make a vertical image display properly, please add in this inline CSS.

**Note:** IMG width and figcaption style. Also, be sure to add in appropriate img path and caption.

```html
	<div class="bat_media">
		
		<figure>
			<img src="media/image.jpg" width="70%">
		</figure>
		
		<figcaption style="width:70%;margin:0 auto;">
			Caption present tense. Past tense. Quote. (Name/photo)
		</figcaption>
	
	</div><!-- /.bat_media -->

```

#### Media queries

You'll notice there are two media queries, here's why.

`@media (min-width: 48em)`

The first is for Pure grids (the byline).

`@media (min-width: 980px)`

The second is for my main CSS.

Since the template is built on mobile primarily, the only media query needed is 980 and up.

#### Sub heads

They go outside `.bat_story`

```html
	</div><!-- /.bat_story -->
		
	<h2>Fortune smiles and frowns</h2>
		
	<div class="bat_story">
```