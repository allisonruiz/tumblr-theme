# tumblr-theme
<!DOCTYPE html>
<head>
 
<!--
 
    BIBLIOPHILE - TWO SIDEBARS (updated 18/6/21)
        by alydae
 
            - this theme DOES support new post types but 
              you must turn on 'use new post types' for it to work
            - it may look weird in customise but it will be fine
              once you exit and view your blog
 
            - do not steal any part of this code
            - do not even TOUCH the credit
            - direct questions to enchantedthemes.tumblr.com
 
        please read the customisation guide before editing this theme 
        http://enchantedthemes.tumblr.com/bibliophile/guide
 
        this version is coded to be a fansite. 
        if you want to use it as a personal blog, instructions are in the guide below - there are areas that need to be changed for it to work.
 
        to edit the sidebars, find 'editing the sidebars'
 
    thank you for using!!!
 
-->


 
<style type="text/css">
body{cursor:url(https://static.tumblr.com/xjqjg7j/Mhcmxtzxp/84.gif), url(https://static.tumblr.com/xjqjg7j/Mhcmxtzxp/84.gif), auto;}
</style>

<title>{block:PostSummary}{PostSummary} - {/block:PostSummary}{block:TagPage}#{Tag} - {/block:TagPage}{Title}</title>
<link rel="shortcut icon" href="{Favicon}">
 
<link rel="alternate" type="application/rss+xml" href="{RSS}">
{block:Description}<meta name="description" content="{MetaDescription}" />{/block:Description}
 
<meta name="color:background" content="#fafafa"/>
<meta name="color:posts" content="#ffffff"/>
<meta name="color:text" content="#666666"/>
<meta name="color:links" content="#222222"/>
<meta name="color:links hover" content="#bad0f1"/>
<meta name="color:title" content="#000000"/>
<meta name="color:accent" content="#222222"/>
<meta name="color:border" content="#eeeeee"/>
 
<meta name="color:blog title" content="#000000"/>
<meta name="color:navi background" content="#eeeeee"/>
<meta name="color:navi border" content="#dddddd"/>
<meta name="color:header background" content="#ffffff"/>
<meta name="color:topbar background" content="#eeeeee"/>
<meta name="color:topbar border" content="#dddddd"/>
 
<meta name="image:header" content=""/>
 
<meta name="select:font size" content="10px"/>
<meta name="select:font size" content="11px"/>
<meta name="select:font size" content="12px"/>
 
<meta name="select:font" content="Open Sans"/>
<meta name="select:font" content="Karla"/>
<meta name="select:font" content="Lato"/>
<meta name="select:font" content="Roboto"/>
 
<meta name="select:post width" content="400px"/>
<meta name="select:post width" content="450px"/>
<meta name="select:post width" content="500px"/>
<meta name="select:post width" content="540px"/>
 
<meta name="select:margin" content="25px"/>
<meta name="select:margin" content="50px"/>
<meta name="select:margin" content="75px"/>
 
<meta name="if:hide header on index" content=""/>
<meta name="if:show header on permalink" content=""/>
<meta name="if:show controls on index" content=""/>
<meta name="if:hide tags on index" content=""/>
<meta name="if:scroll to top" content=""/>
<meta name="if:infinite scroll" content=""/>
<meta name="if:load more" content=""/>
 
<meta name="if:search bar" content=""/>
<meta name="if:manual members" content=""/>
<meta name="if:automatic members" content=""/>
 
<meta name="text:link 1 title" content="link 1"/>
<meta name="text:link 1 url" content=""/>
<meta name="text:link 2 title" content="link 2"/>
<meta name="text:link 2 url" content=""/>
<meta name="text:link 3 title" content="link 3"/>
<meta name="text:link 3 url" content=""/>
<meta name="text:link 4 title" content="link 4"/>
<meta name="text:link 4 url" content=""/>
<meta name="text:link 5 title" content="link 5"/>
<meta name="text:link 5 url" content=""/>
<meta name="text:link 6 title" content="link 6"/>
<meta name="text:link 6 url" content=""/>
 
<script src="https://kit.fontawesome.com/4fe045a39a.js" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdn.linearicons.com/free/1.0.0/icon-font.min.css">
 
<!-- custom font -->
 
<link href="https://fonts.googleapis.com/css?family={select:font}:300,400,600,700,300italic,400italic,600italic,700italic" rel="stylesheet" type="text/css">
 
 
<style type="text/css">
html { background-color:{color:background}!important; }
body { background-color:{color:background}!important; }
 
 
@keyframes fadein {
    from { opacity:0; }
    to   { opacity:1; }
}
 
@-moz-keyframes fadein {
    from { opacity:0; }
    to   { opacity:1; }
}
 
@-webkit-keyframes fadein {
    from { opacity:0; }
    to   { opacity:1; }
}
 
@-ms-keyframes fadein {
    from { opacity:0; }
    to   { opacity:1; }
}
 
@-o-keyframes fadein {
    from { opacity:0; }
    to   { opacity:1; }
}
 
 
/*-- selection --*/
 
::-moz-selection { background:rgba({RGBcolor:links hover},0.1); color:#222; }
::selection { background:rgba({RGBcolor:links hover},0.1); color:#222; }
 
/*-- scrollbar --*/
 
::-webkit-scrollbar { width:2px; height:8px; }  
::-webkit-scrollbar-thumb { background-color:{color:accent}; }  
::-webkit-scrollbar-thumb:horizontal { display:none!important; }  
 
/*-- tooltips --*/
 
#s-m-t-tooltip {
    color:{color:text};
    background-color:{color:posts};
    border:1px solid {color:border};
    font-family:{select:font}, helvetica, sans-serif;
    letter-spacing:0.5px;
    text-transform:uppercase;
    text-align:center;
    position:absolute;
    padding:2px 7px 2px 7px;
    margin-top:30px;
    z-index:99999999!important;
}
 
/*-- tumblr controls --*/
 
iframe.tmblr-iframe {
    z-index:9999999!important;
    top:60px!important;
    right:0!important;
    opacity:0;
    padding-right:43px;
    /* delete from here */
        filter:invert(1) hue-rotate(180deg);
        -webkit-filter:invert(1) hue-rotate(180deg);
        -o-filter:invert(1) hue-rotate(180deg);
        -moz-filter:invert(1) hue-rotate(180deg);
        -ms-filter:invert(1) hue-rotate(180deg);
    /* to here if your blog has a dark background */
    transform:scale(0.6);
    transform-origin:100% 0;
    transition: opacity 0.6s ease-in-out;
    -moz-transition: opacity 0.6s ease-in-out;
    -webkit-transition: opacity 0.6s ease-in-out;
    -webkit-transform:scale(0.6);
    -webkit-transform-origin:100% 0;
    -o-transform:scale(0.6);
    -o-transform-origin:100% 0;
    -moz-transform:scale(0.6);
    -moz-transform-origin:100% 0;
    -ms-transform:scale(0.6);
    -ms-transform-origin:100% 0;
}
 
iframe.tmblr-iframe:hover { opacity:0.4!important; }
 
/*-- lightbox --*/
 
#tumblr_lightbox, .tmblr-lightbox {
    background-color:{color:background}!important;
    z-index:999999!important;
}
 
#vignette, .vignette { opacity:0; }
 
#tumblr_lightbox img, .lightbox-image {
    box-shadow:none!important;
    border-radius:0!important;
}
 
#tumblr_lightbox_caption, .lightbox-caption { visibility:hidden; }
 
 
/*-- general customisation --*/
 
a, a:hover, .links i, .links i:hover, .like_button:hover + svg, .info i, .info i:hover, .hnavi {
    transition-duration: 0.6s;  
    -moz-transition-duration: 0.6s;  
    -webkit-transition-duration: 0.6s;  
    -o-transition-duration: 0.6s
}
 
body {
    color:{color:text};
    background-color:{color:background};
    font-style:normal; 
    font-family:{select:font}, helvetica, sans-serif; 
    font-size:{select:font size}; 
    font-weight:400;
    text-decoration:none; 
    line-height:180%; 
    margin:0;
    overflow-x:overflow;
    word-wrap: break-word;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    font-smoothing: antialiased;
    -webkit-animation: fadein 1.5s;
    -moz-animation: fadein 1.5s;
    -o-animation: fadein 1.5s; 
    animation: fadein 1.5s;
}
 
a {
    text-transform:lowercase;
    text-decoration:none;
    color:{color:links};
}   
 
a:hover { color:{color:links hover}; cursor:pointer; }
a.tumblr_blog b:hover, b a:hover { color:{color:links hover}; }
.c a { border-bottom:1px solid {color:border}; }
a.post_media_photo_anchor, .npf-link-block a { border-bottom:none!important; }
 
i, em { font-style:italic; }
b, strong { color:#444; font-weight:600;}
 
small { font-size:calc({select:font size} - 0.5px); }
big { font-size:calc({select:font size} + 1px); }
 
blockquote {
    padding-left:10px;
    margin-left:0px;
    border-left:1px solid {color:border};
    width:95%;
    word-wrap:break-word;
}
 
h1, h2, h3, h4, h5, h6 {
    text-transform:uppercase!important;
    text-align:left;
    font-weight:bold;
    font-size:calc({select:font size} + 2px);
    letter-spacing:1px;
    color:{color:title};
}
 
h1 { 
    padding-left:15px;
    {block:PermalinkPage}padding-top:5px;{/block:PermalinkPage}
}
 
h1 a { text-transform:uppercase!important; }
 
pre {
    white-space: pre-wrap;
    white-space: -moz-pre-wrap;
    white-space: -pre-wrap;
    white-space: -o-pre-wrap;
    word-wrap: break-word;
    background-color:#fafafa;
    padding:5px;
}
 
 
/*-- top navigation/links --*/
 
#navi {
    top:0;
	left:0;
    width:100vw;
    height:50px;
    background:{color:navi background};
    border-bottom:1px solid {color:navi border};
    z-index:999!important;
    text-align:center;
    {block:IndexPage}
    position:relative;
    {block:ifhideheaderonindex}
    display:none!important;
    {/block:ifhideheaderonindex}
    {/block:IndexPage}
    {block:PermalinkPage}
    {block:ifnotshowheaderonpermalink}
    display:none;
    {/block:ifnotshowheaderonpermalink}
    {block:ifshowheaderonpermalink}
    position:relative!important;
    {/block:ifshowheaderonpermalink}
    {/block:PermalinkPage}
}
 
#navi a, .hnavi a {
    padding:18px;
    line-height:50px;
    font-weight:600;
    font-size:12px;
    text-transform:lowercase!important;
    display:inline;
    margin-left:-3px;
}
 
