xHTML xoops theme by Michael Hokamp [studioC] (c)2005
<a href="http://studiocreativ.de">http://studiocreativ.de</a> 
<a href="http://xoopsfactory.de">http://xoopsfactory.de</a>
VERSION : 1.00
DATE : 06.Feb. 2005


Another theme from xoopsfactory that we've put for download! 

This is not published under GPL, some rights are reserved, 
so please do not remove copyright and links to XOOPSfactory.
Donators are welcome and will get a unique ID which will allow to 
remove copyright notices for ONE domain.

If you are able to use this for a clients page please i think it is
nice to give us a small donation.


the <div id="rechts"> is to place adds like google adsense. I have used
a google adsense format with width 160 and height 600. This works pretty nice.

you might want to place the xoops right blocks into that position and just
use the 3 centerblocks and content in the <div id="centercontent">

to do so:
just delete the lines 56-58 of theme.html

56<{if $xoops_showrblock == 1}>
57<div id="xoopsrightblock"><{foreach item=block from=$xoops_rblocks}><{include file="$xoops_theme/blocks/theme_blockright.html"}><{/foreach}></div>
58<{/if}>

out of the <div id="centercontent"> and put 


<{foreach item=block from=$xoops_rblocks}>
<{include file="$xoops_theme/blocks/theme_blockright.html"}>
<{/foreach}>

(Without the surrounding <div id="xoopsrightblock"></div))


into <div id="rechts"> </div> 


thats all.
Now its your turn ... you may want to float one of the centerblocks ?
see how it's done with <div id="xoopsrightblock">

michael







