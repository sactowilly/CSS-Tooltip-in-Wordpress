# CSS-Tooltip-in-Wordpress
Needed to add tooltips to a plugin but didn't need all the bells and whistles the paid version included.

## Reason and Shout Out 
Specifically, a client wanted tooltips on a pricing table (ARPrice Lite, a worthwhile $25 upgrade to AR Price (and Team Showcase) Premium. It's pretty bad ass if you ask me. 300+ templates all fully customizable? And EASY? If your interested check it out at https://codecanyon.net/item/arprice-pricing-table-plugin-for-wordpress/10049883?ref=sactowilly ... I get NO compensation (remove the ?ref part if you want), but I'd like them to know who is talking mad good shit about their plugin

## Use 
### CSS 
Place the .css in your theme's (more prudent, the child theme's)style.css file, or add it using Appearance => Customize and look for where you can add custom CSS. 
#### Don't know CSS? 
If you're not CSS savvy, try TJ Custom CSS (free), SiteOrigin CSS (free, and some other great plugins), or whatever floats your boat.
#### Customizing your tooltips 
The CSS is pretty well commented so I hope that helps you figure out what you want.
### HTML 
Wrap the item you want the tool tip to be for in a div with the tooltip class `<div class="tooltip"></div>`. Next, span the tooltiptext class in that div around the text you want the tool tip to be: `<span class="tooltiptext">This is the tooltip text that appears wherever you want it to.</span>`.
So each item with a tool tip looks like this:

<p>This is some random <div class="tooltip">text<span class="tooltiptext">Not so random, huh?</span> in a random sentence.</div>

For me, I added the HTML in ARPriceLite's Description field at attached it to an image:

<div class="tooltip"><img src="http://a1solarsolutions.com/wp-content/uploads/2019/10/checkmark-e1571034086101.png"><span class="tooltiptext">Typically there is no lien, but some of the less popular ownership programs may require you to put up your home as collateral.</span></div>

It isn't anywhere as easy as using the tooltip feature in their Premium plugin, but for one table on one site that may never get updated... it was worth it.