.hnavi {
    height:50px;
    {block:IndexPage} 
    position:relative;
    {block:ifnothideheaderonindex}
    display:none;
    {/block:ifnothideheaderonindex}
    {block:ifhideheaderonindex}
    opacity:1!important;
    {/block:ifhideheaderonindex}
    {/block:IndexPage}
    {block:PermalinkPage} 
    {block:ifnotshowheaderonpermalink}
    opacity:1!important;
    {/block:ifnotshowheaderonpermalink}
    {block:ifshowheaderonpermalink}
    display:none;
    {/block:ifshowheaderonpermalink}
    {/block:PermalinkPage}
}
 
.hnavi a:hover { background:{color:accent}; color:{color:posts}; }
 
#navi a:empty, .hnavi a:empty { display:none; }
 
 
/*-- header image --*/
 
#image {
    {block:IndexPage}
    position:relative;
    overflow:hidden;
    background-color:{color:header background};
    {block:ifhideheaderonindex}
    display:none!important;
    {/block:ifhideheaderonindex}
    {/block:IndexPage}
    {block:PermalinkPage}
    {block:ifnotshowheaderonpermalink} 
    display:none;
    {/block:ifnotshowheaderonpermalink} 
    {block:ifshowheaderonpermalink} 
    position:relative;
    overflow:hidden;
    background-color:{color:header background};
    {/block:ifshowheaderonpermalink}
    {/block:PermalinkPage}
	z-index:99;
}
 
#image img {
    height:350px;
    width:auto;
    margin-left:50%;
    transform:translateX(-50%);
    display:block;
}
 
 
/*-- topbar --*/
 
#topbar {
    position:relative;
    height:50px;
    width:100vw;
    background:{color:topbar background};
    border-top:1px solid {color:topbar border};
    border-bottom:1px solid {color:topbar border};
    z-index:999!important;
}
 
.title {
    position:relative;
    float:left;
    line-height:45px;
    text-transform:lowercase;
    font-size:22px;
    letter-spacing:-1px;
    font-weight:700;
    margin-left:50px;
    margin-right:20px;
    color:{color:blog title};
}
 
.links {
    position:absolute;
    top:0;
    right:50px;
    float:right;
    padding:0px;
    height:50px;
}
 
.links img {
    height:30px;
    width:30px;
    border-radius:100%;
    margin:10px 0 -10px 0; 
    float:right;
}
 
.links a { display:inline; margin-left:15px; }
 
.links i, .links i:hover {
    line-height:100%;
    font-size:15px;
    width:15px;
    padding:7.5px;
    margin:10px 0;
    border-radius:100%;
    background-color:{color:accent};
}
 
.links i { color:{color:posts}; }
.links i:hover { color:{color:accent}; background-color:{color:posts}; }
 
 
/*-- posts --*/
 
#entries {
    margin:{select:margin} auto;
    width:{select:post width};
}
 
.posts {
    width:{select:post width};
    margin-bottom:{select:margin};
    background-color:{color:posts};
    border:1px solid {color:border};
}
 
.posts ul li { list-style:none; margin-left:-20px; }
 
.posts ul li:before {
    content:"";
    display:inline-block;
    background:#ddd;
    margin-bottom:2px;
    width:20px;
    height:1px;
    margin-right:10px;
}
 
.posts li, .posts blockquote, .posts img { max-width:100%; height:auto; }
 
 
/*-- captions --*/
 
.c { 
    padding:0px 15px 0px 15px;
    margin:0; 
}
 
.tumblr_parent {
    margin:0;
    padding-left:0px;
    border-left:none;
    width:100%;
}
 
.tumblr_parent blockquote {
    margin-left:0px;
    padding-left:10px;
    border-left:1px solid {color:border};
}
 
.tumblr_avatar { 
    margin-right:10px; 
    margin-bottom:-6px;   
    width:20px;
    height:20px;
    border-radius:100%;
}
 
img.tumblr_avatar + a.tumblr_blog {
    font-weight:600;
    line-height:100%;
    padding:5px;
    background:{color:background};
    border:1px solid {color:border};
}
 
img.tumblr_avatar + a.tumblr_blog:hover { background:{color:posts}; }
 
.tumblr_parent:first-of-type a.tumblr_blog, .tumblr_parent:first-of-type img.tumblr_avatar { display:none; }
.tumblr_parent { padding-top:10px; }
.tumblr_parent:first-of-type { padding-top:0!important; }
 
.npf_photoset { margin-left:-15px; margin-right:-15px; }
.npf_photoset .tmblr-full .npf_image { margin-bottom:-6px; }
 
a.tumblr_blog ~ .npf_photoset, a.tumblr_blog ~ figure:not(.tmblr-full) { margin-top:15px; }
.tumblr_parent:first-of-type a.tumblr_blog ~ .npf_photoset { margin-top:0!important; }
 
.tmblr-full { 
    margin-left:-15px; 
    margin-right:-15px; 
    margin-bottom:-6px; 
}
 
.tmblr-attribution {
    margin-top:-5px!important;
    margin-bottom:6px;
    padding:5px 10px;
    text-align:right;
    background:{color:background};
}
 
.tmblr-attribution a {
    text-transform:lowercase;
    border:none!important;
    font-style:italic;
}
 
.tmblr-attribution:after { 
    content:'>'; 
    float:right;
    padding-left:7px;
    font-weight:700;
    display:inline; 
}
 
.tmblr-attribution:hover { 
    background:{color:background}; 
    cursor:pointer;
}
 
a.read_more { 
    font-style:italic;
    margin-left:42%;
    font-weight:600;
}
 
/*-- quote posts --*/
 
.quote, p.npf_quote {
    padding:10px;
    font-size:calc({select:font size} + 2px);
    font-style:italic;
    line-height:180%;
    text-align:center;
}
 
.quotesource { 
    text-align:right;
    padding-bottom:10px;
    padding-right:10px;
}
 
 
/*-- link posts --*/
 
.npf-link-block {
    border:1px solid {color:border};
    margin-top:15px;
    border-radius:0px;
}
 
.npf-link-block .poster { height:200px; }
 
.npf-link-block .poster .title {
    color:#fff!important;
    text-transform:uppercase!important;
    text-align:left;
    font-weight:700;
    font-size:calc({select:font size} + 2px);
    font-style:normal;
    margin:0!important;
    letter-spacing:2px;
    line-height:180%;
}
 
.npf-link-block .poster .title:after { content:'>>'; padding-left:10px; }
 
.npf-link-block .bottom { background-color:{color:background}; }
 
.npf-link-block .bottom .description {
    margin:0;
    padding:0;
    border:none;
    text-transform:none;
    line-height:160%;
    font-size:{select:font size};
    font-style:italic;
    text-align:left;
}
 
.npf-link-block .bottom .site-name {
    font-size:{select:font size};
    font-weight:700;
    letter-spacing:1px;
    line-height:100%;
}
 
 
/*-- chat posts --*/
 
.chat { list-style:none; }
 
.line.odd { padding:10px; background:{color:background}; }
.line.even { padding:10px; }
 
.label {
    text-transform:uppercase;
    font-weight:600;
    color:{color:accent};
    letter-spacing:1px;
}
 
 
/*-- audio posts --*/
 
.audio { background-color:#f2f2f2; padding:10px; }
 
.playbutton {
    width:30px;
    height:30px;
    position:relative;
    overflow:hidden;
}
 
.playbox { position:absolute; padding:5px; }
 
.trackdetails {
    padding:10px;
    width:auto;
    height:auto;
    margin-left:55px;
    padding-left:10px;
    font-size:calc({select:font size} + 1px);
}
 
 
/* -- video posts --*/
 
.video.resized { overflow:hidden; }
 
.c .embed_iframe { 
    width:{text:post width}px;
    height:calc(({text:post width}px / 9) * 5);
}
 
iframe#youtube_iframe { margin-bottom:-5px!important; }
 
 
/*-- ask posts --*/
 
.question {
    position:relative;
    margin-right:65px;
    margin-left:15px;
    padding:10px;
    height:auto;
    text-align:right;
    word-wrap:break-word;
    background:{color:background};
	border:1px solid {color:border};
}
 
.question p { margin:0!important; }
 
.asker {
    position:relative;
    padding:10px 5px 5px 10px;
    text-align:right;
    text-transform:lowercase;
    font-style:italic;
}
 
.asker a { padding-right:0px; }
 
.aicon {
    position:relative;
    padding:15px;
    float:right;
}
 
.aicon img {
    width:35px;
    border-radius:50%;
    z-index:999!important;
}
 
.answer { margin-top:0px; }
 
 
/*-- top post info --*/
 
.topinfo { padding:10px; border-bottom:1px solid {color:border}; }
 
.topinfo img { 
    height:35px; 
    width:35px; 
    border-radius:100%!important;
    position:absolute;
    margin-left:-27.5px;
    margin-right:10px;
}
 
.toptext {
    margin:-10px 20px;
    position:relative;
    line-height:55px;
    font-size:calc({select:font size} + 1px);
    width:calc({select:post width} - 20px - 25px)
}
 
.pinned { display:inline; font-weight:600; }
 
 
/*-- bottom post info --*/
 
.info {
    padding:10px 3px 7px 10px;
    text-transform:none;
    border-top:1px solid {color:border};
    margin-top:0px;
    background-color:{color:topbar background};
}
 
.info img {
    height:20px;
    width:20px;
    border-radius:100%;
    margin-right:10px;
    position:relative;
}
 
.dtext {
    margin-left:30px;
    margin-top:-28px;
    position:relative;
    background-color:{color:posts};
    padding:3px 5px 3px;
    {block:ifnotshowcontrolsonindex}
    width:calc({select:post width} - 30px - 33px);
    {/block:ifnotshowcontrolsonindex}
    {block:ifshowcontrolsonindex}
    width:calc({select:post width} - 30px - 20px - 55px);
    {block:ifshowcontrolsonindex}
    {block:PermalinkPage}
    width:calc({select:post width} - 30px - 20px - 55px);
    {block:PermalinkPage}
    border:1px solid {color:border};
}
 
.info i {
    font-size:12px;
    margin-right:7px;
    margin-top:-18px;
    float:right;
    position:relative;
    color:{color:accent};
}
 
.info i:hover { color:{color:links hover}; cursor:pointer!important; }
 
#tags { 
    position:relative; 
    padding:7px 10px; 
    border-top:1px solid {color:border};
    word-wrap: break-word;
    {block:IndexPage}
    {block:ifhidetagsonindex}display:none;{/block:ifhidetagsonindex}
    {/block:IndexPage}
}
 
#tags a {
    margin-right:10px;
    text-transform:lowercase;
    font-style:italic;
    font-size:calc({select:font size} - 0.5px)
}
 
.custom-like-button {
    position:relative;
    display:block;
    float:right;
    width:14px;
    height:14px;
    padding-left:7px;
}
 
.like_button {
    position:absolute;
    top:-16px;
    left:0;
    right:15px;
    bottom:0;
    width:100%;
    height:100%;
    opacity:0;
    z-index:10;
}
 
.like_button iframe { width:100%!important; height:100%!important; }
 
.likes i {
    position:absolute;
    top:0;
    left:0;
    right:0;
    bottom:0;
    width:100%;
    height:100%;
    z-index:1;
}
 
.like_button:hover + .likes i {
    color:{color:links hover}!important;
    cursor:pointer!important;
}
 
.like_button.liked + .likes i { color:#dc143c!important; } /* liked heart colour */
 
 
/*-- post notes --*/
 
ol.notes {
    padding:10px;
    margin:25px 0px;
    width:calc({select:post width} - 20px);
    list-style-type:none;
    background:{color:posts};
    border:1px solid {color:border};
}
 
ol.notes li.note { padding:5px; }
 
ol.notes li.note img.avatar {
    vertical-align:-4px;
    margin-right:10px;
    width:14px;
    height:14px;
    border-radius:50%;
}
 
ol.notes li.note span.action { font-weight:none; }
ol.notes li.note .answer_content { font-weight:normal; }
 
ol.notes li.note blockquote {
    padding-left:10px;
    margin-left:25px;
    border-left:1px solid {color:border};
	width:90%;
}
 
ol.notes li.note blockquote a { text-decoration:none; }
 
.more_notes_link, .notes_loading {
    font-weight:600;
    display:block;
    text-align:left!important;
}
 
 
/*-- pagination and infinite scroll --*/
 
#pagination { text-align:center; margin-bottom:{select:margin}; }
#pagination a { margin-right:10px; }
 
{block:ifinfinitescroll}
#pagination, #infscr-loading { display:none!important; }
{/block:ifinfinitescroll}
 
footer {
    width:{select:post width};
    margin:0 auto {select:margin};
    position:relative;
    text-align:center!important;
}
 
a#loadmore { font-size:{select:font size}px; }
 
 
/*-- other --*/
 
.tc {
    position:fixed;
    top:60px;
    right:0;
}
 
.tc .fa { margin:10px 15px 15px 15px; }
 
.st {
    position:fixed;
	display:none;
	left:20px;
	bottom:15px;
}
 
.st a { font-size:9px; }
 
 
/*-- credit - DO NOT TOUCH --*/
 
.credit a {
    font-size:10px;
    bottom:15px;
    right:20px;
    position:fixed;
    text-transform:uppercase;
}
 
 
/*-- sidebars --*/
 
#leftside, #rightside {
    width:200px;
    position:absolute;
    text-align:justify;
    {block:IndexPage}
    margin-top:calc({select:margin} + 452px);
    {block:ifhideheaderonindex}
    margin-top:calc({select:margin} + 52px);
    {/block:ifhideheaderonindex}
    {/block:IndexPage}
    {block:PermalinkPage}
    margin-top:calc({select:margin} + 52px);
    {block:ifshowheaderonpermalink}
    margin-top:calc({select:margin} + 452px);
    {/block:ifshowheaderonpermalink}
    {/block:PermalinkPage}
}
 
#leftside { left:calc(50vw - ({select:post width} + 20px) / 2 - {select:margin} - 200px); }
#rightside { left:calc(50vw + ({select:post width} + 20px) / 2 + {select:margin}); }
 
.box { padding:10px; }
 
.box:after {
    content:"";
    display:block;
    margin:20px 0px;
    height:1px;
    width:100%;
    background:{color:border};
}
 
.box h1 {
    text-transform:uppercase;
    font-size:calc({select:font size} + 2px);
    font-weight:700;
    letter-spacing:0px;
    color:{color:title};
    line-height:100%;
    padding:0px;
}
 
.sb { max-width:100px; z-index:9999!important; }
 
.sb .search .query {
    border:0;
    outline:0;
    margin-top:10px;
    padding:0px;
    font-family:inherit;
    font-size:inherit;
    font-style:italic;
    color:{color:links};
    background-color:transparent;
}
 
::-webkit-input-placeholder { color:{color:links}; }
:-moz-placeholder { color:{color:links}; opacity:1; }
::-moz-placeholder { color:{color:links}; opacity:1; }
:-ms-input-placeholder { color:{color:links}; }
input:focus::-webkit-input-placeholder { color: transparent; }
input:focus:-moz-placeholder { color: transparent; }
input:focus::-moz-placeholder { color: transparent; }
input:focus:-ms-input-placeholder { color: transparent; }
 
.blogs { display:block; height:40px; }
 
.blogs img {
    position:relative;
    height:30px;
    width:30px;
    margin-top:5px;
    margin-right:10px;
    margin-bottom:5px;
    border-radius:100%;
}
 
.blogs a { position:relative; top:-17.5px; }
 
.updates { display:block; }
 
.updates h3 {
    line-height:100%;
    font-style:italic;
    font-weight:600;
    font-size:{select:font size};
    text-transform:none!important;
    letter-spacing:0px;
    display:inline;
    color:{color:text}!important;
}
 
.updates h3:after { content:":"; margin-right:7px; }
 
</style>
 
 
<!-- scripts -->
 
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
 
<!-- video resizing by @shythemes -->
<script src ="//static.tumblr.com/fwgzvyf/Oj1o08f6h/shythemes.vr.js"></script>
 
<!-- pixel union photosets  - modified by @bychloethemes -->
<link href="https://static.tumblr.com/qudkd6d/OcDnl99gb/style.css" rel="stylesheet" type="text/css"/>
<script src="https://static.tumblr.com/yxfeliq/hHwojmt8m/bctphotoset.min.js"></script>
 
<script>
//pxu photosets
$(document).ready(function(){
   $('.photo-slideshow').pxuPhotoset({
       lightbox: true,
       rounded: false,
       gutter: '4px',
       borderRadius: '0px',
       photoset: '.photo-slideshow',
       photoWrap: '.photo-data',
       photo: '.pxu-photo'
   });
});
 
{block:IndexPage}
{block:ifnothideheaderonindex}
//show on scroll
$(document).scroll(function () {
    var y = $(this).scrollTop();
    if (y > 360) {
        $('.hnavi').fadeIn();
    } if (y < 360) {
        $('.hnavi').fadeOut();
    }
});
{/block:ifnothideheaderonindex}
{/block:IndexPage}
 
{block:PermalinkPage}
{block:ifshowheaderonpermalink}
//show on scroll
$(document).scroll(function () {
    var y = $(this).scrollTop();
    if (y > 360) {
        $('.hnavi').fadeIn();
    } if (y < 360) {
        $('.hnavi').fadeOut();
    }
});
{/block:ifshowheaderonpermalink}
{/block:PermalinkPage}
</script>
 
 
</head>
 
<body>
 
 
<!-- EDITING THE SIDEBARS
the sidebar sections that need to be edited are right after this note. before editing, please read the guide as it says what can be done to the sections, including adding more and moving them around. the default sections with templates provided are about, members, statistics, updates, affiliates and disclaimer but they can be changed to many other sections through following the instructions on the guide at
http://enchantedthemes.tumblr.com/bibliophile/guide
-->
 
<!-- left sidebar -->
 
<div id="leftside">
 
<!-- about -->
<div class="box">
<h1>about</h1>
    {Description}
    {block:ifsearchbar}
    <div class="sb">
    <form action="/search" method="get" class="search">
        <input type="text" name="q" value="{SearchQuery}" class="query" placeholder="search this blog..."/>
    </form>
    </div>
    {/block:ifsearchbar}
</div>
<!-- end about -->
 
<!-- members -->
<div class="box">
<h1>members</h1>
<div class="updates"><h3>Student A</h3>Allison Ruiz</div>
<div class="updates"><h3>Student B</h3>Adriana Gallardo</div>
<div class= "updates"><h3>Student C</h3>Christy Chavira</div>
{block:ifmanualmembers}
<div class="blogs">
    <img src="https://api.tumblr.com/v2/blog/blog.tumblr.com/avatar/128" /> 
    <a href="/" title="name">blog url</a>
</div>
<div class="blogs">
    <img src="https://api.tumblr.com/v2/blog/blog.tumblr.com/avatar/128" /> 
    <a href="/" title="name">blog url</a>
</div>
{/block:ifmanualmembers}
 
{block:ifautomaticmembers}
{block:GroupMembers} {block:GroupMember} 
<div class="blogs">
    <img src="{GroupMemberPortraitURL-128}" /> 
    <a href="{GroupMemberURL}" title="{GroupMemberTitle}">{GroupMemberName}</a>
</div>
{/block:GroupMember}{/block:GroupMembers}
{/block:ifautomaticmembers}
</div>
<!-- end members -->
 
<!-- statistics -->
<div class="box">
<h1>statistics</h1>
<div class="updates"><h3>about</h3>info</div>
<div class="updates"><h3>established</h3>2/12/23</div>
<div class="updates"><h3>years active</h3>{CopyrightYears}</div>
<div class="updates"><h3>online</h3> <script language="JavaScript">var fhs = document.createElement('script');var fhs_id = "5683887";
var ref = (''+document.referrer+'');var pn =  window.location;var w_h = window.screen.width + " x " + window.screen.height;
fhs.src = "//freehostedscripts.net/ocounter.php?site="+fhs_id+"&e1=Online User&e2=Online Users&r="+ref+"&m=0&wh="+w_h+"&a=1&pn="+pn+"";
document.head.appendChild(fhs);document.write("<span id='o_"+fhs_id+"'></span>");
</script>
</div>
<div class="updates"><h3>views</h3> <script language="JavaScript">var fhsh = document.createElement('script');var fhs_id_h = "3374876";
fhsh.src = "//freehostedscripts.net/ocount.php?site="+fhs_id_h+"&name=Visits&a=1";
document.head.appendChild(fhsh);document.write("<span id='h_"+fhs_id_h+"'></span>");
</script></div>

<div class="updates"><h3>theme credit</h3><a href="http://enchantedthemes.tumblr.com">enchantedthemes</a></div>
</div>
<!-- end statistics -->
 
</div>
 
<!-- end left sidebar -->
 
 
<!-- right sidebar -->
 
<div id="rightside">
 
<!-- updates -->
<div class="box">
<h1>updates</h1>
<div class="updates"><h3>Student A</h3>Feb.12, 2023</div>
<div class="updates"><h3>Student B</h3>Feb.19, 2023</div>
<div class="updates"><h3>Student C</h3>Feb.26, 2023</div>
</div>
<!-- end updates -->
 
<!-- affiliates-->
<div class="box">
<h1>affiliates</h1>
<div class="blogs">
    <img src="https://api.tumblr.com/v2/blog/blog.tumblr.com/avatar/128" /> 
    <a href="/">blog url</a>
</div>
<div class="blogs">
    <img src="https://api.tumblr.com/v2/blog/blog.tumblr.com/avatar/128" /> 
    <a href="/">blog url</a>
</div>
</div>
<!-- end affiliates-->
 
<!-- disclaimer-->
<div class="box">
<h1>disclaimer</h1>
    Not sponsored, we just love fashion and we are fashion majors(:
</div>
<!-- end disclaimer-->
 
</div>
 
<!-- end right sidebar -->
 
 
<div id="navi">
    <a href="{text:link 1 url}">{text:link 1 title}</a>
    <a href="{text:link 2 url}">{text:link 2 title}</a>
    <a href="{text:link 3 url}">{text:link 3 title}</a>
    <a href="{text:link 4 url}">{text:link 4 title}</a>
    <a href="{text:link 5 url}">{text:link 5 title}</a>
    <a href="{text:link 6 url}">{text:link 6 title}</a>
</div>
 
<div id="image"><img src="{image:header}"/></div>
 
 
<div id="topbar">
 
<div class="title">{title}</div>
    <div class="hnavi">
        <a href="{text:link 1 url}">{text:link 1 title}</a>
        <a href="{text:link 2 url}">{text:link 2 title}</a>
        <a href="{text:link 3 url}">{text:link 3 title}</a>
        <a href="{text:link 4 url}">{text:link 4 title}</a>
        <a href="{text:link 5 url}">{text:link 5 title}</a>
        <a href="{text:link 6 url}">{text:link 6 title}</a>
    </div>
    <div class="links">
        <a href="/" title="home"><i class="fa fa-home" aria-hidden="true"></i></a>
        {block:AskEnabled}<a href="/ask" title="inbox"><i class="fa fa-envelope" aria-hidden="true"></i></a>{/block:AskEnabled}
        {block:SubmitEnabled}<a href="/submit" title="submit"><i class="fa fa-bars" aria-hidden="true"></i></i></a>{/block:SubmitEnabled}
        <a href="https://tumblr.com/follow/{Name}" title="follow"><i class="fas fa-plus"></i></a>
        <a href="/"><img src="{PortraitURL-128}"/></a>
    </div>
</div>
 
 
<div id="entries">
 
{block:Posts}
 
<div class="posts" id="{PostID}">
 
 
{block:Date}
<div class="topinfo">
{block:RebloggedFrom}
<a href="{ReblogRootURL}"><img src="{ReblogRootPortraitURL-128}"/></a>
<div class="toptext">
<a href="{ReblogRootURL}" style="font-weight:600;">{ReblogRootName}</a>
{block:IndexPage}{block:NoteCount}<a href="{Permalink}" style="float:right;">{NoteCountWithLabel}</a>{/block:NoteCount}{/block:IndexPage}
{block:HomePage}{block:PinnedPostLabel}<div class="pinned">&ensp;:&ensp;<a href="{Permalink}">{PinnedPostLabel}</a></div>{/block:PinnedPostLabel}{/block:HomePage}
</div>
{/block:RebloggedFrom}
{block:NotReblog}
<a href="{Permalink}"><img src="{PortraitURL-128}"/></a>
<div class="toptext">
<a href="{Permalink}" style="font-weight:600;">{Name}</a>
{block:IndexPage}{block:NoteCount}<a href="{Permalink}" style="float:right;">{NoteCountWithLabel}</a>{/block:NoteCount}{/block:IndexPage}
{block:HomePage}{block:PinnedPostLabel}<div class="pinned">&ensp;:&ensp;<a href="{Permalink}">{PinnedPostLabel}</a></div>{/block:PinnedPostLabel}{/block:HomePage}
</div>
{/block:NotReblog}
</div>
{/block:Date}
 
 
{block:Text}
<div class="txt" id="{PostID}">
{block:Title}<h1>{Title}</h1>{/block:Title}
<div class="c">{Body}</div>
</div>
{/block:Text}
 
 
{block:Photo}
<a href="#" onclick="Tumblr.Lightbox.init([{ width: {PhotoWidth-HighRes}, height: {PhotoHeight-HighRes}, low_res: '{PhotoURL-500}', high_res: '{PhotoURL-HighRes}' }]); $('body').toggleClass('tumblr_lightbox_active'); return false">
    <img src="{PhotoURL-HighRes}" width="{select:post width}" id="photos" style="margin-bottom:-5px;">
</a>
{/block:Photo}
 
 
{block:Photoset}
<div class="photo-slideshow" id="photoset_{PostID}" data-layout="{PhotosetLayout}">{block:Photos}<div class="photo-data"><div class="pxu-photo"><img src="{PhotoURL-500}" width="{PhotoWidth-500}" height="{PhotoHeight-500}" data-highres="{PhotoURL-HighRes}" data-width="{PhotoWidth-HighRes}" data-height="{PhotoHeight-HighRes}"></div><a class="tumblr-box" rel="post-{PostID}" href="{PhotoURL-HighRes}"></a></div>{/block:Photos}</div>
{/block:Photoset}
 
 
{block:Quote}
<div class="quote">{Quote}</div>
{block:Source}<div class="quotesource">{Source}</div>{/block:Source}
{/block:Quote}
 
 
{block:Link}
<h1><a href="{URL}" {Target}>{Name}&ensp;>></a></h1>
{block:Description}<div class="c">{Description}</div>{/block:Description}
{/block:Link}
 
 
{block:Chat}
{block:Title}<h1>{Title}</h1>{/block:Title} <div class="chat"> {block:Lines} <li class="line {Alt}"> {block:Label} <span class="label"> {Label}</span> {/block:Label}{Line}</li> {/block:Lines}</div>
{/block:Chat}
 
 
{block:Audio}
<div class="audio">
<div class="playbox"><div class="playbutton">{block:AudioPlayer}{AudioPlayer}{/block:AudioPlayer}</div></div>
 
<div class="trackdetails">
{block:TrackName}<b>{TrackName}</b>{/block:TrackName} {block:Artist}by <i>{Artist}</i>{/block:Artist}
</div>
 
</div>
{/block:Audio}
 
 
{block:Video}
<div class="video">{Video-500}</div>
{/block:Video}
 
 
{block:Caption}
<div class="c">{Caption}</div>
{/block:Caption}
 
 
{block:Answer}
<div class="aicon"><img src="{AskerPortraitURL-128}" /></div>
<div class="asker"><b>{Asker}</b> asked:</div>
<div class="question">{Question}</div>
<div class="answer"><div class="c">{Answer}</div></div>
{/block:Answer}
 
 
{block:Date}
<div class="info">
<a href="{PostAuthorURL}"><img src="{PostAuthorPortraitURL-128}"/></a>
<div class="dtext">
{block:IndexPage}
Posted {TimeAgo} by <a href="{PostAuthorURL}">{PostAuthorName}</a> on <b><a href="{Permalink}" title="{TimeAgo}" style="text-transform:capitalize;">{DayOfMonth} {Month}</a></b>
{/block:IndexPage}
{block:PermalinkPage}
Posted {TimeAgo} on <span style="text-transform:capitalize;">{DayOfMonth} {Month}, {Year}</span>
{/block:PermalinkPage}
</div>
 
{block:IndexPage}
{block:ifshowcontrolsonindex}
<div class="custom-like-button">
  {LikeButton}
<span class="likes"><i class="fa fa-heart" aria-hidden="true"></i></span>
</div>
<a href="{ReblogURL}"><i class="fa fa-undo" aria-hidden="true"></i></a>
{/block:ifshowcontrolsonindex}
{/block:IndexPage}
 
{block:PermalinkPage}
<div class="custom-like-button">
<div class="like_button">
  {LikeButton}
</div>
<span class="likes"><i class="fa fa-heart" aria-hidden="true"></i></span>
</div>
<a href="{ReblogURL}"><i class="fa fa-undo" aria-hidden="true"></i></a>
<div style="margin:5px 40px -2.5px;">
{block:NotReblog}Original post<br>{/block:NotReblog}
{block:RebloggedFrom}
Reblogged from <a href="{ReblogParentURL}" title="{ReblogParentTitle}">{ReblogParentName}</a>
{block:ContentSource},&nbsp;&nbsp;&nbsp;Source <a href="{ReblogRootURL}" title="{ReblogRootTitle}">{ReblogRootName}</a>{/block:ContentSource}<br>
{/block:RebloggedFrom} 
Posted by <a href="{PostAuthorURL}">{PostAuthorName}</a>
</div>
{/block:PermalinkPage} 
</div>
{/block:Date}
 
{block:Date}
{block:HasTags}
<div id="tags">
Tagged:&ensp;{block:Tags}<a href="{TagURL}">#{Tag}</a>{/block:Tags}
</div>
{/block:HasTags}
{/block:Date}
 
 
</div>
 
 
{block:PostNotes}
{block:NoteCount}<div style="font-size:calc({select:font size} + 2px); font-weight:700; color:{color:title}">{NoteCountWithLabel}</div>{/block:NoteCount}
{PostNotes}
{/block:PostNotes}
 
{/block:Posts}
 
 
</div>
 
 
{block:Pagination}{block:ifloadmore}
<footer><a id="loadmore">load more posts</a></footer>
{/block:Pagination}{/block:ifloadmore}
 
 
{block:Pagination}
<div id="pagination">
{block:Previouspage}
<a href="{PreviousPage}" title="back"><i class="fa fa-angle-left"></i></a>{/block:PreviousPage}
{block:JumpPagination length="3"}
{block:CurrentPage}
<span class="current_page" style="margin-right:10px; font-weight:700;">{PageNumber}</span>
{/block:CurrentPage}
{block:JumpPage}
<a class="jump_page" href="{URL}">{PageNumber}</a>
{/block:JumpPage}
{/block:JumpPagination}
{block:NextPage}
<a class="next" href="{NextPage}" title="next"><i class="fa fa-angle-right"></i></a>
{/block:Nextpage}
</div>
{/block:Pagination}
 
 
{block:ContentSource}
<!-- {SourceURL}{block:SourceLogo}<img src=â€{BlackLogoURL}â€
width=â€{LogoWidth}â€ height=â€{LogoHeight}â€ alt=â€{SourceTitle}â€ />
{/block:SourceLogo}
{block:NoSourceLogo}{SourceLink}{/block:NoSourceLogo} -->
{/block:ContentSource}{block:ReblogParent}{/block:ReblogParent}
 
 
{block:ifscrolltotop}
<div class="st"><a href="#">scroll to top</a></div>
{/block:ifscrolltotop}
 
 
<div class="tc">
    <i class="fa fa-bars" aria-hidden="true"></i>
</div>
 
 
<!-- credit - DO NOT TOUCH -->
 
<div class="credit">
    <a href="http://enchantedthemes.tumblr.com" title="alydae">A.</a>
</div>
 
<!--- scripts --->
 
<!-- npfPhotosets script by @codematurgy -->
<script src="https://cdn.jsdelivr.net/gh/boscoxvi/npfphotosets/npfphotosets.js"></script><link href="https://cdn.jsdelivr.net/gh/boscoxvi/npfphotosets/npfphotosetstyle.css" rel="stylesheet" type="text/css">
<script>
npfPhotosets(".posts", {
   includeCommonPhotosets: true,
   photosetMargins:"4"
});
</script>
 
<!-- un-next captions script by @neothm and @magnusthemes -->
<script src="https://static.tumblr.com/wgg6svp/OoTofxa0c/unnest.min.js"></script>
 
<script> 
$(document).ready(function(){
    $('.posts').unnest({ 
    yourCaption: ".c", 
    wrapName: ".tumblr_parent",
    newCaptionUsername: true, 
    originalPostCaptionUsername: false,
    tumblrAvatars: true,
    tumblrAvatarClass: ".tumblr_avatar", 
    usernameColon: false 
}); 
}); 
</script>
 
<!--- tooltips script --->
<script src="https://static.tumblr.com/rzl30kg/eAxm7a751/jquery.style-my-tooltips.js"></script>
 
<script type="text/javascript">
 
//tooltips
(function($){
    $(document).ready(function(){
        $("[title]").style_my_tooltips({
            tip_follows_cursor:true,
            tip_delay_time:200,
            tip_fade_speed:300
        });
    });
})(jQuery);
 
//sticky    
$(function(){
    var stickyRibbonTop = $('#topbar').offset().top;
    $(window).scroll(function(){
        if( $(window).scrollTop() > stickyRibbonTop ) {
            $('#topbar').css({position: 'fixed', top: '0px'});
        } else {
            $('#topbar').css({position: 'relative', top: '0px'});
        }
    });
});
 
//scroll to top
{block:ifscrolltotop}
$(window).scroll(function() {
	if ( $(window).scrollTop() > 100 ) {
		$('.st').fadeIn('slow');
	} else {
		$('.st').fadeOut('slow');
	}
});
$('.st').click(function() {
	$('html, body').animate({scrollTop: 0}, 700);
	return false;
});
{/block:ifscrolltotop}
 
</script>
 
<!-- infinite scroll -->
{block:ifInfiniteScroll}
<script src="https://static.tumblr.com/wgijwsy/u2vm2hxv6/jquery.infinitescroll.min.js"></script>
{/block:ifInfiniteScroll}
 
{block:ifInfiniteScroll}
<script type="text/javascript">
$(document).ready(function(){
    var $container = $('#entries');
        $container.infinitescroll({
            itemSelector: '.posts',
            navSelector: '#pagination',
            nextSelector: '.next',
            loadingImg: '',
            loadingText: '<em></em>',
            {block:ifloadmore}
            errorCallback: function () {$('a#loadmore:last').fadeOut();},
            {/block:ifloadmore}
            bufferPx: 2000,
        },
        function( newElements ) {
            var $newElems = $( newElements );
        $newElems.find('.photo-slideshow').pxuPhotoset({
            lightbox: true,
            rounded: false,
            gutter: '4px',
            photoset: '.photo-slideshow',
            photoWrap: '.photo-data',
            photo: '.pxu-photo',
        });
        resizeVideos();
        $newElems.unnest({
            yourCaption: ".c", 
            wrapName: ".tumblr_parent",
            newCaptionUsername: true, 
            originalPostCaptionUsername: false,
            tumblrAvatars: true,
            tumblrAvatarClass: ".tumblr_avatar", 
            usernameColon: false 
        });
        var $newElemsIDs = $newElems.map(function(){ 
            return this.id; 
        }).get();
        console.log($newElems, $newElemsIDs);
        Tumblr.LikeButton.get_status_by_post_ids($newElemsIDs);
        });
        {block:ifloadmore}
        $(window).unbind('.infscr'); 
        $('a#loadmore').click(function(){ 
        $('#entries').infinitescroll('retrieve');
        return false; 
        });
        {/block:ifloadmore}
});
</script>
{/block:ifInfiniteScroll}
 
</body>
