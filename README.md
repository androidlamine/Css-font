<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:defaultwidgetversion='2' b:layoutsVersion='3' b:responsive='true' b:templateUrl='rockpool.xml' b:templateVersion='1.0.0' expr:dir='data:blog.languageDirection' expr:lang='data:blog.locale' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <meta content='width=device-width, initial-scale=1' name='viewport'/>
    <title>
      <b:if cond='data:view.isError'>Page Not Found | </b:if>
      <b:if cond='data:view.isSearch or data:view.isArchive'>
        <b:eval expr='data:blog.pageName ? data:blog.pageName + &quot; | &quot; : &quot;&quot;'/>
      </b:if>
      <data:view.title/>
    </title>
    <b:include data='blog' name='all-head-content'/>
    <meta content='website' property='og:type'/>
    <meta content='summary_large_image' name='twitter:card'/>
<link href='https://fonts.googleapis.com/css?family=Cairo|Tajawal' rel='stylesheet'/>  
    <!-- Theme CSS -->
    <link href='//fonts.googleapis.com/css?family=Changa:300,400,500,700' rel='stylesheet'/>
    <link href='//ar-themes.github.io/templates/themeforest/salbuta/plugins-rtl.min.css' rel='stylesheet'/>

    <b:skin version='1.0.0'><![CDATA[/*
-------------------------------------------
Responsive Blogger Theme Style
Name:   Salbuta - v1.1 - RTL
link: Androidlamine.blogspot.com

------------------------------------------- */
/* Variables
-------------------------------
<Variable name="keycolor" description="Main color" type="color" default="#007bff"  value="#007bff"/>

<Group description="Global">
<Variable name="body.text.font" description="Font" type="font" default="normal normal 1rem 'Poppins', sans-serif"  value="normal normal 1rem &#39;Changa&#39;, sans-serif"/>
<Variable name="body.text.color" description="Text Color" type="color" default="#333"  value="#333333"/>
<Variable name="body.link.color" description="Link Color" type="color" default="#007bff"  value="#007bff"/>
<Variable name="body.link.hover.color" description="Hover Link Color" type="color" default="#0056b3"  value="#0056b3"/>
</Group>
<Group description="Header">
<Variable name="header.bg.color.1" description="Background Color 1" type="color" default="#c4183c"  value="#c4183c"/>
<Variable name="header.bg.color.2" description="Background Color 2" type="color" default="#4f37ac"  value="#4f37ac"/>
</Group>
<Group description="Footer">
<Variable name="footer.bg.color.1" description="Background Color 1" type="color" default="#c4183c"  value="#c4183c"/>
<Variable name="footer.bg.color.2" description="Background Color 2" type="color" default="#4f37ac"  value="#4f37ac"/>
</Group>

<Variable name="body.background" description="Background" color="#eee" type="background" default="$(color) none repeat scroll top left"  value="$(color) url() repeat scroll top center"/>

<Variable name="3bold" description="300 Bold Weight" type="font" default="300 1rem $(body.text.font.family)" hideEditor="true" value="300 1rem &#39;Changa&#39;, sans-serif"/>
<Variable name="5bold" description="500 Bold Weight" type="font" default="500 1rem $(body.text.font.family)" hideEditor="true" value="500 1rem &#39;Changa&#39;, sans-serif"/>
<Variable name="7bold" description="700 Bold Weight" type="font" default="700 1rem $(body.text.font.family)" hideEditor="true" value="700 1rem &#39;Changa&#39;, sans-serif"/>

<Variable name="header.background" description="Header Full Background" type="color" hideEditor="true" default="#7d99a4" value="#7d99a4"/>
<Variable name="body.background.color" description="Body Background Color" type="color" hideEditor="true" default="#fff"  value="#ffffff"/>
<Variable name="item.action.color" description="Action color" type="color" default="$(body.text.color)" hideEditor="true" value="#444444"/>
<Variable name="item.action.font" description="Action font" type="font" default="700 15px Oswald, serif" hideEditor="true" value="700 15px Oswald, serif"/>
*/

/* Global
------------------------------- */
html[dir="rtl"][lang]{direction:rtl!important}
body{background:$(body.background);color:$(body.text.color);font:$(body.text.font);line-height:1.42857143;margin:0;min-height:100vh}
body.single_view:not(.light){background-color:#fff}
a,a:hover,a:focus{text-decoration:none;outline:none}
a,button,input,textarea,.btn,.contact-note p,.post_snippet_text,.post_share_buttons{-webkit-transition:all 0.3s ease 0s;-o-transition:all 0.3s ease 0s;transition:all 0.3s ease 0s}
a,a:focus,.uk-spinner,.uk-form-icon:hover,.uk-button-link{color:$(body.link.color)}
.uk-totop,.uk-tab>.uk-active>a{border-color:$(body.link.color)}
.uk-tooltip,.uk-totop,.uk-open>.uk-accordion-title{background:$(body.link.color)}
.uk-icon-button:focus,.uk-icon-button:hover,.uk-active>.uk-icon-button,.uk-icon-button:active,.uk-button-default:focus,.uk-button-default:hover,.uk-button-default.uk-active,.uk-button-default:active{background-color:$(body.link.hover.color)}
.uk-button-default:focus,.uk-button-default:hover,.uk-button-default.uk-active,.uk-button-default:active,.uk-totop:active,.uk-totop:focus,.uk-totop:hover{border-color:$(body.link.hover.color)}
a:hover,.uk-button-link:focus,.uk-button-link:hover{color:$(body.link.hover.color)}
.uk-totop:active,.uk-totop:focus,.uk-totop:hover,.uk-accordion-title:focus,.uk-accordion-title:hover{background:$(body.link.hover.color)}
.uk-slidenav,.uk-slidenav:hover{color:$(keycolor)}
.uk-slidenav:not(.uk-invisible):hover{opacity:.7}
.uk-slidenav.uk-invisible{visibility:visible!important;opacity:.4}
.uk-dotnav > * > *{width:12px;height:12px;border:1px solid $(keycolor)}
.uk-dotnav > * >:focus,.uk-dotnav > * >:hover,.uk-dotnav > .uk-active > *{background:$(keycolor);border-color:transparent}
.uk-h1,.uk-h2,.uk-h3,.uk-h4,.uk-h5,.uk-h6,h1,h2,h3,h4,h5,h6{font:$(5bold)}
.uk-h1,h1{font-size:2.23125rem;line-height:1.2}
.uk-h2,h2{font-size:1.7rem;line-height:1.3}
.uk-h3,h3{font-size:1.5rem;line-height:1.4}
.uk-h4,h4{font-size:1.25rem;line-height:1.4}
.uk-h5,h5{font-size:1rem;line-height:1.4}
.uk-h6,h6{font-size:.875rem;line-height:1.4}
.item-control,.options{display:none}
.clip{border:0;clip:rect(1px,1px,1px,1px);height:1px;width:1px;overflow:hidden;padding:0;position:absolute}
.hidden{display:none!important}

/* .wrapper
------------------------------- */

/* header + footer
------------------------------- */
header{background-color:$(header.bg.color.1);background-image: -webkit-gradient(linear,left top,right top,from($(header.bg.color.1)),to($(header.bg.color.2)));background-image: linear-gradient(to right,$(header.bg.color.1),$(header.bg.color.2));position:relative;padding-top:60px;padding-bottom:40px;z-index:4}
header>div,:not(blockquote)>footer>div{position:relative;z-index:2}
.no_waves header{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}

/* .topnav */
.topnav .sidenav_button a{border-color:transparent}
.topnav .topnav_social li a{background:$(body.text.color);color:#fff;font-size:0;height:40px;width:40px;line-height:40px;text-align:center}
.topnav .topnav_social li a:hover,.topnav .topnav_social li a:focus{background:$(keycolor);color:#fff}

/* .mainnav */
.mainnav_wrapper:not(.uk-sticky-fixed){height:60px}
.mainnav .header-image-wrapper{display:flex;height:60px;width:100%;align-items:center}
.mainnav .header-image-wrapper img{height:60px;-webkit-transition:height 0.3s ease-in-out 0s;-o-transition:height 0.3s ease-in-out 0s;transition:height 0.3s ease-in-out 0s}
.mainnav_menu > ul > li:not(:last-child){margin-right:20px;margin-left:20px}
.mainnav_menu > ul > li:last-child{margin-right:20px}
.mainnav_menu > ul > li > ul{display:none}
.mainnav_menu.uk-navbar-container{background:transparent;position:static}
.mainnav_menu .uk-navbar-nav > li > a{color:#fff;min-height:60px;font-family:inherit;font-weight:300;position:relative;padding:0;margin:0;text-transform:capitalize;transition-duration:.3s;transition-property:color,background-color,min-height}
.mainnav_menu .uk-navbar-nav > li > a:hover,.mainnav_menu .uk-navbar-nav > li > a:focus{color:#fff}
.mainnav_menu .uk-navbar-nav > li > a:before{background:#fff;content:'';display:block;position:absolute;right:0;left:100%;bottom:0;height:1px;background-color:currentColor;transition:all .3s ease-in-out}
.mainnav_menu .uk-navbar-nav > li:hover > a:before,.mainnav_menu .uk-navbar-nav > li > a.uk-open:before,.mainnav_menu .uk-navbar-nav > li.current > a:before{left:0}
.mainnav_menu .uk-navbar-nav > li > a.uk-open:after{left:0}
.mainnav_menu .uk-navbar-nav > li > a:not(.icon_search) svg{-webkit-transition:all 0.3s ease 0s;-o-transition:all 0.3s ease 0s;transition:all 0.3s ease 0s}
.mainnav_menu .uk-navbar-nav > li > a.uk-open:not(.icon_search) svg{-webkit-transform:rotate(45deg);transform:rotate(45deg)}
.mainnav_menu .uk-navbar-nav > li li{position:relative}
.mainnav_menu .uk-navbar-nav > li li .uk-navbar-dropdown{right:calc(100% + 20px)!important;top:0!important}
.mainnav_menu .uk-navbar-nav > li li a{font-size:90%}
.mainnav_menu .uk-navbar-nav > li li a,.mainnav_menu .uk-navbar-nav > li li a:focus{color:#999}
.mainnav_menu .uk-navbar-nav li li:hover > a,.mainnav_menu .uk-navbar-nav li li.current > a{color:$(keycolor)}
.mainnav_menu .uk-navbar-nav .uk-navbar-dropdown{min-width:200px;width:auto;margin-top:0;top:60px!important}
[dir="ltr"] .mainnav_menu .mega_menu{right:40px!important;left:0!important}
[dir="rtl"] .mainnav_menu .mega_menu{left:40px!important;right:0!important}
.mainnav_menu .mega_menu{background:#f1f1f1;padding:0;top:60px!important}
.mainnav_menu .has_single_mega > .mega_menu{padding:25px}
.thumb_video{background-position:center;background-repeat:no-repeat;background-size:cover}
.thumb_video img{opacity:0}
.mainnav_menu .mega_menu .post_thumbnail a{color:#fff}
.mainnav_menu .mega_menu .post_content{padding:15px!important}
.mainnav_menu .mega_menu .post_title{font-size:16px;line-height:1.4;margin-bottom:15px}
.mainnav_menu .mega_menu .post_title a{color:#333}
.mainnav_menu .mega_menu .uk-tab{background:#fff;height:100%;margin-left:0;overflow:hidden;padding:20px 0 20px 20px}
.mainnav_menu .mega_menu .uk-tab:before,.mainnav_menu .mega_menu .uk-tab:after{display:none}
.mainnav_menu .mega_menu .uk-tab > li > a{border-left:0;padding:13px 15px;-webkit-transition:all 0.3s ease 0s;-o-transition:all 0.3s ease 0s;transition:all 0.3s ease 0s}
.mainnav_menu .mega_menu .uk-tab > .uk-active > a,.mega_menu .uk-tab > li:hover > a:hover{border:0;background:#f1f1f1;color:$(keycolor);border-radius:50px 0 0 50px;padding-right:15px}
.mainnav_menu .mega_menu .uk-switcher{padding:25px 25px 25px 16px}
.mega[data-label] [data-uk-spinner]{min-height:100px;line-height:100px}
.featured_error,.no_results,.no_matching_results:before{color:#ff0000;line-height:1.5}
.has_single_mega .featured_error{text-align:center}
.no_results,.no_matching_results:before{background:#fff;padding:20px 25px;border-radius:4px;-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}
.no_matching_results:before{width:100%;margin-right:40px}

/* .uk-navbar-sticky */
.mainnav_wrapper.uk-sticky-fixed{background-color:$(header.bg.color.1);background-image: -webkit-gradient(linear,left top,right top,from($(header.bg.color.1)),to($(header.bg.color.2)));background-image: linear-gradient(to right,$(header.bg.color.1),$(header.bg.color.2));-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}
.mainnav_wrapper.uk-sticky-fixed .mainnav .Header .header-image-wrapper{height:50px}
.mainnav_wrapper.uk-sticky-fixed .mainnav .Header .header-image-wrapper img{height:40px}
.mainnav_wrapper.uk-sticky-fixed .mainnav .mainnav_menu .uk-navbar-nav > li > a{min-height:50px}
.mainnav_wrapper.uk-sticky-fixed .mainnav .mainnav_menu .uk-navbar-dropdown,.mainnav_wrapper.uk-sticky-fixed .mainnav .mainnav_menu .mega_menu{top:50px!important}
.mainnav_wrapper.uk-sticky-fixed .mainnav .mainnav_menu .uk-navbar-nav > li li .uk-navbar-dropdown{top:0!important}

/* .sidemenu */
.sidemenu ul,.sidemenu li{list-style:none;margin:0;padding:0}
.sidemenu .uk-accordion{border:0;border-radius:0;box-shadow:none}
.sidemenu .sidemenu_list{padding:80px 0;border-bottom:0}
.sidemenu .sidemenu_list :not(.post_thumbnail):not(.post_title) > a{background:transparent;color:#fff;display:block;position:relative;font-size:inherit;line-height:inherit;border-bottom:0;text-transform:none;padding:12px 30px}
.sidemenu .sidemenu_list :not(.post_thumbnail):not(.post_title) > a > span{color:#fff;float:left;line-height:inherit}
.sidemenu .sidemenu_list .current > a,.sidemenu .sidemenu_list .current > div > a{border-right:3px solid $(keycolor);padding-right:27px}
.sidemenu .sidemenu_list .current > a,.sidemenu .sidemenu_list .current > div > a,.sidemenu .sidemenu_list .uk-open > a,.sidemenu .sidemenu_list li > a:focus,.sidemenu .sidemenu_list li > div > a:focus{color:$(keycolor)!important}
.sidemenu .sidemenu_list li > a:hover,.sidemenu .sidemenu_list li > div > a:hover{background:$(keycolor)!important;color:#fff!important}
.sidemenu .sidemenu_list > li ul,.sidemenu .sidemenu_list li.has_single_mega .mega{background:#333;border-bottom:0}
.sidemenu .sidemenu_list > li ul :not(.post_thumbnail):not(.post_title) > a{font-size:14px}
.sidemenu .sidemenu_list > li ul ul{background:#444;padding:0}
.sidemenu .sidemenu_list li .featured_error{background:#333;color:#fff;padding:30px;text-align:center}
.sidemenu .sidemenu_list li.has_single_mega .blog_posts{padding:30px}
.sidemenu .sidemenu_list li.has_single_mega .blog_posts li{margin-bottom:30px}
.sidemenu .sidemenu_list li.has_single_mega .blog_posts li:last-child{margin-bottom:0}
.sidemenu .sidemenu_list li.has_multi_mega ul{padding-right:0}
.sidemenu .sidemenu_list li.has_multi_mega .blog_posts{padding:30px}
.sidemenu .sidemenu_list li.has_multi_mega .mega,.sidemenu .sidemenu_list li.has_multi_mega .featured_error{background:#444}
.sidemenu .sidemenu_list li.has_multi_mega .blog_posts li{margin-bottom:30px}
.sidemenu .sidemenu_list li.has_multi_mega .blog_posts li:last-child{margin-bottom:0}
.sidemenu .sidemenu_list li.has_mega .blog_posts .post_title{font-size:14px;line-height:24px}

/* main
------------------------------- */
main{position:relative;z-index:3}
main .main_content{margin-top:50px;margin-bottom:70px}
.error_view{background:url('https://3.bp.blogspot.com/-9FmvwdH6NtA/XHNTKm-cOeI/AAAAAAAAGl4/0HFJkQHaRsA34uW44dXTclRn0uPs80RoACLcBGAs/s1600/brick-wall.png');background-repeat:repeat;background-repeat:repeat}

/* .top_bg + .bottom_bg */
.top_bg > svg:not(.hidden),.bottom_bg > svg:not(.hidden){display:block}
.top_bg svg .g_fill_1{color:$(header.bg.color.1)}
.top_bg svg .g_fill_2{color:$(header.bg.color.2)}
.bottom_bg svg .g_fill_1{color:$(footer.bg.color.1)}
.bottom_bg svg .g_fill_2{color:$(footer.bg.color.2)}
.bottom_bg svg{-webkit-transform:scale(1,-1.01);transform:scale(1,-1.01)}

/* .filtering_labels */
.filtering_labels .mark{background-color:#eee;border:1px solid #aaa;border-radius:0;cursor:default}
.filtering_labels .select_label a{padding:0 10px}
.filtering_labels .select_label a:not(.uk-active):not(:hover):not(:active):not(:focus){border-color:#fff}
.filtering_labels .select_view a{height:40px;width:40px}
.filtering_labels .breadcrumb .uk-breadcrumb li a,.breadcrumb .uk-breadcrumb li span{text-transform:uppercase;line-height:40px;font-size:14px;font-weight:300;letter-spacing:1px}
.filtering_labels .breadcrumb .uk-breadcrumb li a{color:$(keycolor)}
.filtering_labels .breadcrumb .uk-breadcrumb li a:hover,.breadcrumb .uk-breadcrumb li span{color:#333}

/* .blog_posts + .blog_pager */
.blog_posts .post_thumbnail a{color:#fff}
.blog_posts .post_thumbnail a img{display:block;width:100%}
.blog_posts .post_title{font-size:18px;font-weight:500;line-height:28px;text-transform:uppercase}
.blog_posts .post_title a{color:#333}
.blog_posts .post_title a:hover,.blog_posts .post_title a:focus{color:$(keycolor)}
.blog_posts .post_labels a{font-size:13px;font-weight:300}
.blog_posts .post_snippet{font-size:14px;font-weight:300;line-height:24px;color:#888;margin-bottom:30px}
.blog_posts .post_snippet_text,.blog_posts .post_snippet.open .post_share_buttons{opacity:1;visibility:visible}
.blog_posts .post_snippet.open p,.blog_posts .post_snippet .post_share_buttons{opacity:0;visibility:hidden}
.blog_posts .post_share_buttons span,.single_post .post_share_buttons span{background:#333;color:#fff;line-height:36px;cursor:pointer}
.blog_posts .post_share_buttons span:hover,.blog_posts .post_share_buttons span:focus,.single_post .post_share_buttons span:hover,.single_post .post_share_buttons span:focus{background:$(body.link.hover.color);color:#fff;line-height:36px}
.blog_posts .post_meta{font-size:11px;font-weight:300;color:#333;text-transform:uppercase;letter-spacing:.5px}
.blog_posts .post_meta .post_share .action{cursor:pointer}
.blog_posts .post_meta .post_share .action:hover,.blog_posts .post_meta .post_share .action.uk-active{color:$(keycolor)}
.blog_posts .post_labels a:hover,.blog_posts .post_snippet_text a:hover,.blog_posts .post_body a:hover{text-decoration:underline}
.blog_pager a:not(:hover):not(:active):not(:focus){border-color:#fff}
.blog_pager a.loading,.blog_pager a.loading:hover{cursor:default;background:#fff;color:$(keycolor);padding:5px;border:0;line-height:0}

/* .inline_ad */
.inline_ad em{font-size:0;line-height:0;letter-spacing:0;float:right}
.single_post .inline_ad{margin-bottom:30px} 

/* .single_post + .full_header */
.single_post .post_title,.single_post .post_header,.single_post .post_footer,.full_header .post_title,.full_header .post_header{font-weight:300;font-size:38px}
.single_post .post_header,.full_header .post_header{font-size:12px}
.single_post .post_header a,.single_post .post_footer a,.full_header .post_header a,.full_header .post_footer a{color:$(keycolor)}
.single_post .post_header a:hover,.single_post .post_footer a:hover,.full_header .post_header a:hover,.full_header .post_footer a:hover{color:#333}
.single_post .post_header .post_header_line > span,.single_post .post_footer .post_footer_line > span,.full_header .post_header .post_header_line > span,.full_header .post_footer .post_footer_line > span{display:inline-block}
.single_post .post_header .post_header_line .post_reactions iframe,.single_post .post_footer .post_footer_line .post_reactions iframe,.full_header .post_header .post_header_line .post_reactions iframe,.full_header .post_footer .post_footer_line .post_reactions iframe{height:26px}
.single_post .post_share_label,.full_header .post_share_label{float:right;height:36px;line-height:36px}
.single_post .post_footer{font-size:14px}
.single_post .post_author_profile{background:#f9f9f9;border:1px solid #f1f1f1;padding:20px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.05);box-shadow:0 5px 10px rgba(0,0,0,0.05)}
.single_post .post_author_profile .post_author_profile_photo img,.single_post .post_author_profile .post_author_profile_name img{border-radius:500px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.15);box-shadow:0 5px 10px rgba(0,0,0,0.15)}
.single_post .post_author_profile .post_author_profile_name{font-weight:500}
.single_post .post_author_profile .post_author_profile_desc{font-weight:300;color:#444;line-height:1.6}
.full_header{background-color:#fff;background-repeat:no-repeat;background-size:cover;background-position:center;margin-bottom:40px;padding:50px 0;position:relative;-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}
.full_header:before{content:'';position:absolute;top:0;right:0;width:100%;height:100%;z-index:1;background:#fff;opacity:0.92}
.full_header .uk-container{position:relative;z-index:2}
.full_header .post_header{margin-bottom:0!important}
.has_full_header{position:relative;background-color:#fff;background-repeat:no-repeat;background-size:cover;background-position:center;-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}
.has_full_header > svg{position:relative;z-index:2}
.has_full_header .full_header{background:transparent;position:static;-webkit-box-shadow:none;box-shadow:none}

/* .post_body */
.single_post .post_body{line-height:1.6}
.single_post .post_body a:hover{text-decoration:underline}
.single_post .post_body a.uk-button:hover{text-decoration:none;color:#fff}
.single_post .post_body ul{line-height:30px}
.single_post .post_body blockquote{font-size:17px;font-weight:300;border-right:5px solid $(keycolor);padding:0 20px}
.single_post .post_body a.uk-accordion-title,.single_post .post_body .uk-tab > * > a,.single_post .post_body a.uk-accordion-title:hover,.single_post .post_body .uk-tab > * > a:hover{text-decoration:none}

/* .post_related */
.post_related{margin:0 -15px 15px;padding:0 15px 25px;overflow:hidden;position:relative}
.post_related .uk-slider{overflow:visible}
.post_related .post_related_title{background:#f9f9f9;font-size:14px;font-weight:700;line-height:30px;letter-spacing:1px;margin:0 0 25px;padding:8px 20px;text-transform:uppercase;border:1px solid #f1f1f1;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.05);box-shadow:0 5px 10px rgba(0,0,0,0.05)}
.post_related .blog_posts{margin-bottom:20px}
.post_related .blog_posts .uk-card-default{box-shadow:0 3px 10px rgba(0,0,0,.08)}
.post_related .blog_posts .uk-card-default:hover{box-shadow:0 5px 15px rgba(0,0,0,.16)}
.post_related .blog_posts .post_title{font-size:16px;line-height:1.4;font-weight:500;text-overflow:ellipsis;overflow:hidden;white-space:nowrap}
.post_related .blog_posts .post_title a{font-size:90%}
.single_post .post_related .uk-slidenav{position: absolute;top:-65px;left:10px}
.single_post .post_related .uk-slidenav[data-uk-slidenav-previous]{left:44px}

/* .post_comments */
.single_post .post_comments:not(.uk-width-auto){border:1px solid #f1f1f1;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.05);box-shadow:0 5px 10px rgba(0,0,0,0.05)}
.single_post .post_comments .post_comments_title{background:#f9f9f9;font-size:14px;font-weight:700;line-height:30px;letter-spacing:1px;margin:0;padding:8px 20px;text-transform:uppercase}
.single_post .post_comments .post_comments_content{background:#fff;padding:30px 20px}
.single_post .post_comments .post_comments_content ol,.single_post .post_comments .post_comments_content li{list-style:none;margin:0;padding:0}
.single_post .post_comments .post_comments_content li{border-top:1px solid rgba(0,0,0,0.1);padding:30px 0}
.single_post .post_comments .post_comments_content li:first-child{border-top:0;padding-top:0}
.single_post .post_comments .post_comments_content li:last-child{border-bottom:1px solid rgba(0,0,0,0.1)}
.single_post .post_comments .post_comments_content li .avatar-image-container{margin-bottom:30px;position:relative}
.single_post .post_comments .post_comments_content li .avatar-image-container:before,.single_post .post_comments .post_comments_content li .avatar-image-container:after,.single_post .post_comments .post_comments_content li .avatar-image-container:before,.single_post .post_comments .post_comments_content li .avatar-image-container:after{content:"";display:table}
.single_post .post_comments .post_comments_content li .avatar-image-container:after,.single_post .post_comments .post_comments_content li .avatar-image-container:after{clear:both}
.single_post .post_comments .post_comments_content li .avatar-image-container > img{background:url(https://2.bp.blogspot.com/-SMMGhBOTQjY/WXf6weOcZnI/AAAAAAAAFLQ/1I1u3ga-qIQzqrxrfegjrONx9MnQgsUcwCLcBGAs/s1600/user.png);background-repeat:repeat;background-position-x:0%;background-position-y:0%;background-size:auto auto;background-size:35px;background-repeat:no-repeat;background-position:center;border-radius:500px;float:right;height:45px;width:45px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.15);box-shadow:0 5px 10px rgba(0,0,0,0.15)}
/*.single_post .post_comments .post_comments_content ol ol li .avatar-image-container > img{height:50px;width:50px}*/
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header{font-size:14px;font-weight:300;position:absolute;top:50%;right:65px;border-right:1px solid #eee;padding-right:20px;z-index:1;-webkit-transform:translateY(-50%);transform:translateY(-50%)}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header a{color:currentColor;font-style:normal;text-transform:uppercase}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header a:hover{color:$(keycolor)}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header .icon.blog-author{margin-right:10px}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header .icon.blog-author:after{background:$(keycolor);color:#fff;border-radius:4px;content:'Admin';font-size:12px;padding:2px 5px}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header .datetime{margin-top:10px;text-transform:lowercase;font-size:12px;display:block;color:#999}
.single_post .post_comments .post_comments_content li .comment-block{font-size:15px;padding-right:85px}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-actions{font-size:13px;font-weight:300;letter-spacing:1px;left:0;top:50%;text-transform:uppercase;position:absolute;z-index:2;-webkit-transform:translateY(-50%);transform:translateY(-50%)}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-actions > * + *{margin-right:15px}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-actions > span a{color:red}
.single_post .post_comments .post_comments_content .comment-thread ol ol li{background:#f9f9f9;border:1px dashed $(keycolor);border-radius:4px 4px 0 0;position:relative;margin-right:85px;padding:30px 20px}
.single_post .post_comments .post_comments_content .comment-thread ol ol li+li{border-top:0;border-radius:0 0 4px 4px}
.single_post .post_comments .post_comments_content .comment-thread ol ol li:last-child{border-bottom-right-radius:4px;border-bottom-left-radius:4px}
/*.single_post .post_comments .post_comments_content .comment-thread ol ol li:before{background:rgba(0,0,0,.1);content:'';height:1px;top:0;right:20px;left:20px;position:absolute;z-index:200}*/
.single_post .post_comments .post_comments_content .comment-thread ol ol li:first-child{margin-top:30px}
.single_post .post_comments .post_comments_content .comment-thread ol ol li:first-child:before{display:none}
.single_post .post_comments .post_comments_content li .comment-block .comment-content{margin-bottom:0}
.single_post .post_comments .post_comments_content li .comment-block .deleted-comment{font-style:italic;color:#999;font-size:14px}
.single_post .post_comments iframe#comment-editor{background:#fff url(https://2.bp.blogspot.com/-0NRT3RqZ-UE/WXaJxtQDL6I/AAAAAAAAFLA/P7rVvFYoC3UAeLeflj0n-fSdJWChSW9CQCLcBGAs/s1600/loader.gif) no-repeat center;margin-top:30px;padding-right:20px;padding-left:20px;border-left:1px dashed #ccc;border-right:1px dashed #ccc;max-width:100%;box-sizing:border-box}
.single_post .post_comments .post_comments_content .loadmore{margin-top:20px}
.single_post .post_comments .post_comments_content .loadmore.loaded{max-height:0;opacity:0;overflow:hidden;margin-top:0}
.single_post .post_comments .post_comments_content .post_comments_message{background:#eee;border-radius:5px;margin-top:20px;padding:12px 20px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.05);box-shadow:0 5px 10px rgba(0,0,0,0.05)}
.single_post .post_comments .continue{margin-top:20px}
.single_post .post_comments .continue a{line-height:20px;display:inline-block}
.single_post .post_comments ol .continue,.single_post .post_comments .comments_locked .continue,.single_post .post_comments .comment-thread .thread-count,/*.single_post .post_comments .post_comments_content .post_comments_form,*/.single_post .post_comments .post_comments_content.comments_locked li .avatar-image-container .comment-actions > a{display:none!important}
.single_post .post_comments .comments_emotions .comments_emotions_content_wrapper{display:none}
.single_post .post_comments .comments_emotions .comments_emotions_content{background:#fbfbfb;border:1px solid #eee;border-radius:5px;margin-top:20px;padding:15px}
.single_post .post_comments .comments_emotions .comments_emotions_content .emoji_note{margin-bottom:10px;font-weight:300;font-size:14px;text-align:center}
.single_post .post_comments .comments_emotions .comments_emotions_content span{width:32px;height:32px;display:inline-block}
.single_post .post_comments .comments_emotions .comments_emotions_content input{font-family:Segoe UI Emoji;font-size:20px;font-weight:300;display:block;border:0;background:transparent;text-align:center;width:32px;height:32px}
.single_post .post_comments .post_comments_locked{line-height:20px;text-transform:uppercase;font-weight:700}
.single_post .post_comments.not_threaded iframe#comment-editor,.single_post .post_comments.not_threaded .post_comments_locked,.single_post .post_comments.not_threaded .post_comments_content .post_comments_message{margin-top:0!important}
.single_post .post_comments.not_threaded .post_comments_content .post_comments_message{margin-bottom:20px!important}
.single_post .post_comments.not_threaded .post_comments_content .post_comments_form{display:block!important}

/* error
------------------------------- */
.error .error_content h2{font-size:40px;text-transform:uppercase;color:#f95959}
.error .error_content h2 span:nth-child(2){color:$(keycolor)}
.error .error_content h2 span:last-child{font-size:18px;color:#aaa}
.error .error_search form{max-width:350px;margin:0 auto}
.error .post_related{margin-bottom:0;padding-bottom:0}
.error .post_related .uk-dotnav{display:none}
.error .featured_error{text-align:center}

/* footer
------------------------------- */
:not(blockquote)>footer{background-color:$(footer.bg.color.1);background-image: -webkit-gradient(linear,left top,right top,from($(footer.bg.color.1)),to($(footer.bg.color.2)));background-image:linear-gradient(to right,$(footer.bg.color.1),$(footer.bg.color.2));position:relative;padding-top:70px;padding-bottom:40px;color:#fff;z-index:2}
:not(blockquote)>footer .uk-h1,:not(blockquote)>footer .uk-h2,:not(blockquote)>footer .uk-h3,:not(blockquote)>footer .uk-h4,:not(blockquote)>footer .uk-h5,:not(blockquote)>footer .uk-h6,:not(blockquote)>footer h1,:not(blockquote)>footer h2,:not(blockquote)>footer h3,:not(blockquote)>footer h4,:not(blockquote)>footer h5,:not(blockquote)>footer h6{color:#fff}
:not(blockquote)>footer a,:not(blockquote)>footer a:focus{color:#ccc!important}
:not(blockquote)>footer a:hover{color:#f1f1f1!important;text-decoration:underline}
:not(blockquote)>footer .widget_title{font-size:20px}
:not(blockquote)>footer .widget_title:before{border-color:#000}

/* .topgrid */
.topgrid_section > .widget{margin-bottom:20px;padding-bottom:20px}
.topgrid_section > .widget:last-child{margin-bottom:0;padding-bottom:0}

/* .maingrid */
.copyrights{font-size:14px;text-transform:uppercase}
.social_social a{color:#fff!important}
.social_social a:hover{color:#aaa!important}

/* gadgets style
------------------------------- */

/* .Attribution */
.Attribution{text-align:center}
.Attribution div{line-height:24px}
.Attribution div svg{fill:#fff;vertical-align:bottom;cursor:pointer;height:24px;width:24px;min-width:24px}

/* .Wikipedia */
.wikipedia-search-results-header{padding:0 0 5px;margin-bottom:10px;height:inherit;border-bottom:1px solid #444}
.wikipedia-search-results div{padding:5px 0}
.wikipedia-search-results div:first-child{padding-top:0}
.Wikipedia br,.Wikipedia nobr div,.wikipedia-search-results-header{display:none}

/* .ContactForm */
.ContactForm .uk-button{position:relative}
.ContactForm .uk-button input{background:transparent;border:0;border-radius:100px;cursor:pointer;top:0;right:0;bottom:0;left:0;width:100%;height:100%;opacity:0;position:absolute;padding:0;margin:0;line-height:0;font-size:0}
.ContactForm p{margin:0;overflow:hidden}
.ContactForm .contact-form-message-box{text-align:center;max-width:100%;width:100%}
.ContactForm p.contact-form-error-message-with-border,.ContactForm p.contact-form-success-message-with-border{line-height:20px;padding:5px 12px;border:0;border-radius:2px;background-color:#dedede;display:block;color:rgba(0,0,0,.87);position:relative;margin-top:14px;font-size:12px;font-weight:300}
.ContactForm p.contact-form-error-message-with-border{padding-left:42px}
.contact-form-error-message-with-border:before,.contact-form-error-message-with-border img{content:'';height:22px;width:23px;line-height:22px;position:absolute;top:4px;left:5px;z-index:1;background:#777;border-radius:100%}
.contact-form-error-message-with-border img{opacity:0;cursor:pointer;z-index:10}
.contact-form-error-message-with-border:after{content:'+';height:22px;line-height:22px;width:22px;position:absolute;top:5px;left:5px;z-index:2;color:#dedede;font-size:26px;text-align:center;-webkit-transform:rotate(-45deg);-ms-transform:rotate(-45deg);-o-transform:rotate(-45deg);transform:rotate(-45deg)}
.ContactForm p.contact-form-success-message-with-border{background:#83B641;color:#fff;border-radius:100px}

/* .Translate */
.Translate .goog-te-gadget{white-space:inherit}
footer .Translate .goog-te-gadget,footer .Translate .goog-te-gadget a{color:#fff !important}

/* .Subscribe + .Feed */
.Subscribe{color:#333;font-size:14px;position:static}
.Subscribe .subscribe-wrapper{margin:0;margin-top:0.5em;padding:0;position:relative;zoom:1}
.Subscribe .subscribe-wrapper:first-child{margin-top:0}
.Subscribe div.subscribe{width:100%}
.Subscribe div.subscribe div.bottom{display:none}
.Subscribe div.subscribe{cursor:pointer;margin:0;padding:0;text-align:right}
.Subscribe div.subscribe div.top{background:#fff;border:1px solid #eee;padding:6px 8px;border-radius:3px}
.Subscribe .subscribe-dropdown-arrow{float:left;margin-left:6px;margin-top:4px}
.Subscribe .feed-icon{display:inline-block;vertical-align:top;margin-top:6px;margin-left:4px}
.Subscribe .subscribe-wrapper .expanded{position:absolute;top:0;z-index:20}
.Subscribe a.feed-reader-link{display:block;font-weight:normal;margin:.5em .5em .5em 0;text-decoration:none;z-index:1000;color:#333}

/* .BloggerButton */
.BloggerButton img{width:auto}

/* .Stats */
.Stats .counter-wrapper{display:inline-block;font-size:24px;font-weight:bold;height:30px;line-height:30px;vertical-align:top;direction:ltr}
.Stats img{margin-left:10px;vertical-align:top}
.Stats .graph-counter-wrapper{color:#eee}
.Stats .digit{background:url("https://www.blogger.com/img/widgets/stats-flipper.png") no-repeat right!important;border:1px solid #444;display:inline-block;height:28px;line-height:28px;margin-right:-1px;position:relative;text-align:center;width:22px}
.Stats .blind-plate{border-bottom:1px solid #fff;border-top:1px solid #000;filter:alpha(opacity=65);height:0;right:0;opacity:.65;position:absolute;top:13px;width:22px}
.Stats .stage-0{background-position:0 0!important}
.Stats .stage-1{background-position:-22px 0!important}
.Stats .stage-2{background-position:-44px 0!important}
.Stats .stage-3{background-position:-66px 0!important}

/* .PopularPosts */
.PopularPosts ul,.PopularPosts li{margin:0;padding:0;list-style:none}
.PopularPosts ul li{display:inline-block;line-height:1.6;margin-bottom:15px;width:100%}
.PopularPosts ul li:last-child{border-bottom:0;margin-bottom:0;padding-bottom:0}
.PopularPosts ul li:before{display:none}
.PopularPosts ul > li > a,.PopularPosts ul > li > .item-title > a{position:relative;padding-right:22px}
.PopularPosts .item-thumbnail{float:right;padding:0;margin:0;margin-left:10px;margin-bottom:5px}
.PopularPosts .item-thumbnail a{border-radius:500px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.15);box-shadow:0 5px 10px rgba(0,0,0,0.15)}
.PopularPosts .item-thumbnail a,.PopularPosts .item-thumbnail a img{color:#fff;display:block;height:72px;width:72px;padding:0}
.PopularPosts .item-title{font-weight:400}
.PopularPosts .item-title a:hover{text-decoration:none}
.PopularPosts .item-snippet{font-size:13px;font-weight:300;color:rgba(255,255,255,.6)}

/* .BlogArchive */
.BlogArchive a:hover{text-decoration:none}
.BlogArchive ul:not(.flat),.BlogArchive ul:not(.flat) li{margin:0;padding:0;list-style:none}
.BlogArchive #ArchiveList .collapsed > ul{display:none}
.BlogArchive #ArchiveList .expanded > ul{display:block}
.BlogArchive #ArchiveList ul ul.hierarchy li,.BlogArchive #ArchiveList ul.posts li{padding-right:1.3em}
.BlogArchive #ArchiveList ul{margin-top:12px}
.BlogArchive #ArchiveList > div > ul{margin-top:0}
.BlogArchive select{width:100%}

/* .Profile */
.Profile .profile-img{float:right;margin-left:10px;margin-bottom:5px;height:72px;width:72px;border-radius:500px;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.15);box-shadow:0 5px 10px rgba(0,0,0,0.15)}
.Profile .profile-data .profile-link{margin-bottom:10px;background-repeat:no-repeat;background-position:right center;display:inline-block;}
.Profile .profile-info > .profile-link{font-size:90%}
.Profile .profile-datablock{margin-bottom:10px}
.Profile .profile-textblock{font-size:90%;line-height:1.6;margin-top:15px}
.Profile ul,.Profile li{margin:0;padding:0;list-style:none}
.Profile ul{display:table;width:100%}
.Profile li{float:right;margin-bottom:15px;padding-bottom:15px;border-bottom:1px solid #eee;width:100%}
.Profile li:last-child{margin-bottom:0;padding-bottom:0;border-bottom:0}
.Profile li .profile-link{background:none!important;line-height:35px}
.Profile li .profile-img{width:35px;height:35px;margin-bottom:0;border-radius:4px}

/* .FeaturedPost */
.FeaturedPost ul,.FeaturedPost li{list-style:none;margin:0;padding:0}
.FeaturedPost .item-content{margin-bottom:-10px}
.FeaturedPost .item-thumbnail{margin-bottom:15px}
.FeaturedPost .item-thumbnail a{color:#fff}
.FeaturedPost .item-thumbnail img{border-radius:2px;width:100%;-webkit-box-shadow:0 5px 10px rgba(0,0,0,0.15);box-shadow:0 5px 10px rgba(0,0,0,0.15)}
.FeaturedPost .item-title,.FeaturedPost .item-snippet{margin-bottom:10px}
.FeaturedPost .item-snippet{font-size:95%}

/* .Image */
.Image img{height:auto}
.Image .caption {margin-top:10px;display:inline-block}

/* totop */
[uk-totop].hide,[data-uk-totop].hide{left:-100px!important}

/* social icons */
[class*="icon_"]{color:#fff!important;transition-property: color,background-color,box-shadow,opacity}
[class*="icon_"]:hover{opacity:.8}
.icon_500px{background:#0099e5!important}
.icon_behance{background:#1769ff!important}
.icon_dribbble{background:#ea4c89!important}
.icon_facebook{background:#3b5998!important}
.icon_flickr{background:#ff0084!important}
.icon_foursquare{background:#0732a2!important}
.icon_github,.icon_github-alt{background:#333!important}
.icon_gitter{background:#46bc99!important}
.icon_google{background:#4285f4!important}
.icon_google-plus{background:#dd4b39!important}
.icon_instagram{background:#f77737!important}
.icon_joomla{background:#f44321!important}
.icon_linkedin{background:#0077b5!important}
.icon_pagekit{background:#212121!important}
.icon_pinterest{background:#bd081c!important}
.icon_reddit{background:#ff4500!important}
.icon_soundcloud{background:#ff3300!important}
.icon_tripadvisor{background:#00af87!important}
.icon_tumblr{background:#35465c!important}
.icon_twitter{background:#1da1f2!important}
.icon_uikit{background:#1e87f0!important}
.icon_vimeo{background:#1ab7ea!important}
.icon_whatsapp{background:#25d366!important}
.icon_wordpress{background:#21759b!important}
.icon_xing{background:#026466!important}
.icon_yelp{background:#af0606!important}
.icon_youtube{background:#ff0000!important}
.icon_rss{background:#f26522!important}
.icon_mail{background:#444!important}

/* sideanv + .sidebar
------------------------------- */
.sidenav .section .widget,.sidebar .widget{border-bottom:1px solid rgba(255,255,255,.1);margin-bottom:30px;padding-bottom:30px}
.sidenav .section .widget:last-child,.sidebar .widget:last-child{border-bottom:0;margin-bottom:0;padding-bottom:0}
.sidenav .section .widget .widget_title,.sidebar .widget .widget_title{font-size:18px}
.sidenav .section .widget .widget_title:before,.sidebar .widget .widget_title:before{border-right-color:$(keycolor)}

/* .sidebar
------------------------------- */
.sidebar .widget,.light .sidenav .section .widget{border-bottom:1px solid rgba(0,0,0,.1)}
.sidebar .PopularPosts .item-snippet{color:inherit}

/* .light
------------------------------- */
.light header .mainnav_menu .uk-navbar-nav > li > a{color:$(body.link.color)!important;font-weight:500!important}
.light header .mainnav_menu .uk-navbar-nav > li.current > a,.light header .mainnav_menu .uk-navbar-nav > li > a:hover{color:$(keycolor)!important}
.light header .mainnav_menu .uk-navbar-nav > li > a:before{background:$(keycolor)}
.light.no_waves :not(blockquote)>footer{-webkit-box-shadow:0 5px 15px rgba(0,0,0,.08);box-shadow:0 5px 15px rgba(0,0,0,.08)}
.light :not(blockquote)>footer,.light :not(blockquote)>footer .uk-h1,.light :not(blockquote)>footer .uk-h2,.light :not(blockquote)>footer .uk-h3,.light :not(blockquote)>footer .uk-h4,.light :not(blockquote)>footer .uk-h5,.light :not(blockquote)>footer .uk-h6,.light :not(blockquote)>footer h1,.light :not(blockquote)>footer h2,.light :not(blockquote)>footer h3,.light :not(blockquote)>footer h4,.light :not(blockquote)>footer h5,.light :not(blockquote)>footer h6{color:#444}
.light :not(blockquote)>footer .widget_title:before{border-color:$(keycolor)}
.light :not(blockquote)>footer a,.light :not(blockquote)>footer a:focus{color:$(body.link.color)!important}
.light :not(blockquote)>footer a:hover{color:$(body.link.hover.color)!important}
.light .social_social a{color:$(keycolor)}
.light .sidemenu .sidemenu_list :not(.post_thumbnail):not(.post_title) > a{color:$(keycolor)}
.light .sidemenu .sidemenu_list > li ul,.light .sidemenu .sidemenu_list li .mega,.light .sidemenu .sidemenu_list li .featured_error{background:#e8e8e8}
.light .sidemenu .sidemenu_list > li ul ul,.light .sidemenu .sidemenu_list li.has_multi_mega .mega,.light .sidemenu .sidemenu_list li.has_multi_mega .featured_error{background:#d8d8d8}
.light .sidemenu .sidemenu_list :not(.post_thumbnail):not(.post_title) > a > span{color:#222}
.light .sidemenu .sidemenu_list :not(.post_thumbnail):not(.post_title) > a:hover > span{color:#fff}
.light .sidemenu .sidemenu_list li .featured_error{color:#ff0000}
.light .uk-close{color:#333}
.light .uk-close:focus,.uk-close:hover{color:#fff}

/* responsive
------------------------------- */
@media (max-width:1199px) and (min-width:992px){
.mainnav .Header .header-image-wrapper img{height:50px}
.mainnav_wrapper.uk-sticky-fixed .mainnav .Header .header-image-wrapper img{height:40px}
.filtering_labels .mark{padding:0 20px}
}
@media (min-width:992px){
.breadcrumb{margin-bottom:20px}
}
@media (max-width:991px){
.topnav{padding-bottom:50px!important}
.Header{display:flex;align-items:center}
.Header .haeder-menu a,header .Header .haeder-menu a:hover{color:#fff}
.mainnav_menu>*>*:not(:last-child){display:none}
.filtering_labels .uk-grid .uk-icon{line-height:40px}
.topgrid_section > .widget:last-child{margin-bottom:20px;padding-bottom:20px}
.sidebar{margin-top:80px}
.light header .haeder-menu a{color:$(body.link.color)!important}
.light header .haeder-menu a:hover{color:$(body.link.hover.color)!important}
}
@media (max-width:991px) and (min-width:768px){
header{padding-top:40px}
main .main_content{margin-top:40px}
.filtering_labels{margin-bottom:40px!important}
.filtering_labels .select_view{margin-bottom:0!important}
.filtering_labels .uk-grid select{min-width:150px;max-width:250px}
}
@media (max-width:767px){
header{padding-top:15px}
.topnav{border-bottom:1px solid rgba(255,255,255,.08);padding-bottom:15px!important;margin-bottom:40px!important}
.topnav .sidenav_button a{background:transparent;color:#fff;box-shadow:0 0 0 transparent;height:25px;line-height:25px;border:0;padding:0}
.topnav .sidenav_button a span:not(.uk-icon){display:none}
.topnav .topnav_social{align-items:center;justify-content:center}
.topnav .topnav_social li a{height:25px;width:25px;line-height:25px;background:transparent!important;box-shadow:0 0 0 transparent}
.sidemenu .sidemenu_list li.has_mega .blog_posts{padding:30px 15px}
main .main_content{margin-top:25px}
.filtering_labels{margin-bottom:0!important}
.filtering_labels .select_label,.filtering_labels .select_view,.breadcrumb{margin-bottom:25px}
.filtering_labels .uk-grid select{width:100%}
.full_header{padding:40px 0}
.maingrid{text-align:center}
.maingrid .copyrights{margin-bottom:30px}
.maingrid .social .social_social{align-content:center;justify-content:center}
.single_post .post_author_profile .post_author_profile_name{margin-bottom:20px!important}
.single_post .post_author_profile .post_author_profile_name img{width:30px;height:30px}
.single_post .post_comments .post_comments_content li .comment-block{padding-right:0}
.single_post .post_comments .post_comments_content .comment-thread ol ol li{margin-right:0}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header,.single_post .post_comments .post_comments_content li .avatar-image-container .comment-actions{float:right;position:relative;top:0;right:0;-webkit-transform:none;transform:none}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-header{margin-right:20px;display:block}
.single_post .post_comments .post_comments_content li .avatar-image-container .comment-actions{width:100%;margin-top:20px;text-align:left}
.error .error_content h2 span:first-child{display:block;width:100%}
.error .error_content h2 span:nth-child(2){margin-right:0!important}
.light header .topnav .sidenav_button a,.light .topnav .topnav_social li a{color:$(body.link.color)!important}
.light header .topnav .sidenav_button a:hover,.light .topnav .topnav_social li a:hover{color:$(body.link.hover.color)!important}
.light header .topnav{border-bottom:1px solid rgba(0,0,0,.08)}
}
@media (max-width:575px){
header{padding-bottom:15px}
.topnav{margin-bottom:15px!important}
.error .error_content h2 span:first-child{font-size:28px}
}
body {font-family: 'Tajawal';}

]]></b:skin>

    <b:template-skin>
      <![CDATA[
html{direction:ltr}
body#layout{background:#f9f9f9;border:3px dashed #444;border-radius:4px;display:table;margin-bottom:30px;font-family:Roboto,sans-serif;padding:0;position:relative;width:1000px}
body#layout div.section{background:transparent;border:0;margin:0;padding:16px 24px}
body#layout div.section h4,body#layout div.section .add_widget .add-icon,body#layout .top_bg,body#layout .bottom_bg{display:none}
body#layout div.section .add_widget{border:0;margin:0;padding:0}
body#layout div.section .add_widget a{border:3px dashed #007bff;border-radius:500px;margin:0;padding:0 16px;text-align:center;height:50px;line-height:44px;color:#007bff;position:relative}
body#layout div.section .add_widget a:hover{background:#007bff}
body#layout div.section .add_widget a:before{content:'';background-color:transparent;background-image:url('https://1.bp.blogspot.com/-Nc1YdQOh96M/XG8LoBwtCWI/AAAAAAAAGk4/3NJ28m_joS4xQs5kVnPBqY4McgiTK_fNwCLcBGAs/s1600/add_24dp.png');background-repeat:no-repeat;background-position:center;width:24px;height:24px;top:0;left:100%;display:inline-block;vertical-align:middle;margin-right:10px}
body#layout div.section .add_widget a:hover:before{background-image:url('https://2.bp.blogspot.com/-4M9za3ZqdkQ/XG8NN2b2yEI/AAAAAAAAGlE/djfAoi6Fnl00oug6YbZjQsULIHawL0Q4QCLcBGAs/s1600/add_white_24dp.png')}
body#layout div.section .add_widget a:hover{color:#fff;text-decoration:none}
body#layout div.section .widget-content{border-radius:500px;padding:10px 20px;background:#fff}
body#layout div.section .layout-widget-state{position:absolute;top:50%;left:20px;margin-top:-12px}
body#layout div.section .editlink.icon{position:absolute;top:50%;right:20px;margin-top:-12px}
body#layout div.section .Blog .widget-content{border-radius:5px}
body#layout div.section .Blog .layout-widget-state{position:relative;top:auto;left:auto;margin-top:0}
body#layout div.section .Blog .editlink.icon{right:16px;top:16px;margin-top:0}
body#layout div.section .draggable-widget .widget-wrap3,body#layout div.section .draggable-widget .widget-wrap2{background:none;margin-left:0}
body#layout div.section .draggable-widget{margin-left:12px;position:relative}
body#layout div.section .draggable-widget{z-index:1}
body#layout div.section .draggable-widget:before{background-image:url(https://3.bp.blogspot.com/-VoGWwIOGJ0Y/XG-MsA3165I/AAAAAAAAGlQ/XLtqyEgMSiY967d1Silkp8zZ2C94LgtmgCLcBGAs/s1600/draggable.png);background-color:#bbb;background-repeat:no-repeat;background-position:center;border-radius:500px;content:'';position:absolute;width:12px;top:0;left:-12px;bottom:0;z-index:2}
body#layout div.section div.widget,body#layout div.section > div{margin-top:18px}
body#layout div.section .dr_active{border:3px dashed #666;background:transparent;border-radius:500px}
body#layout div.section div.widget.el_active{margin-top:0}
body#layout .hidden{display:inherit!important}
body#layout .uk-container{width:auto}
body#layout .wrapper{position:relative;width:100%;z-index:1}
body#layout header{background-color:#ae1e51;background-image:url(https://1.bp.blogspot.com/-RN5eSQCeFJc/W0vBLeGmEBI/AAAAAAAAGM0/2556CYyDPlgkPbcrx66L-3y05hOium01QCK4BGAYYCw/s1600/logo_1x.png);background-repeat:no-repeat;background-position:24px 15px;border-left:3px dashed #444;padding:85px 0 50px;margin-bottom:0;margin-left:317px}
body#layout header:before,body#layout main:before,body#layout footer:before,body#layout .sidenav:before{content:"Header Content";font-size:18px;display:block;padding:20px 24px 0;color:#fff}
body#layout header .topnav_wrapper div.section > div{margin-top:0}
body#layout header div.section{padding:20px 24px}
body#layout header .mainnav_wrapper div.section .dropregion{display:none}
body#layout header .mainnav_wrapper .mainnav{display:table;table-layout:fixed;padding:0 24px;width:100%}
body#layout header .mainnav_wrapper .mainnav > div{display:table-cell;width:50%;padding:0 12px}
body#layout header .mainnav_wrapper .mainnav > div.Header{padding-left:0}
body#layout header .mainnav_wrapper .mainnav > div.HTML{padding-right:0}
body#layout main{padding:20px 0 30px;margin-left:317px;border-left:3px dashed #444;border-top:3px dashed #444}
body#layout main:before{content:"Main Content";color:inherit;padding-bottom:20px}
body#layout main .uk-container,body#layout main .uk-container .uk-grid,body#layout .topgrid,body#layout .maingrid{display:table;table-layout:fixed;width:100%}
body#layout main .uk-container > div,body#layout main .uk-container .uk-grid > div,body#layout .maingrid > div{display:table-cell;width:50%}
body#layout main .uk-container > div.main:before,body#layout main .uk-container .uk-grid > div > div.main:before{content:'Blog & Labels Filter Gadgets';font-size:15px}
body#layout main .uk-container > div.sidebar:before,body#layout main .uk-container .uk-grid > div.sidebar:before{content:'Sidebar Gadgets';margin-bottom:18px;display:block;font-size:15px}
body#layout footer{padding:20px 0 20px;border-top:3px dashed #444}
body#layout footer:before{content:"Footer Content";color:inherit;padding-bottom:20px}
body#layout .topgrid{margin:0 -12px;padding:0 24px;width:auto}
body#layout .topgrid > div{display:table-cell;width:25%;padding:16px 12px}
body#layout .sidenav{position:absolute;padding:85px 0 20px;left:0;top:0;z-index:2;width:320px}
body#layout .sidenav:before{content:"Side Gadgets";color:inherit;padding:20px 24px}
      ]]>
    </b:template-skin>

    <b:defaultmarkups>
      <b:defaultmarkup type='Common'>
        <b:includable id='widget-title'>
          <b:if cond='data:widget.sectionId not in {&quot;topnav&quot;,&quot;mainnav&quot;,&quot;main&quot;,&quot;copyrights&quot;,&quot;social&quot;}'>
            <b:if cond='data:title != &quot;&quot;'>
              <h3 class='widget_title uk-heading-bullet'><span><b:eval expr='data:defaultTitle ?: data:title'/></span></h3>
            </b:if>
          </b:if>
        </b:includable>
        <b:includable id='adverts-code'>
          <div expr:style='&quot;background:#f9f9f9;border:1px dashed #e5e5e5;line-height:&quot; + data:height + &quot;;text-align:center;width:100%;height:&quot; + data:height + &quot;;max-width:100%;margin:0 auto;font-size:14px;text-transform:uppercase;&quot;'><data:messages.adsGoHere/></div>
        </b:includable>
        <b:includable id='background-svg'>
          <svg viewBox='0 9 100 6' width='100%' xmlns='http://www.w3.org/2000/svg'>
            <linearGradient expr:id='data:id'>
              <stop class='g_fill_1' offset='0%' stop-color='currentcolor'/>
              <stop class='g_fill_2' offset='100%' stop-color='currentcolor'/>
            </linearGradient>
            <path d='M0 0 V12 Q30 17 55 12 T100 11 V0z' expr:fill='&quot;url(#&quot; + data:id + &quot;)&quot;'/>
            <b:if expr:cond='data:isHeader'>
              <clipPath id='clip-path'><path d='M0 0 V12 Q30 17 55 12 T100 11 V0z'/></clipPath>
              <path clip-path='url(#clip-path)' d='M0 30 V15 Q30 3 60 15 V30z' fill='#fff' opacity='0.5'/>
            </b:if>
          </svg>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='LinkList'>
        <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;topnav&quot;'>
            <div class='uk-grid' data-uk-grid=''>
              <div class='sidenav_button uk-width-auto uk-margin-remove'>
                <a class='uk-button' data-uk-toggle='target:#sidenav' href='#!'>
                  <b:class expr:name='data:theme.layout.enableLightStyle ? &quot;uk-button-primary&quot; : &quot;uk-button-default&quot;'/>
                  <span data-uk-icon='thumbnails'/>
                  <span class='uk-margin-small-right'><data:theme.text.sideMenu/></span>
                </a>
              </div>
              <div class='topnav_social_wrapper uk-width-expand uk-margin-remove'>
                <div class='uk-align-left uk-margin-remove'>
                  <ul class='topnav_social uk-iconnav'>
                    <b:loop index='i' values='data:links' var='link'>
                      <li><a data-uk-tooltip='pos:bottom' expr:class='&quot;uk-icon-button icon_&quot; + data:link.name' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
                    </b:loop>
                  </ul>
                </div>
              </div>
            </div>
          </b:if>
          <b:if cond='data:widget.sectionId == &quot;social&quot;'>
            <ul class='social_social uk-iconnav'>
              <b:loop index='i' values='data:links' var='link'>
                  <li><a data-uk-tooltip='pos:top' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
              </b:loop>
            </ul>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;social&quot;,&quot;topnav&quot;}'>
            <div class='widget-content'>
              <b:class cond='!data:theme.layout.enableLightStyle and data:widget.sectionId in {&quot;footer_section_1&quot;,&quot;footer_section_2&quot;,&quot;footer_section_3&quot;,&quot;footer_section_4&quot;}' name='uk-light'/>
              <ul class='uk-list uk-list-bullet uk-margin-remove'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:href='data:link.target'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:if>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='Header'>
        <b:includable id='main' var='this'>
          <b:class name='uk-margin-remove uk-width-auto'/>
          <div class='haeder-menu uk-margin-left uk-hidden@l' data-uk-tooltip='pos:bottom' expr:title='data:theme.text.menu'>
            <a class='icon_menu' data-uk-icon='icon:menu;ratio:1.2' data-uk-toggle='target:#sidemenu' href='#!'/>
          </div>
          <div class='header-widget'>
            <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
            <b:include cond='data:imagePlacement not in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='title'/>
          </div>
          <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='behindImageStyle'/>
        </b:includable>
        <b:includable id='image'>
          <b:if cond='!data:view.isSingleItem'>
            <h1 class='clip'>
              <a expr:href='data:blog.homepageUrl' expr:title='data:title'><span><data:title/></span></a>
            </h1>
          </b:if>
          <a class='header-image-wrapper' expr:href='data:blog.homepageUrl'>
            <b:include data='{ image: data:image, altText: data:blog.title.escaped }' name='responsiveImage'/>
          </a>
        </b:includable>
        <b:includable id='responsiveImage'>
          <img expr:alt='data:altText ?: data:messages.image' expr:src='data:image'/>
        </b:includable>
        <b:includable id='behindImageStyle'>
          <b:if cond='data:sourceUrl and data:imagePlacement == &quot;BEHIND&quot;'>
            <b:include cond='data:this.image' data='{ image: data:this.image, selector: &quot;.header-widget&quot; }' name='responsiveImageStyle'/>
          </b:if>
        </b:includable>
        <b:includable id='title'>
          <h1><b:tag expr:href='data:blog.homepageUrl' name='a'><data:title/></b:tag></h1>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='HTML'>
        <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='Blog'>
        <b:includable id='main' var='this'>
          <div expr:class='data:view.isMultipleItems ? &quot;blog_posts&quot; : &quot;single_post&quot;' expr:id='data:view.isMultipleItems ? &quot;blog_posts&quot; : &quot;single_post&quot;'>
            <b:class name='hfeed'/>
            <b:class cond='data:view.isMultipleItems and !data:enableSidebar' name='uk-child-width-1-1 uk-child-width-1-2@m uk-child-width-1-3@l'/>
            <b:class cond='data:view.isMultipleItems and data:enableSidebar' name='uk-child-width-1-1 uk-child-width-1-2@m uk-child-width-1-2@l'/>
            <b:attr cond='data:view.isMultipleItems' name='data-uk-grid' value='masonry:true'/>
            <b:with value='3' var='maxNumAds'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include data='post' expr:name='data:view.isMultipleItems ? &quot;postGridsAndAd&quot; : &quot;postCommentsAndAd&quot;'/>
                <b:include cond='data:view.isMultipleItems' data='post' name='inlineAdGrid'/>
              </b:loop>
              <b:if cond='data:posts.length == 0'>
                <div class='uk-width'>
                  <div class='no_results'>
                    <span class='uk-margin-left' data-uk-icon='warning'/><data:messages.noResultsFound/>
                  </div>
                </div>
              </b:if>
            </b:with>
          </div>
          <b:include name='nextPageLink'/>
        </b:includable>
        <b:includable id='postGridsAndAd' var='post'>
          <article class='post hentry'>
            <b:attr expr:value='data:post.id' name='data-id'/>
            <script>
              var filterTags_<data:post.id/> = Object.values({<b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
            </script>
            <b:include data='post' name='postMeta'/>
            <div class='uk-card uk-card-hover uk-card-default'>
              <b:include name='postThumbnail'/>
              <div class='post_content uk-card-small uk-card-body'>
                <b:include data='post' name='postLabels'/>
                <b:include data='post' name='postTitle'/>
                <b:include data='post' name='postSnippet'/>
                <b:include data='post' name='postMetaInfo'/>
              </div>
            </div>
          </article>
        </b:includable>
        <b:includable id='postCommentsAndAd' var='post'>
          <article class='post hentry'>
            <b:include data='post' name='postMeta'/>
            <div class='post_content'>
              <b:include data='post' name='postTitle'/>
              <b:include data='post' name='postHeader'/>
              <b:include data='post' name='postAlignment'/>
              <b:include data='post' name='postBody'/>
              <b:include data='post' name='inlineAdPost'/>
              <b:include data='post' name='postRelated'/>
              <b:include data='post' name='postFooter'/>
            </div>
            <b:include data='post' name='commentPicker'/>
          </article>
        </b:includable>
        <b:includable id='inlineAdGrid' var='post'>
          <b:if cond='data:post.includeAd'>
            <b:if cond='not data:maxNumAds or data:post.adNumber lt data:maxNumAds'>
              <div class='post inline_ad'>
                <div class='uk-card uk-card-hover uk-card-default'>
                  <em><data:messages.adsGoHere/></em>
                  <div class='post_content uk-card-small uk-card-body'>
                    <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
                      <data:this.adCode/>
                      <b:else/>
                      <b:include data='{height: &quot;250px&quot;}' name='adverts-code'/>
                    </b:if>
                  </div>
                </div>
              </div>
            </b:if>
          </b:if>
        </b:includable>
        <b:includable id='inlineAdPost' var='post'>
          <b:if cond='data:post.includeAd'>
            <b:if cond='not data:maxNumAds or data:post.adNumber lt data:maxNumAds'>
              <div class='inline_ad'>
                <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
                  <data:this.adCode/>
                  <b:else/>
                  <b:include data='{height: &quot;90px&quot;}' name='adverts-code'/>
                </b:if>
              </div>
            </b:if>
          </b:if>
        </b:includable>
        <b:includable id='postTitle' var='post'>
          <b:if cond='data:post.title != &quot;&quot;'>
            <b:if cond='data:view.isMultipleItems'>
              <h2 class='post_title entry-title uk-margin'>
                <b:if cond='data:post.link or (data:post.url and data:view.url != data:post.url)'>
                  <a expr:href='data:post.link ?: data:post.url' rel='bookmark'><data:post.title/></a>
                  <b:else/>
                  <data:post.title/>
                </b:if>
              </h2>
              <b:else/>
              <h1 class='post_title entry-title uk-article-title'><data:post.title/></h1>
            </b:if>
          </b:if>
        </b:includable>
        <b:includable id='postLabels'>
          <b:if cond='data:post.labels'>
            <b:if cond='data:view.isMultipleItems'>
              <div class='post_labels uk-panel uk-margin-small'>
                <b:attr name='b:whitespace' value='remove'/>
                <span class='uk-margin-small-left' data-uk-icon='icon:tag;ratio:.7'/>
                <b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                  <b:if cond='data:i &lt; 2'>
                    <b:if cond='data:i &gt; 0'><span class='uk-margin-xsmall-left'>, </span></b:if>
                    <a expr:href='data:label.url' rel='tag'>#<data:label.name/></a>
                  </b:if>
                </b:loop>
              </div>
              <b:else/>
              <span class='post_labels uk-margin-left uk-margin-small-bottom'>
                <b:attr name='b:whitespace' value='remove'/>
                <span class='post_labels_label'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
                  <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:tag;ratio:.75'/><data:byline.label/>
                </span>
                <b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                  <b:if cond='data:i &gt; 0'><span class='uk-margin-xsmall-left'>, </span></b:if>
                  <a expr:href='data:label.url' rel='tag'>#<data:label.name/></a>
                </b:loop>
              </span>
            </b:if>
          </b:if>
        </b:includable>
        <b:includable id='postThumbnail'>
          <b:if cond='data:post.featuredImage'>
            <div class='post_thumbnail uk-card-media-top uk-text-center uk-position-relative uk-transition-toggle' expr:data-title='data:post.title'>
              <a expr:href='data:post.url'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <b:include data='{ image: data:post.featuredImage, imageSizes: [480], imageRatio: &quot;16:9&quot;, sourceSizes: &quot;480px&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                  <b:else/>
                  <b:if cond='data:theme.layout.enableImagesAutoHeight'>
                    <b:include data='{ image: data:post.featuredImage, imageSizes: [345,285,330,510], sourceSizes: &quot;(min-width: 1200px) 345px, (min-width: 992px) 285px, (min-width: 768px) 330px, (min-width: 576px) 510px, calc(100vw - 30px)&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                    <b:else/>
                    <b:include data='{ image: data:post.featuredImage, imageSizes: [345,285,330,510], imageRatio: &quot;16:9&quot;, sourceSizes: &quot;(min-width: 1200px) 345px, (min-width: 992px) 285px, (min-width: 768px) 330px, (min-width: 576px) 510px, calc(100vw - 30px)&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                  </b:if>
                </b:if>
                <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
                <div class='uk-position-center'>
                  <b:if cond='data:post.featuredImage.isYoutube'>
                    <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:2.3'/>
                    <b:else/>
                    <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:2.3'/>
                  </b:if>
                </div>
              </a>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='postHeader' var='post'>
          <div class='post_header uk-article-meta uk-margin-bottom'>
            <div class='post_header_line'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:loop index='i' values='data:widgets.Blog.first.headerByline' var='region'>
                <b:if cond='data:region.items.any'>
                  <b:include data='region.items' name='bylineRegion'/>
                </b:if>
              </b:loop>
            </div>
          </div>
        </b:includable>
        <b:includable id='postBody' var='post'>
          <div class='post_body entry-content' expr:id='&quot;post_body_&quot; + data:post.id'>
            <b:class cond='data:view.isSingleItem' name='uk-margin-large-bottom'/>
            <data:post.body/>
          </div>
        </b:includable>
        <b:includable id='postFooter' var='post'>
          <div class='post_footer uk-article-meta'>
            <b:loop index='i' values='data:widgets.Blog.first.footerBylines' var='region'>
              <b:if cond='data:region.items.any'>
                <div class='post_footer_line'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <b:class expr:name='&quot;post_footer_line_&quot; + (data:i + 1)'/>
                  <b:include data='region.items' name='bylineRegion'/>
                </div>
              </b:if>
            </b:loop>
            <b:include cond='!data:view.isPage' data='post' name='postFooterAuthorProfile'/>
          </div>
        </b:includable>
        <b:includable id='postRelated' var='post'>
          <b:if cond='data:theme.relatedPosts.enable and data:view.isPost'>
            <div class='post_related uk-text-center' expr:data-count='data:theme.relatedPosts.maxResults' expr:data-id='data:post.id' expr:data-title='data:theme.relatedPosts.title'>
              <div data-uk-spinner=''/>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='postAuthor'>
          <span class='post_author vcard uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_author_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:user;ratio:.75'/><data:byline.label/>
            </span>
            <span class='fn'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:if cond='data:post.author.profileUrl'>
                <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <span><data:post.author.name/></span>
                </a>
                <b:else/>
                <span><data:post.author.name/></span>
              </b:if>
            </span>
          </span>
        </b:includable>
        <b:includable id='postTimestamp'>
          <span class='post_timestamp uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_timestamp_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:clock;ratio:.75'/><data:byline.label/>
            </span>
            <b:if cond='data:post.url'>
              <meta expr:content='data:post.url.canonical'/>
              <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'>
                <b:attr name='b:whitespace' value='remove'/>
                <time class='published' expr:datetime='data:post.date.iso8601' expr:title='data:post.date.iso8601'><data:post.date/></time>
              </a>
            </b:if>
          </span>
        </b:includable>
        <b:includable id='postLocation'>
          <span class='post_location uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_location_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:location;ratio:.75'/><data:byline.label/>
            </span>
            <a expr:href='data:post.location.mapsUrl' target='_blank'><data:post.location.name/></a>
          </span>
        </b:includable>
        <b:includable id='postReactions'>
          <span class='post_reactions uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_reactions_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:happy;ratio:.75'/><data:byline.label/>
            </span>
            <iframe allowtransparency='true' class='reactions-iframe' expr:src='data:post.reactionsUrl' frameborder='0' name='reactions' scrolling='no'/>
          </span>
        </b:includable>
        <b:includable id='postCommentsLink'>
          <span class='post_comment_link uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_comment_link_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:comment;ratio:.75'/><data:byline.label/>
            </span>
            <a class='comment-link' expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
              <b:if cond='data:post.numberOfComments gt 0'>
                <b:message name='messages.numberOfComments'><b:param expr:value='data:post.numberOfComments' name='numComments'/></b:message>
                <b:else/>
                <data:messages.postAComment/>
              </b:if>
            </a>
          </span>
        </b:includable>
        <b:includable id='postFooterAuthorProfile' var='post'>
          <b:if cond='data:post.author.aboutMe'>
            <div class='post_author_profile uk-margin-top'>
              <div class='uk-grid uk-grid-medium'>
                <b:if cond='data:post.author.authorPhoto.image'>
                  <div class='uk-width-auto uk-visible@m'>
                    <div class='post_author_profile_photo'>
                      <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                        <img alt='author photo' expr:src='data:post.author.authorPhoto.image'/>
                      </a>
                    </div>
                  </div>
                </b:if>
                <div class='uk-width-expand'>
                  <div class='post_author_profile_name uk-flex uk-flex-middle uk-margin-small-bottom uk-text-uppercase'>
                    <b:if cond='data:post.author.authorPhoto.image'>
                      <a class='g-profile uk-margin-left uk-hidden@m' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                        <img alt='author photo' expr:src='data:post.author.authorPhoto.image'/>
                      </a>
                    </b:if>
                    <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                      <span><data:post.author.name/></span>
                    </a>
                  </div>
                  <div class='post_author_profile_desc'>
                    <span><data:post.author.aboutMe/></span>
                  </div>
                </div>
              </div>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='postSnippet' var='post'>
          <div class='post_snippet entry-summary uk-position-relative'>
            <p expr:id='&quot;body&quot; + data:post.id'>
              <textarea><b:eval expr='data:post.body snippet { length: 150, links: false, linebreaks: false, ellipsis: false }'/></textarea>
              <script class='js'>var postId = &quot;<data:post.id/>&quot;, postLink = &quot;<data:post.url/>&quot;,readMore = &quot;<data:messages.readMore/>&quot;;/*<![CDATA[*/eval(function(n,e,r,t,i,o){if(i=function(n){return n.toString(27)},!$salA[5][$salA[4]](/^/,String)){for(;r--;)o[i(r)]=t[r]||i(r);t=[function(n){return o[n]}],i=function(){return $salA[6]},r=1}for(;r--;)t[r]&&(n=n[$salA[4]](new RegExp($salA[7]+i(r)+$salA[7],$salA[8]),t[r]));return n}($salA[0],0,27,$salA[3][$salA[2]]($salA[1]),0,{}));//]]></script>
            </p>
            <b:include cond='data:post.shareUrl' data='post' name='postShareButtons'/>
          </div>
        </b:includable>
        <b:includable id='postMetaInfo' var='post'>
          <div class='post_meta uk-grid uk-grid-small'>
            <div class='post_date uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='icon: clock; ratio: .7'/><span><time class='published' expr:datetime='data:post.date.iso8601' expr:title='data:post.date.iso8601'><data:post.date/></time></span></div>
            <b:if cond='data:post.numberOfComments &gt; 0'>
              <div class='post_comments uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='icon: comment; ratio: .7'/><span><data:post.numberOfComments/></span></div>
            </b:if>
            <b:if cond='data:post.shareUrl'>
              <div class='post_share uk-width-auto'>
                <span class='action'><span class='uk-margin-small-left' data-uk-icon='icon: social; ratio: .7'/><span><data:messages.share/></span></span>
              </div>
            </b:if>
          </div>
        </b:includable>
        <b:includable id='postShareButtons'>
          <b:tag class='post_share uk-margin-left uk-margin-small-bottom' cond='data:view.isSingleItem' name='div'>
            <b:attr cond='data:view.isSingleItem' name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isSingleItem'>
              <span class='post_share_label'>
                <b:attr name='b:whitespace' value='remove'/>
                <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
                <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:social;ratio:.75'/><data:messages.share/>
              </span>
            </b:if>
            <ul class='post_share_buttons uk-iconnav uk-text-center'>
              <b:class cond='data:view.isMultipleItems' name='uk-iconnav uk-position-center uk-animation-toggle'/>
              <b:loop values='data:blog.sharing.platforms' var='platform'>
                <b:if cond='data:platform.key not in {&quot;link&quot;,&quot;blogThis&quot;,&quot;googlePlus&quot;,&quot;email&quot;}'>
                  <li><span data-uk-tooltip='pos:top' expr:class='&quot;icon_&quot; + data:platform.key + &quot; uk-icon-button&quot;' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:data-uk-icon='data:platform.key' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
                <b:if cond='data:platform.key == &quot;googlePlus&quot;'>
                  <li><span class='icon_google-plus uk-icon-button' data-uk-icon='google-plus' data-uk-tooltip='pos:top' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
                <b:if cond='data:post.emailPostUrl and data:platform.key == &quot;email&quot;'>
                  <li><span class='icon_reddit uk-icon-button' data-uk-icon='reddit' data-uk-tooltip='pos:top' expr:data-href='appendParams(&quot;https://www.reddit.com/submit&quot;, { url: data:post.url, title: data:post.title } )' expr:title='data:theme.text.shareTo + &quot; Reddit&quot;' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                  <li><span class='icon_mail uk-icon-button' data-uk-icon='mail' data-uk-tooltip='pos:top' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
              </b:loop>
            </ul>
          </b:tag>
        </b:includable>
        <b:includable id='postAlignment' var='post'>
          <b:if cond='data:view.isPost'>
            <script class='js'>var labelsName = &quot;<b:loop values='data:post.labels' var='label'><data:label.name/> </b:loop>&quot;.trim().split(&quot; &quot;),postImage = &quot;<b:eval expr='resizeImage(data:post.featuredImage,1600,&quot;16:9&quot;)'/>&quot;;/*<![CDATA[*/eval(function(e,n,t,a,r,i){if(r=function(e){return(e<51?$salB[4]:r(parseInt(e/51)))+(35<(e%=51)?String[$salB[5]](e+29):e.toString(36))},!$salB[4][$salB[6]](/^/,String)){for(;t--;)i[r(t)]=a[t]||r(t);a=[function(e){return i[e]}],r=function(){return $salB[7]},t=1}for(;t--;)a[t]&&(e=e[$salB[6]](new RegExp($salB[8]+r(t)+$salB[8],$salB[9]),a[t]));return e}($salB[0],0,51,$salB[3][$salB[2]]($salB[1]),0,{}));//]]></script>
          </b:if>
        </b:includable>
        <b:includable id='nextPageLink'>
          <b:if cond='data:view.isMultipleItems and data:olderPageUrl'>
            <div class='blog_pager uk-text-center uk-margin-large-top' id='blog_pager'>
              <a class='blog-pager-older-link uk-button uk-button-default' data-uk-icon='more' expr:href='data:olderPageUrl' expr:title='data:messages.morePosts'>
                <span class='uk-margin-small-left'><data:messages.morePosts/></span>
              </a>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='commentPicker' var='post'>
          <b:if cond='data:post.allowComments'>
            <div class='post_comments uk-margin-medium-top' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
              <b:if cond='data:post.commentSource != 1'>
                <b:class cond='data:post.showThreadedComments' name='threaded'/>
                <b:class cond='!data:post.showThreadedComments' name='not_threaded'/>
              </b:if>
              <b:include name='commentsTitle'/>
              <div class='post_comments_content'>
                <b:if cond='data:post.commentSource == 1'>
                  <b:include data='post' name='iframeComments'/>
                  <b:elseif cond='data:post.showThreadedComments'/>
                  <b:include data='post' name='threadedComments'/>
                  <b:else/>
                  <b:include data='post' name='comments'/>
                </b:if>
              </div>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='commentsTitle'>
          <h3 class='post_comments_title'><span class='uk-margin-left' data-uk-icon='comments'/><data:messages.comments/></h3>
        </b:includable>
        <b:includable id='commentForm' var='post'>
          <div class='post_comments_form'>
            <b:if cond='data:this.messages.blogComment != &quot;&quot;'>
              <div class='post_comments_message'><span class='uk-margin-small-left' data-uk-icon='info'/><data:this.messages.blogComment/></div>
            </b:if>
            <b:include data='post' name='commentFormIframeSrc'/>
            <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight ?: &quot;90px&quot;' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
            <div class='comments_emotions' id='comments_emotions'/>
            <data:post.cmtfpIframe/>
            <script>BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);</script>
          </div>
        </b:includable>
        <b:includable id='commentItem' var='comment'>
          <li class='comment' expr:id='&quot;c&quot; + data:comment.id'>
            <div class='avatar-image-container'>
              <b:if cond='data:blog.enabledCommentProfileImages'>
                <img alt='author-avatar' expr:src='resizeImage(data:comment.authorAvatarSrc,80,&quot;1:1&quot;)'/>
              </b:if>
              <div class='comment-header'>
                <cite class='user blog-author'>
                  <b:if cond='data:comment.authorUrl'>
                    <a expr:href='data:comment.authorUrl' rel='nofollow'><data:comment.author/></a>
                    <b:else/>
                    <span><data:comment.author/></span>
                  </b:if>
                </cite>
                <span class='datetime secondary-text'>
                  <a expr:href='data:comment.url' rel='nofollow'><data:comment.timestamp/></a>
                </span>
              </div>
              <span class='comment-actions secondary-text'>
                <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
                  <b:if cond='data:showCmtPopup'>
                    <div class='goog-toggle-button'>
                      <div class='goog-inline-block comment-action-icon'/>
                    </div>
                    <b:else/>
                    <a expr:href='data:comment.deleteUrl' target='_self'>
                      <span class='uk-margin-small-left' data-uk-icon='trash'/><data:messages.deleteComment/></a>
                  </b:if>
                </span>
              </span>
            </div>
            <div class='comment-block'>
              <div expr:class='&quot;comment-body&quot; + (data:comment.isDeleted ? &quot; deleted-comment&quot; : &quot;&quot;)'>
                <data:comment.body/>
              </div>
            </div>
          </li>
        </b:includable>
        <b:includable id='threadedCommentJs' var='post'>
          <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>
          <b:template-script inline='true' name='threaded_comments'/>
          <script type='text/javascript'>
            blogger.widgets.blog.initThreadedComments(
              <data:post.commentJso/>,
              <data:post.commentMsgs/>,
              <data:post.commentConfig/>);
          </script>
        </b:includable>
        <b:includable id='threadedComments' var='post'>
          <b:class cond='!data:post.allowNewComments' name='comments_locked'/>
          <b:include cond='data:post.embedCommentForm' data='post' name='threadedCommentJs'/>
          <div class='post_comments_holder' id='comment-holder'>
            <data:post.commentHtml/>
            <script class='js'>/*<![CDATA[*/eval(function(e,n,r,t,a,i){if(a=function(e){return(e<43?$salC[4]:a(parseInt(e/43)))+(35<(e%=43)?String[$salC[5]](e+29):e.toString(36))},!$salC[4][$salC[6]](/^/,String)){for(;r--;)i[a(r)]=t[r]||a(r);t=[function(e){return i[e]}],a=function(){return $salC[7]},r=1}for(;r--;)t[r]&&(e=e[$salC[6]](new RegExp($salC[8]+a(r)+$salC[8],$salC[9]),t[r]));return e}($salC[0],0,43,$salC[3][$salC[2]]($salC[1]),0,{}));//]]></script>
          </div>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
            <b:else/>
            <div class='post_comments_locked uk-margin-top uk-text-danger'>
              <span class='uk-margin-small-left' data-uk-icon='ban'/><span><data:post.noNewCommentsText/></span>
            </div>
          </b:if>
          <b:if cond='data:showCmtPopup'>
            <div id='comment-popup'>
              <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'/>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='comments' var='post'>
          <b:class cond='!data:post.allowNewComments' name='comments_locked'/>
          <b:if cond='data:post.comments'>
            <div class='post_comments_holder' expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
              <b:include cond='data:post.comments' data='post.comments' name='commentList'/>
              <ol id='comments-block'>
                <b:loop values='data:post.comments' var='comment'>
                  <b:include data='comment' name='commentItem'/>
                </b:loop>
              </ol>
            </div>
          </b:if>
          <b:if cond='data:post.embedCommentForm'>
            <b:if cond='data:post.allowNewComments'>
              <b:include data='post' name='commentForm'/>
              <b:else/>
              <div class='post_comments_locked uk-margin-top uk-text-danger'>
                <span class='uk-margin-small-left' data-uk-icon='ban'/><span><data:post.noNewCommentsText/></span>
              </div>
            </b:if>
            <b:else/>
            <b:if cond='data:post.allowComments'>
              <div class='add_comments uk-margin-top'>
                <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
                  <span class='uk-margin-small-left' data-uk-icon='commenting'/><b:message name='messages.postAComment'/>
                </a>
              </div>
            </b:if>
          </b:if>
          <b:if cond='data:showCmtPopup'>
            <div id='comment-popup'>
              <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'/>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='post'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='postPagination'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='previousPageLink'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='headerByline'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='footerBylines'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='emailPostIcon'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='aboutPostAuthor'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='commentsLink'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='threadedCommentForm'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='addComments'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='commentList'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='commentAuthorAvatar'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='commentDeleteIcon'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='feedLinks'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='feedLinksBody'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='postJumpLink'><b:comment>Removed</b:comment></b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='Label'>
        <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;main&quot;'>
            <b:include name='filter'/>
            <b:else/>
            <div class='widget-content'>
              <b:class expr:name='data:this.display + &quot;-label-widget-content&quot;'/>
              <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
              <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
            </div>
          </b:if>
        </b:includable>
        <b:includable id='filter'>
          <div class='filtering_labels uk-grid uk-margin-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isHomepage'>
              <div class='select_label uk-width-expand@m'>
                <b:if cond='data:theme.layout.enableFilterOption'>
                  <script class='js'>
                    var filterTags = Object.values({<b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
                  </script>
                  <ul class='uk-list uk-list-inline uk-visible@l'>
                    <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='settings'/><span><data:theme.text.filter/></span></span></li>
                    <li><a class='uk-button uk-button-default uk-margin-bottom uk-active' data-uk-filter-control='' href='#!'><data:messages.viewAll/></a></li>
                    <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                      <li><a class='uk-button uk-button-default uk-margin-bottom' expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' href='#!'><data:label.name/></a></li>
                    </b:loop>
                  </ul>
                  <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                    <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='settings'/></div>
                    <div class='uk-width-auto@m uk-width-expand'>
                      <select class='uk-select'>
                        <option data-uk-filter-control='' value=''><data:messages.viewAll/></option>
                        <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                          <option expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' expr:value='&quot;.filter_&quot; + data:i'><data:label.name/></option>
                        </b:loop>
                      </select>
                    </div>
                  </div>
                </b:if>
              </div>
            </b:if>
            <b:if cond='data:view.isMultipleItems and !data:view.isHomepage'>
              <div class='breadcrumb uk-width-expand@m'>
                <ul class='uk-breadcrumb'>
                  <li><a href='/'><data:messages.home/></a></li>
                  <b:if cond='data:view.isSearch'>
                    <li><a href='/search'><data:messages.search/></a></li>
                    <b:if cond='data:view.isLabelSearch'>
                      <li class='uk-disabled'><span><data:messages.labels/></span></li>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                      <b:elseif cond='data:view.search.query'/>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                    </b:if>
                  </b:if>
                  <b:if cond='data:view.isArchive'>
                    <li class='uk-disabled'><span><data:messages.archive/></span></li>
                    <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                  </b:if>
                </ul>
              </div>
            </b:if>
            <b:if cond='data:theme.layout.enableViewOption'>
              <div class='select_view uk-width-exapnd uk-width-auto@m'>
                <b:class cond='!data:theme.layout.enableFilterOption' name='uk-margin-bottom'/>
                <ul class='uk-list uk-list-inline uk-visible@l'>
                  <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='cog'/><span><data:theme.text.view/></span></span></li>
                  <li class='uk-active'><a class='uk-icon-button' data-uk-icon='expand' data-uk-tooltip='pos:top' expr:title='data:theme.text.expandPosts' href='#!' id='view_e'/></li>
                  <li><a class='uk-icon-button' data-uk-icon='shrink' data-uk-tooltip='pos:top' expr:title='data:theme.text.shrinkPosts' href='#!' id='view_s'/></li>
                </ul>
                <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                  <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='cog'/></div>
                  <div class='uk-width-auto@m uk-width-expand'>
                    <select class='uk-select'>
                      <option value='expand'><data:theme.text.expandPosts/></option>
                      <option value='shrink'><data:theme.text.shrinkPosts/></option>
                    </select>
                  </div>
                </div>
                <script class='js'>/*<![CDATA[*/eval(function(e,c,r,t,d,i){if(d=function(e){return e.toString(16)},!$salD[5][$salD[4]](/^/,String)){for(;r--;)i[d(r)]=t[r]||d(r);t=[function(e){return i[e]}],d=function(){return $salD[6]},r=1}for(;r--;)t[r]&&(e=e[$salD[4]](new RegExp($salD[7]+d(r)+$salD[7],$salD[8]),t[r]));return e}($salD[0],0,16,$salD[3][$salD[2]]($salD[1]),0,{}));//]]></script>
              </div>
            </b:if>
          </div>
        </b:includable>
        <b:includable id='cloud'>
          <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
            <a class='label-name uk-button uk-button-default uk-button-small uk-margin-small-left uk-margin-small-bottom' expr:href='data:label.url'>
              <b:class expr:name='&quot;label-size-&quot; + data:label.cssSize'/>
              <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-margin-small-right'>_<data:label.count/></span></b:if>
            </a>
          </b:loop>
        </b:includable>
        <b:includable id='list'>
          <ul class='uk-list uk-list-bullet uk-margin-remove'>
            <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
              <li>
                <a class='label-name' expr:href='data:label.url'>
                  <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-align-left uk-margin-remove'><data:label.count/></span></b:if>
                </a>
              </li>
            </b:loop>
          </ul>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='ReportAbuse'>
        <b:includable id='reportAbuse'>
          <h3 class='title uk-margin-remove'>
            <b:attr name='b:whitespace' value='remove'/>
            <a class='report_abuse uk-button uk-button-danger uk-width-1-1' href='https://www.blogger.com/go/report-abuse' rel='noopener nofollow' target='_blank'>
              <span class='uk-margin-small-left' data-uk-icon='warning'/>
              <span><data:messages.reportAbuse/></span>
            </a>
          </h3>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='Wikipedia'>
        <b:includable id='content'>
          <div class='wikipedia-search-main-container'>
            <form class='wikipedia-search-form' expr:id='data:widget.instanceId + &quot;_wikipedia-search-form&quot;' name='wikipedia'>
              <div class='uk-width-1-1 uk-inline uk-margin-small-bottom'>
                <button class='wikipedia-search-button uk-form-icon uk-form-icon-flip uk-icon' data-uk-icon='search' type='submit'/>
                <input class='wikipedia-search-input uk-input' expr:id='data:widget.instanceId + &quot;_wikipedia-search-input&quot;' placeholder='Search Wikipedia...' type='text'/>
              </div>
            </form>
            <div class='wikipedia-search-results-header' expr:id='data:widget.instanceId + &quot;_wikipedia-search-results-header&quot;'><data:searchResultsMsg/></div>
            <div class='wikipedia-search-results' expr:id='data:widget.instanceId + &quot;_wikipedia-search-results&quot;'/>
            <nobr><div expr:dir='data:blog.languageDirection' expr:id='data:widget.instanceId + &quot;_wikipedia-search-more&quot;'/></nobr>
          </div><br/>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='ContactForm'>
        <b:includable id='content'>
          <div class='contact-form-widget'>
            <div class='form'>
              <form name='contact-form'>
                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <span class='uk-form-icon uk-form-icon-flip' data-uk-icon='user'/>
                    <input class='contact-form-name uk-input' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' type='text' value=''/>
                  </div>
                </div>
                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <span class='uk-form-icon uk-form-icon-flip' data-uk-icon='mail'/>
                    <input class='contact-form-email uk-input' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg + &quot; *&quot;' name='email' type='text' value=''/>
                  </div>
                </div>

                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <textarea class='contact-form-email-message uk-textarea' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg + &quot; *&quot;' name='email-message' rows='5'/>
                  </div>
                </div>
                <div class='uk-button uk-button-danger uk-width-1-1'>
                  <span><data:contactFormSendMsg/></span><span class='uk-margin-small-right uk-icon' data-uk-icon='forward'/><input class='class=&quot;contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' value=''/>
                </div>
                <div class='contact-form-message-box'>
                  <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
                  <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
                </div>
              </form>
            </div>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='TextList'>
        <b:includable id='content'>
          <div class='widget-content'>
            <ul class='uk-list uk-list-bullet uk-margin-remove'>
              <b:loop values='data:items' var='item'>
                <li><data:item/></li>
              </b:loop>
            </ul>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='FeaturedPost,PopularPosts'>
        <b:includable id='snippetedPosts'>
          <ul>
            <b:loop values='data:posts' var='post'>
              <li>
                <b:include name='snippetedPostContent'/>
              </li>
            </b:loop>
          </ul>
        </b:includable>
        <b:includable id='postSnippet'>
          <div class='item-snippet'><b:eval expr='data:post.snippets.short snippet { length: 80, links: false, linebreaks: false, ellipsis: true }'/></div>
        </b:includable>
        <b:includable id='snippetedPostTitle'>
          <div class='item-title'>
            <a expr:href='data:post.url'><data:post.title/></a>
          </div>
        </b:includable>
        <b:includable id='snippetedPostContent'>
          <div class='item-content'>
            <b:include cond='data:postDisplay.showFeaturedImage and data:post.featuredImage' name='snippetedPostThumbnail'/>
            <b:include cond='data:widget.type == &quot;FeaturedPost&quot; ? data:postDisplay.showTitle : true' name='snippetedPostTitle'/>
            <b:include cond='data:postDisplay.showSnippet' name='postSnippet'/>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='PopularPosts'>
        <b:includable id='snippetedPostThumbnail'>
          <b:class name='uk-transition-toggle'/>
          <div class='item-thumbnail uk-text-center'>
            <a class='uk-position-relative uk-overflow-hidden' expr:href='data:post.url'>
              <img alt='Image' expr:src='resizeImage(data:post.featuredImage,72,&quot;1:1&quot;)'/>
              <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
              <div class='uk-position-center'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:1.5'/>
                  <b:else/>
                  <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:1.5'/>
                </b:if>
              </div>
            </a>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='FeaturedPost'>
        <b:includable id='snippetedPostThumbnail'>
          <div class='item-thumbnail uk-text-center uk-position-relative uk-transition-toggle'>
            <a expr:href='data:post.url'>
              <img alt='Image' expr:src='resizeImage(data:post.featuredImage,360,&quot;16:9&quot;)'/>
              <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
              <div class='uk-position-center'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:2.3'/>
                  <b:else/>
                  <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:2.3'/>
                </b:if>
              </div>
            </a>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='PageList'>
        <b:includable id='pageList'>
          <ul class='uk-list uk-list-bullet uk-margin-remove'>
            <b:class cond='data:pageListClass' expr:name='data:pageListClass'/>
            <b:loop values='data:links' var='link'>
              <b:include name='pageLink'/>
            </b:loop>
          </ul>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='BlogArchive'>
        <b:includable id='main'>
          <b:include name='widget-title'/>
          <div class='widget-content'>
            <div id='ArchiveList'>
              <div expr:id='data:widget.instanceId + &quot;_ArchiveList&quot;'>
                <b:include cond='data:style == &quot;HIERARCHY&quot;' data='data' name='interval'/>
                <b:include cond='data:style == &quot;FLAT&quot;' data='data' name='flat'/>
                <b:include cond='data:style == &quot;MENU&quot;' data='data' name='menu'/>
              </div>
            </div>
          </div>
        </b:includable>
        <b:includable id='flat' var='data'>
          <ul class='flat uk-list uk-list-bullet uk-margin-remove'>
            <b:loop values='data:data' var='i'>
              <li class='archivedate'>
                <a expr:href='data:i.url'><data:i.name/></a> (<data:i.post-count/>)
              </li>
            </b:loop>
          </ul>
        </b:includable>
        <b:includable id='interval' var='intervalData'>
          <b:loop values='data:intervalData' var='interval'>
            <ul class='hierarchy'>
              <li expr:class='&quot;archivedate &quot; + data:interval.expclass'>
                <b:include cond='data:interval.toggleId' data='interval' name='toggle'/>
                <a class='post-count-link' expr:href='data:interval.url'>
                  <data:interval.name/>
                </a>
                <span class='post-count' dir='ltr'>(<data:interval.post-count/>)</span>
                <b:include cond='data:interval.data' data='interval.data' name='interval'/>
                <b:include cond='data:interval.posts' data='interval.posts' name='posts'/>
              </li>
            </ul>
          </b:loop>
        </b:includable>
        <b:includable id='menu' var='data'>
          <select class='uk-select' expr:id='data:widget.instanceId + &quot;_ArchiveMenu&quot;'>
            <option value=''><data:title/></option>
            <b:loop values='data:data' var='i'>
              <option expr:value='data:i.url'><data:i.name/> (<data:i.post-count/>)</option>
            </b:loop>
          </select>
        </b:includable>
        <b:includable id='posts' var='posts'>
          <ul class='posts'>
            <b:loop values='data:posts' var='post'>
              <li><a expr:href='data:post.url'><data:post.title/></a></li>
            </b:loop>
          </ul>
        </b:includable>
        <b:includable id='toggle' var='interval'>
          <a class='toggle' href='javascript:void(0)'>
            <span expr:class='&quot;zippy&quot; + (data:interval.expclass == &quot;expanded&quot; ? &quot; toggle-open&quot; : &quot;&quot;)'>
              <b:if cond='data:interval.expclass == &quot;expanded&quot;'>
                &#9660;&#160;
                <b:elseif cond='data:blog.languageDirection == &quot;rtl&quot;'/>
                &#9668;&#160;
                <b:else/>
                &#9658;&#160;
              </b:if>
            </span>
          </a>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='BlogSearch'>
        <b:includable id='searchSubmit'><b:comment>Removed</b:comment></b:includable>
        <b:includable id='searchForm'>
          <form expr:action='data:blog.searchUrl'>
            <b:attr cond='not data:view.isPreview' name='target' value='_top'/>
            <b:include name='urlParamsAsFormInput'/>
            <div class='search-input uk-width-1-1 uk-inline'>
              <button class='search-action uk-form-icon uk-form-icon-flip' data-uk-icon='search' type='submit'/>
              <input autocomplete='off' class='uk-input' expr:aria-label='data:messages.searchThisBlog' expr:placeholder='data:messages.searchThisBlog' expr:value='data:view.isSearch ? data:view.search.query.escaped : &quot;&quot;' name='q' type='text'/>
            </div>
          </form>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='FollowByEmail'>
        <b:includable id='content'>
          <div class='widget-content'>
            <div class='follow-by-email-inner'>
              <form action='https://feedburner.google.com/fb/a/mailverify' expr:onsubmit='&quot;window.open(\&quot;https://feedburner.google.com/fb/a/mailverify?uri=&quot; + data:feedPath + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' target='popupwindow'>
                <div class='uk-grid uk-grid-small uk-margin-bottom'>
                  <span class='uk-width-auto' data-uk-icon='icon:mail;ratio:2'/>
                  <span class='uk-width-expand'><data:theme.text.followByEmailMessage/></span>
                </div>
                <div class='search-input uk-width-1-1 uk-inline'>
                  <button class='search-action uk-form-icon uk-form-icon-flip' data-uk-icon='forward' type='submit'/>
                  <input autocomplete='off' class='follow-by-email-address uk-input' expr:placeholder='data:messages.emailAddress' name='email' type='email'/>
                </div>
                <input expr:value='data:feedPath' name='uri' type='hidden'/>
                <input name='loc' type='hidden' value='en_US'/>
              </form>
            </div>
          </div>
        </b:includable>
      </b:defaultmarkup>
      <b:defaultmarkup type='Image'>
        <b:includable id='content'>
          <div class='widget-content'>
            <b:tag cond='data:link' expr:href='data:link' name='a'>
              <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl' expr:width='data:width'/>
            </b:tag>
            <br/>
            <b:if cond='data:caption'>
              <span class='caption'><data:caption/></span>
            </b:if>
          </div>
        </b:includable>
      </b:defaultmarkup>
    </b:defaultmarkups>

    <style>.no_matching_results:before{content:&quot;<data:messages.noResultsFound/>&quot;}</style>

    <b:if cond='data:widgets.AdSense.first or data:blog.adsenseClientId'>
      <script async='async' src='//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js'/>
    </b:if>
    <b:include data='blog' name='google-analytics'/>
  </head>

  <body>
    <b:class cond='data:view.isPreview' name='preview'/>
    <b:class cond='data:view.isHomepage' name='homepage_view'/>
    <b:class cond='data:view.isArchive' name='archive_view'/>
    <b:class cond='data:view.isLabelSearch' name='label_view'/>
    <b:class cond='data:view.isSearch and !data:view.isLabelSearch' name='search_view'/>
    <b:class cond='data:view.isPost' name='post_view'/>
    <b:class cond='data:view.isPage' name='page_view'/>
    <b:class cond='data:view.isMultipleItems' name='multiple_view'/>
    <b:class cond='data:view.isSingleItem' name='single_view'/>
    <b:class cond='data:view.isError' name='error_view'/>

    <b:comment>Theme Options</b:comment>
    <b:with value='{ text: { sideMenu: &quot;القائمة الجانبية&quot;, menu: &quot;القائمة&quot;, followOn: &quot;تابعنا على&quot;, shareTo: &quot;شارك على&quot;, filter: &quot;التصنيف&quot;, view: &quot;العرض&quot;, expandPosts: &quot;عرض كامل&quot;, shrinkPosts: &quot;عرض مصغر&quot;, followByEmailMessage: &quot;إحصل على التحديثات مباشرة في بريدك. إشترك لكي يتم تنبيهك بكل المستجدات&quot;, backToTop: &quot;العودة لأعلى&quot;, emotions: &quot;الوجوه التعبيرية&quot;, emotionsInfo: &quot;إنسخ ثم إلصق الوجوه التعبيرية في صندوق التعليقات&quot;, monthsNames: &quot;يناير فبراير مارس أبريل مايو يونيو يوليو أغسطس سبتمبر أكتوبر نوفمبر ديسمبر&quot; }, layout: { enableLightStyle: false, enableWavyStyle: true, enableStickyHeader: true, enableStickySidebar: true, enableIndexSidebar: false, enablePagesSidebar: true, enableFilterOption: true, enableViewOption: true, enableShrinkedPosts: false, enableShrinkingForAll: false, enableImagesAutoHeight: false, enableInfiniteScroll: true }, relatedPosts: { enable: true, title: &quot;مواضيع ذات صلة&quot;, maxResults: &quot;5&quot; }, errorPage: { header1st: &quot;الصفحة غير موجودة&quot;, header2nd: &quot;خطأ 404 - عفوا&quot;, message: &quot;ربما تم إزالة الصفحة أو تم إعادة تسميتها أو غير متاحة مؤقتا. إبحث مجددا&quot;, enableFeaturedPosts: true, featuredPostsMaxResults: &quot;6&quot; } }' var='theme'>

      <b:class expr:cond='data:theme.layout.enableLightStyle' name='light'/>
      <b:class cond='!data:theme.layout.enableWavyStyle' name='no_waves'/>

      <script class='js'>const textSearch=&quot;<data:messages.search/>&quot;,textBackToTop=&quot;<data:theme.text.backToTop/>&quot;,textEmotions=&quot;<data:theme.text.emotions/>&quot;,textEmotionsInfo=&quot;<data:theme.text.emotionsInfo/>&quot;,monthsNames=&quot;<data:theme.text.monthsNames/>&quot;,enableLightStyle=<data:theme.layout.enableLightStyle/>,enableStickySidebar=<data:theme.layout.enableStickySidebar/>,enableShrinkedPosts=<data:theme.layout.enableShrinkedPosts/>,enableShrinkingForAll=<data:theme.layout.enableShrinkingForAll/>,enableInfiniteScroll=<data:theme.layout.enableInfiniteScroll/>,/*<![CDATA[! js-cookie v2.2.0 | MIT */defaultThumb="//3.bp.blogspot.com/-p4FTeqsJBK8/XDe3J33UAWI/AAAAAAAAGYg/CLdsnYg0fYkwGPLxDWvtEXx_1wjuaipkgCLcBGAs/s72-c/default_thumb.png",$salA=['!4(){7 e,n,2,3=$8("#9"+b)[0];3&&(3.c=(e=3.d("f")[0].g,n=h,(2=e.i("<")).j(4(e,n){-1!=2[n].5(">")&&(2[n]=2[n].6(2[n].5(">")+1,2[n].k))}),(2=(2=2.l("")).6(0,n-1)).m()+\'... <a o="\'+p+\'">\'+q+"</a>"))}();',"|","split","||t|r|function|indexOf|substring|var|get|body||postId|innerHTML|querySelectorAll||textarea|value|150|split|forEach|length|join|trim||href|postLink|readMore","replace","","\\w+","\\b","g"],$salB=['!y(){8(-1<9.a("z"))$2("#6")[0].k.m+=" 5-A-B@l";C 8(-1<9.a("D")){(t=4.b("n")).3(4.c(".E{F:G}")),$2("d")[0].3(t),$2("#6")[0].k.o="5-H-1-1"}8(-1<9.a("I")){J e=4.b("f"),t=4.b("n");e.o="7",e.K="<f L=\'5-g\'></f>",h!=$2(".i")[0]?(t.3(4.c(".p{q-r:s("+u+")}")),$2("d")[0].3(t),e.v[0].3($2(".w")[0]),e.v[0].3($2(".x")[0]),$2(".i")[0].m.M("p"),$2(".i")[0].3(e)):(t.3(4.c(".7{q-r:s("+u+")}")),$2("d")[0].3(t),$2("6")[0].j(e,$2("6")[0].N[0]),$2(".7 .5-g")[0].j($2(".w")[0],h),$2(".7 .5-g")[0].j($2(".x")[0],h))}}();',"|","split","||get|appendChild|document|uk|main|full_header|if|labelsName|indexOf|createElement|createTextNode|head||div|container|null|top_bg|insertBefore|parentElement||classList|style|className|has_full_header|background|image|url||postImage|children|post_title|post_header|function|right_side|flex|last|else|no_side|sidebar|display|none|width|full_title|var|innerHTML|class|add|childNodes","","fromCharCode","replace","\\w+","\\b","g"],$salC=['$k(".l .x y.8").m(o(e){z n=[e.5(".p-q-r")[0],e.5(".p-q-r A")[0],e.5(".8-b > a")[0],e.5(".8-b > 4 a")[0]];n[0]&&(n[0].t(e.5(".8-B")[0]),n[0].t(e.5(".8-b")[0])),n[1]&&(n[1].u=n[1].u.v(/\\/s[0-9]+(-*c*)\\//,"/w-c/").v(/\\=s[0-9]+/,"=w")),n[2]&&(n[2].6="<4 d=\'7-f-g-h\' i-7-j=\'C\'></4>"+n[2].6),n[3]&&(n[3].6="<4 d=\'7-f-g-h\' i-7-j=\'D\'></4>"+n[3].6)}),$k(".E .l .F a").m(o(e,n){e.6="<4 d=\'7-f-g-h\' i-7-j=\'G\'></4>"+e.6});',"|","split","||||span|querySelectorAll|innerHTML|uk|comment|||actions||class||margin|small|left|data|icon|get|post_comments|forEach||function|avatar|image|container||appendChild|src|replace|s45|post_comments_holder|li|var|img|header|reply|trash|single_post|continue|commenting","","fromCharCode","replace","\\w+","\\b","g"],$salD=['"2"==7.1("8")&&($1("#9")[0].3.4.a("5-6"),$1("#b")[0].3.4.c("5-6"),$1(".d e")[0].f="2");',"|","split","|get|shrink|parentNode|classList|uk|active|Cookies|grid_view|view_e|remove|view_s|add|select_view|select|value","replace","","\\w+","\\b","g"],$salE=['6 5=f(){6 a=7.g(\'h\');a.i=\'j-k-1\';a.l(\'m\',\'n/o\');a.8(7.p((q?\'\':\'#r \')+\'.s + .t{u:v}\'));$4(\'w\')[0].8(a)};x&&"9"!=2.4("3")?(5(),2.b("3","c",{d:e})):y==2.4("3")?2.b("3","9",{d:e}):"c"==2.4("3")&&5();',"|","split","||Cookies|grid_view|get|shrinkPosts|var|document|appendChild|expand||set|shrink|expires|99999|function|createElement|style|id|view|skin|setAttribute|type|text|css|createTextNode|enableShrinkingForAll|blog_posts|post_thumbnail|post_content|display|none|head|enableShrinkedPosts|null","replace","","\\w+","\\b","g"],$salF=['p 1y={1z:L(e){o("2"9 e){p t=q A;o("j"9 e.2&&(t.B=e.2.j.$t,t.B=t.B.b(t.B.f("1A-")+5),t.B=t.B.C(".D","")),"G"9 e.2&&(t.1B=e.2.G.$t),"18"9 e.2&&(t.1C=e.2.18.$t),t.a=q A,"g"9 e.2)x(p n=0;n<e.2.g.u;n++)"19"==e.2.g[n].M&&(t.1D=e.2.g[n].H),"l"==e.2.g[n].M&&(t.a.l=e.2.g[n].H,-1<t.a.l.f("/N/")?t.a.l="/O"+t.a.l.b(t.a.l.f("/N/")):-1<t.a.l.f("/D/")&&(t.a.l="/O"+t.a.l.b(t.a.l.f("/D/")))),"m"==e.2.g[n].M&&(t.a.m=e.2.g[n].H,-1<t.a.m.f("/N/")?t.a.m="/O"+t.a.m.b(t.a.m.f("/N/")):-1<t.a.m.f("/D/")&&(t.a.m="/O"+t.a.m.b(t.a.m.f("/D/"))));o("E$T"9 e.2&&(t.a.T=e.2.E$T.$t),"E$U"9 e.2&&(t.a.U=e.2.E$U.$t),"E$V"9 e.2&&(t.a.V=e.2.E$V.$t),"3"9 e.2){t.1a=q 1b;x(n=0;n<e.2.3.u;n++){p d=q A;o("j"9 e.2.3[n]&&(d.j=e.2.3[n].j.$t,-1<d.j.f(".1c-")?d.j=d.j.b(d.j.f(".1c-")+6):-1<d.j.f(".1d-")&&(d.j=d.j.b(d.j.f(".1d-")+6))),"1e"9 e.2.3[n]){p r=q A;d.y=e.2.3[n].1e.$t,r.1f=d.y.b(0,4),r.1g=d.y.b(5,7),r.1h=d.y.b(8,10),r.1i=d.y.b(11,13),r.1j=d.y.b(14,16),d.y=r}o("1k"9 e.2.3[n]){p i=q A;d.z=e.2.3[n].1k.$t,i.1f=d.z.b(0,4),i.1g=d.z.b(5,7),i.1h=d.z.b(8,10),i.1i=d.z.b(11,13),i.1j=d.z.b(14,16),d.z=i}o("W"9 e.2.3[n]){d.1l=q 1b;x(p s=0;s<e.2.3[n].W.u;s++)d.1l.1m(e.2.3[n].W[s].1E)}o("G"9 e.2.3[n]&&(d.G=e.2.3[n].G.$t),"P"9 e.2.3[n]?d.P=e.2.3[n].P.$t:"1n"9 e.2.3[n]&&(d.P=e.2.3[n].1n.$t),"g"9 e.2.3[n])x(s=0;s<e.2.3[n].g.u;s++)"19"==e.2.3[n].g[s].M&&(d.g=e.2.3[n].g[s].H);o("k"9 e.2.3[n]){d.k=q A;x(s=0;s<e.2.3[n].k.u;s++){"I"9 e.2.3[n].k[s]&&(d.k.I=e.2.3[n].k[s].I.$t),"1o"9 e.2.3[n].k[s]&&(d.k.g=e.2.3[n].k[s].1o.$t),"v$X"9 e.2.3[n].k[s]&&(d.k.1F=e.2.3[n].k[s].v$X.Q);1G}}o("1p$J"9 e.2.3[n]&&(d.R=e.2.3[n].1p$J.1q),"S$1r"9 e.2.3[n]&&(d.D=e.2.3[n].S$1r.$t),"S$9-1s-1t"9 e.2.3[n]&&(d.1H=e.2.3[n]["S$9-1s-1t"].H),"v$F"9 e.2.3[n])x(s=0;s<e.2.3[n].v$F.u;s++)"1u.1I"==e.2.3[n].v$F[s].I&&(d.Y=e.2.3[n].v$F[s].1v,d.Y=d.Y.C("1J-","")),"1u.1K"==e.2.3[n].v$F[s].I&&(d.1L=e.2.3[n].v$F[s].1v);t.1a.1m(d)}}K t}K"1M 1N"},1O:L(e,t){x(p n=e.1w("<"),d=0;d<n.u;d++)-1!=n[d].f(">")&&(n[d]=n[d].b(n[d].f(">")+1,n[d].u));K n=(n=n.1P("")).b(0,t-1)},1Q:L(e,t,n,d){K 1R==e?\'<Z 12="R 1S" 15="J" Q="\'+d.C("/17-c/","/h"+n+"-w"+t+"-c/")+\'"/>\':-1<e.f("1T")||-1<e.f("/1U/")?\'<1x 12="R 1V" 1W="1X-X:1q(\'+e.C("/1Y","/1Z")+\')"><Z 15="J" Q="\'+d.C("/17-c/","/h"+n+"-w"+t+"-c/")+\'"/></1x>\':\'<Z 12="R 20" 15="J" Q="\'+e.C("/17-c/","/h"+n+"-w"+t+"-c/")+\'"/>\'},21:L(e,t){K e.1w(" ")[22(t,10)-1]}};',"|","split","||feed|entry||||||in|blogStats|substring||||indexOf|link|||id|author|next|previous||if|var|new||||length|gd||for|datePublished|dateUpdated|Object|blogId|replace|comments|openSearch|extendedProperty|title|href|name|thumbnail|return|function|rel|posts|feeds|content|src|thumb|thr|totalResults|startIndex|itemsPerPage|category|image|commentId|img|||class|||alt||s72|subtitle|alternate|blogPosts|Array|post|page|published|year|month|day|hour|minute|updated|label|push|summary|uri|media|url|total|reply|to|blogger|value|split|div|arThemes|PostsObject|blog|blogTitle|blogSubTitle|blogLink|term|photo|break|commentPostLink|itemClass|pid|displayTime|commentDate|No|Supported|snippetGet|join|thumbGet|null|thumb_default|youtube|vi|thumb_video|style|background|default|hqdefault|thumb_img|monthGet|parseInt","","fromCharCode","replace","\\w+","\\b","g"],$get=function(e){return document.querySelectorAll(e)};!function(e){var n=!1;if("function"==typeof define&&define.amd&&(define(e),n=!0),"object"==typeof exports&&(module.exports=e(),n=!0),!n){var o=window.Cookies,t=window.Cookies=e();t.noConflict=function(){return window.Cookies=o,t}}}(function(){function e(){for(var e=0,n={};e<arguments.length;e++){var o=arguments[e];for(var t in o)n[t]=o[t]}return n}function n(o){function t(n,r,i){var c;if("undefined"!=typeof document){if(arguments.length>1){if("number"==typeof(i=e({path:"/"},t.defaults,i)).expires){var a=new Date;a.setMilliseconds(a.getMilliseconds()+864e5*i.expires),i.expires=a}i.expires=i.expires?i.expires.toUTCString():"";try{c=JSON.stringify(r),/^[\{\[]/.test(c)&&(r=c)}catch(e){}r=o.write?o.write(r,n):encodeURIComponent(r+"").replace(/%(23|24|26|2B|3A|3C|3E|3D|2F|3F|40|5B|5D|5E|60|7B|7D|7C)/g,decodeURIComponent),n=(n=(n=encodeURIComponent(n+"")).replace(/%(23|24|26|2B|5E|60|7C)/g,decodeURIComponent)).replace(/[\(\)]/g,escape);var s="";for(var f in i)i[f]&&(s+="; "+f,!0!==i[f]&&(s+="="+i[f]));return document.cookie=n+"="+r+s}n||(c={});for(var p=document.cookie?document.cookie.split("; "):[],d=/(%[0-9A-Z]{2})+/g,u=0;u<p.length;u++){var l=p[u].split("="),C=l.slice(1).join("=");this.json||'"'!==C.charAt(0)||(C=C.slice(1,-1));try{var m=l[0].replace(d,decodeURIComponent);if(C=o.read?o.read(C,m):o(C,m)||C.replace(d,decodeURIComponent),this.json)try{C=JSON.parse(C)}catch(e){}if(n===m){c=C;break}n||(c[m]=C)}catch(e){}}return c}}return t.set=t,t.get=function(e){return t.call(t,e)},t.getJSON=function(){return t.apply({json:!0},[].slice.call(arguments))},t.defaults={},t.remove=function(n,o){t(n,"",e(o,{expires:-1}))},t.withConverter=n,t}return n(function(){})});eval(function(e,t,n,i,r,d){if(r=function(e){return e.toString(35)},!$salE[5][$salE[4]](/^/,String)){for(;n--;)d[r(n)]=i[n]||r(n);i=[function(e){return d[e]}],r=function(){return $salE[6]},n=1}for(;n--;)i[n]&&(e=e[$salE[4]](new RegExp($salE[7]+r(n)+$salE[7],$salE[8]),i[n]));return e}($salE[0],0,35,$salE[3][$salE[2]]($salE[1]),0,{}));eval(function(e,t,n,d,a,s){if(a=function(e){return(e<62?$salF[4]:a(parseInt(e/62)))+(35<(e%=62)?String[$salF[5]](e+29):e.toString(36))},!$salF[4][$salF[6]](/^/,String)){for(;n--;)s[a(n)]=d[n]||a(n);d=[function(e){return s[e]}],a=function(){return $salF[7]},n=1}for(;n--;)d[n]&&(e=e[$salF[6]](new RegExp($salF[8]+a(n)+$salF[8],$salF[9]),d[n]));return e}($salF[0],0,127,$salF[3][$salF[2]]($salF[1]),0,{}));$get('meta[name="theme-color"]')[0].setAttribute("content","#c4183c");$get('meta[name="msapplication-navbutton-color"]')[0].setAttribute("content","#c4183c")/*]]>*/</script>

      <!-- .wrapper -->
      <div class='wrapper uk-offcanvas-content'>

        <!-- header -->
        <header>

          <!-- .topnav -->
          <div class='topnav_wrapper'>
            <div class='uk-container'>
              <b:section class='topnav uk-panel uk-padding-large-bottom' id='topnav' maxwidgets='1' showaddelements='false'>
                <b:widget id='LinkList1' locked='true' title='أيقونات التواصل الإجتماعي' type='LinkList' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='link-5'>#!</b:widget-setting>
                    <b:widget-setting name='link-3'>#!</b:widget-setting>
                    <b:widget-setting name='link-4'>#!</b:widget-setting>
                    <b:widget-setting name='text-1'>facebook</b:widget-setting>
                    <b:widget-setting name='text-0'>twitter</b:widget-setting>
                    <b:widget-setting name='text-3'>instagram</b:widget-setting>
                    <b:widget-setting name='text-2'>google-plus</b:widget-setting>
                    <b:widget-setting name='text-5'>dribbble</b:widget-setting>
                    <b:widget-setting name='text-4'>behance</b:widget-setting>
                    <b:widget-setting name='sorting'>NONE</b:widget-setting>
                    <b:widget-setting name='link-1'>#!</b:widget-setting>
                    <b:widget-setting name='link-2'>#!</b:widget-setting>
                    <b:widget-setting name='link-0'>#!</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;topnav&quot;'>
            <div class='uk-grid' data-uk-grid=''>
              <div class='sidenav_button uk-width-auto uk-margin-remove'>
                <a class='uk-button' data-uk-toggle='target:#sidenav' href='#!'>
                  <b:class expr:name='data:theme.layout.enableLightStyle ? &quot;uk-button-primary&quot; : &quot;uk-button-default&quot;'/>
                  <span data-uk-icon='thumbnails'/>
                  <span class='uk-margin-small-right'><data:theme.text.sideMenu/></span>
                </a>
              </div>
              <div class='topnav_social_wrapper uk-width-expand uk-margin-remove'>
                <div class='uk-align-left uk-margin-remove'>
                  <ul class='topnav_social uk-iconnav'>
                    <b:loop index='i' values='data:links' var='link'>
                      <li><a data-uk-tooltip='pos:bottom' expr:class='&quot;uk-icon-button icon_&quot; + data:link.name' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
                    </b:loop>
                  </ul>
                </div>
              </div>
            </div>
          </b:if>
          <b:if cond='data:widget.sectionId == &quot;social&quot;'>
            <ul class='social_social uk-iconnav'>
              <b:loop index='i' values='data:links' var='link'>
                  <li><a data-uk-tooltip='pos:top' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
              </b:loop>
            </ul>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;social&quot;,&quot;topnav&quot;}'>
            <div class='widget-content'>
              <b:class cond='!data:theme.layout.enableLightStyle and data:widget.sectionId in {&quot;footer_section_1&quot;,&quot;footer_section_2&quot;,&quot;footer_section_3&quot;,&quot;footer_section_4&quot;}' name='uk-light'/>
              <ul class='uk-list uk-list-bullet uk-margin-remove'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:href='data:link.target'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
            </div>
          </div>

          <!-- .mainnav -->
          <div class='mainnav_wrapper'>
            <b:attr cond='data:theme.layout.enableStickyHeader' name='data-uk-sticky' value='sel-target:.mainnav;cls-active:uk-navbar-sticky'/>
            <div class='uk-container'>
              <b:section class='mainnav uk-panel uk-grid' id='mainnav' maxwidgets='2' showaddelements='false'>
                <b:widget id='Header1' locked='true' title='Salbuta (رأس الصفحة)' type='Header' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='displayUrl'>http://1.bp.blogspot.com/-RN5eSQCeFJc/W0vBLeGmEBI/AAAAAAAAGM0/2556CYyDPlgkPbcrx66L-3y05hOium01QCK4BGAYYCw/s1600/logo_1x.png</b:widget-setting>
                    <b:widget-setting name='displayHeight'>60</b:widget-setting>
                    <b:widget-setting name='sectionWidth'>767</b:widget-setting>
                    <b:widget-setting name='useImage'>true</b:widget-setting>
                    <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                    <b:widget-setting name='imagePlacement'>REPLACE</b:widget-setting>
                    <b:widget-setting name='displayWidth'>150</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main' var='this'>
          <b:class name='uk-margin-remove uk-width-auto'/>
          <div class='haeder-menu uk-margin-left uk-hidden@l' data-uk-tooltip='pos:bottom' expr:title='data:theme.text.menu'>
            <a class='icon_menu' data-uk-icon='icon:menu;ratio:1.2' data-uk-toggle='target:#sidemenu' href='#!'/>
          </div>
          <div class='header-widget'>
            <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
            <b:include cond='data:imagePlacement not in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='title'/>
          </div>
          <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='behindImageStyle'/>
        </b:includable>
                  <b:includable id='behindImageStyle'>
          <b:if cond='data:sourceUrl and data:imagePlacement == &quot;BEHIND&quot;'>
            <b:include cond='data:this.image' data='{ image: data:this.image, selector: &quot;.header-widget&quot; }' name='responsiveImageStyle'/>
          </b:if>
        </b:includable>
                  <b:includable id='description'>
    <p>
      <data:this.description/>
    </p>
  </b:includable>
                  <b:includable id='image'>
          <b:if cond='!data:view.isSingleItem'>
            <h1 class='clip'>
              <a expr:href='data:blog.homepageUrl' expr:title='data:title'><span><data:title/></span></a>
            </h1>
          </b:if>
          <a class='header-image-wrapper' expr:href='data:blog.homepageUrl'>
            <b:include data='{ image: data:image, altText: data:blog.title.escaped }' name='responsiveImage'/>
          </a>
        </b:includable>
                  <b:includable id='responsiveImage'>
          <img expr:alt='data:altText ?: data:messages.image' expr:src='data:image'/>
        </b:includable>
                  <b:includable id='title'>
          <h1><b:tag expr:href='data:blog.homepageUrl' name='a'><data:title/></b:tag></h1>
        </b:includable>
                </b:widget>
                <b:widget id='HTML1' locked='true' title='القائمة' type='HTML' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='content'>&lt;li&gt;&lt;a href=&#39;/&#39;&gt;الرئيسية&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;/&#39;&gt;تصميم&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;/&#39;&gt;حياة&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;/&#39;&gt;مميزة&lt;/a&gt;&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;#&#39;&gt;الصفحات&lt;/a&gt;
  &lt;ul&gt;
    &lt;li&gt;&lt;a href=&quot;#!&quot;&gt;صفحات مخصصة&lt;/a&gt;
      &lt;ul&gt;
        &lt;li&gt;&lt;a href=&quot;/2018/02/&quot;&gt;صفحة الأرشيف&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href=&quot;/search/label/%D8%A7%D9%84%D8%B7%D8%A8%D9%8A%D8%B9%D8%A9&quot;&gt;صفحة التسميات&lt;/a&gt;&lt;/li&gt;
        &lt;li&gt;&lt;a href=&quot;/search?q=%D9%83%D9%8A%D9%81&amp;max-results=9&quot;&gt;صفحة البحث&lt;/a&gt;&lt;/li&gt;
      &lt;/ul&gt;
    &lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/p/static-page.html&quot;&gt;صفحة تقليدية&lt;/a&gt;&lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/p/typography.html&quot;&gt;أسلوب الكتابة&lt;/a&gt;&lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/p/short-codes.html&quot;&gt;أكواد قصيرة&lt;/a&gt;&lt;/li&gt;
  &lt;/ul&gt;
&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;#&#39;&gt;المواضيع&lt;/a&gt;
  &lt;ul&gt;
    &lt;li&gt;&lt;a href=&quot;/2017/05/how-star-isn-as-bad-as-you-think.html&quot;&gt;موضوع 1&lt;/a&gt;&lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/2018/02/mars-can-get-you-your-heart-desire.html&quot;&gt;موضوع 2&lt;/a&gt;&lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/2018/01/cards-could-help-you-win-game.html&quot;&gt;موضوع 3&lt;/a&gt;&lt;/li&gt;
    &lt;li&gt;&lt;a href=&quot;/2018/02/layers-of-july-will-be-hidden.html&quot;&gt;موضوع 4&lt;/a&gt;&lt;/li&gt;
  &lt;/ul&gt;
&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;#&quot;&gt;ميجا واحدة&lt;/a&gt;
  &lt;div class=&quot;mega&quot; data-label=&quot;مميزة&quot;&gt;&lt;/div&gt;
&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;#&quot;&gt;ميجا متعددة&lt;/a&gt;
  &lt;div class=&quot;mega&quot; data-label=&quot;موضة&quot;&gt;&lt;/div&gt;
  &lt;div class=&quot;mega&quot; data-label=&quot;حياة&quot;&gt;&lt;/div&gt;
  &lt;div class=&quot;mega&quot; data-label=&quot;طعام&quot;&gt;&lt;/div&gt;
&lt;/li&gt;
&lt;li&gt;&lt;a href=&#39;/404&#39;&gt;خطأ 404&lt;/a&gt;&lt;/li&gt;</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
            </div>
          </div>

        </header>

        <!-- main -->
        <main>

          <b:if cond='data:theme.layout.enableWavyStyle'>
            <!-- .top_bg -->
            <div class='top_bg'>
              <b:include data='{ id: &quot;fill_1&quot;, isHeader: true }' name='background-svg'/>
            </div>
          </b:if>

          <!-- .main_content -->
          <div class='main_content uk-container'>

            <b:if cond='!data:view.isError'>
              <b:with value='data:theme.layout.enableIndexSidebar or data:view.isPost' var='enableSidebar'>
                <b:with value='data:enableSidebar and !data:view.isPage' var='enableIndexSidebar'>
                  <b:with value='data:theme.layout.enablePagesSidebar and data:view.isPage' var='enablePagesSidebar'>
                    <b:tag class='uk-grid' cond='data:enableIndexSidebar or data:enablePagesSidebar' name='div'>

                      <!-- .main -->
                      <b:tag class='uk-width-2-3@l' expr:cond='data:enableIndexSidebar or data:enablePagesSidebar' name='div'>
                        <b:section class='main uk-width-auto' cond='!data:view.isError' id='main' maxwidgets='2' showaddelements='false'>
                          <b:widget cond='!data:view.isSingleItem' id='Label1' locked='true' title='التسميات' type='Label' visible='true'>
                            <b:widget-settings>
                              <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                              <b:widget-setting name='display'>LIST</b:widget-setting>
                              <b:widget-setting name='selectedLabelsList'/>
                              <b:widget-setting name='showType'>ALL</b:widget-setting>
                              <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
                            </b:widget-settings>
                            <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                            <b:includable id='cloud'>
          <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
            <a class='label-name uk-button uk-button-default uk-button-small uk-margin-small-left uk-margin-small-bottom' expr:href='data:label.url'>
              <b:class expr:name='&quot;label-size-&quot; + data:label.cssSize'/>
              <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-margin-small-right'>_<data:label.count/></span></b:if>
            </a>
          </b:loop>
        </b:includable>
                            <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;main&quot;'>
            <b:include name='filter'/>
            <b:else/>
            <div class='widget-content'>
              <b:class expr:name='data:this.display + &quot;-label-widget-content&quot;'/>
              <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
              <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='filter'>
          <div class='filtering_labels uk-grid uk-margin-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isHomepage'>
              <div class='select_label uk-width-expand@m'>
                <b:if cond='data:theme.layout.enableFilterOption'>
                  <script class='js'>
                    var filterTags = Object.values({<b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
                  </script>
                  <ul class='uk-list uk-list-inline uk-visible@l'>
                    <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='settings'/><span><data:theme.text.filter/></span></span></li>
                    <li><a class='uk-button uk-button-default uk-margin-bottom uk-active' data-uk-filter-control='' href='#!'><data:messages.viewAll/></a></li>
                    <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                      <li><a class='uk-button uk-button-default uk-margin-bottom' expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' href='#!'><data:label.name/></a></li>
                    </b:loop>
                  </ul>
                  <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                    <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='settings'/></div>
                    <div class='uk-width-auto@m uk-width-expand'>
                      <select class='uk-select'>
                        <option data-uk-filter-control='' value=''><data:messages.viewAll/></option>
                        <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                          <option expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' expr:value='&quot;.filter_&quot; + data:i'><data:label.name/></option>
                        </b:loop>
                      </select>
                    </div>
                  </div>
                </b:if>
              </div>
            </b:if>
            <b:if cond='data:view.isMultipleItems and !data:view.isHomepage'>
              <div class='breadcrumb uk-width-expand@m'>
                <ul class='uk-breadcrumb'>
                  <li><a href='/'><data:messages.home/></a></li>
                  <b:if cond='data:view.isSearch'>
                    <li><a href='/search'><data:messages.search/></a></li>
                    <b:if cond='data:view.isLabelSearch'>
                      <li class='uk-disabled'><span><data:messages.labels/></span></li>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                      <b:elseif cond='data:view.search.query'/>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                    </b:if>
                  </b:if>
                  <b:if cond='data:view.isArchive'>
                    <li class='uk-disabled'><span><data:messages.archive/></span></li>
                    <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                  </b:if>
                </ul>
              </div>
            </b:if>
            <b:if cond='data:theme.layout.enableViewOption'>
              <div class='select_view uk-width-exapnd uk-width-auto@m'>
                <b:class cond='!data:theme.layout.enableFilterOption' name='uk-margin-bottom'/>
                <ul class='uk-list uk-list-inline uk-visible@l'>
                  <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='cog'/><span><data:theme.text.view/></span></span></li>
                  <li class='uk-active'><a class='uk-icon-button' data-uk-icon='expand' data-uk-tooltip='pos:top' expr:title='data:theme.text.expandPosts' href='#!' id='view_e'/></li>
                  <li><a class='uk-icon-button' data-uk-icon='shrink' data-uk-tooltip='pos:top' expr:title='data:theme.text.shrinkPosts' href='#!' id='view_s'/></li>
                </ul>
                <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                  <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='cog'/></div>
                  <div class='uk-width-auto@m uk-width-expand'>
                    <select class='uk-select'>
                      <option value='expand'><data:theme.text.expandPosts/></option>
                      <option value='shrink'><data:theme.text.shrinkPosts/></option>
                    </select>
                  </div>
                </div>
                <script class='js'>/*<![CDATA[*/eval(function(e,c,r,t,d,i){if(d=function(e){return e.toString(16)},!$salD[5][$salD[4]](/^/,String)){for(;r--;)i[d(r)]=t[r]||d(r);t=[function(e){return i[e]}],d=function(){return $salD[6]},r=1}for(;r--;)t[r]&&(e=e[$salD[4]](new RegExp($salD[7]+d(r)+$salD[7],$salD[8]),t[r]));return e}($salD[0],0,16,$salD[3][$salD[2]]($salD[1]),0,{}));//]]></script>
              </div>
            </b:if>
          </div>
        </b:includable>
                            <b:includable id='list'>
          <ul class='uk-list uk-list-bullet uk-margin-remove'>
            <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
              <li>
                <a class='label-name' expr:href='data:label.url'>
                  <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-align-left uk-margin-remove'><data:label.count/></span></b:if>
                </a>
              </li>
            </b:loop>
          </ul>
        </b:includable>
                          </b:widget>
                          <b:widget id='Blog1' locked='true' title='رسائل المدونة الإلكترونية' type='Blog' visible='true'>
                            <b:widget-settings>
                              <b:widget-setting name='commentLabel'/>
                              <b:widget-setting name='showShareButtons'>true</b:widget-setting>
                              <b:widget-setting name='authorLabel'>المؤلف</b:widget-setting>
                              <b:widget-setting name='disableGooglePlusShare'>true</b:widget-setting>
                              <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
                              <b:widget-setting name='timestampLabel'>التاريخ</b:widget-setting>
                              <b:widget-setting name='reactionsLabel'>ردود الأفعال</b:widget-setting>
                              <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
                              <b:widget-setting name='style.layout'>1x1</b:widget-setting>
                              <b:widget-setting name='showLocation'>true</b:widget-setting>
                              <b:widget-setting name='showTimestamp'>true</b:widget-setting>
                              <b:widget-setting name='postsPerAd'>4</b:widget-setting>
                              <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
                              <b:widget-setting name='backlinksLabel'>Links to this post</b:widget-setting>
                              <b:widget-setting name='showDateHeader'>false</b:widget-setting>
                              <b:widget-setting name='style.textcolor'>#2196f3</b:widget-setting>
                              <b:widget-setting name='showCommentLink'>true</b:widget-setting>
                              <b:widget-setting name='style.urlcolor'>#212121</b:widget-setting>
                              <b:widget-setting name='postLocationLabel'>الموقع</b:widget-setting>
                              <b:widget-setting name='showAuthor'>true</b:widget-setting>
                              <b:widget-setting name='style.linkcolor'>#757575</b:widget-setting>
                              <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
                              <b:widget-setting name='showLabels'>true</b:widget-setting>
                              <b:widget-setting name='postLabelsLabel'>التسميات</b:widget-setting>
                              <b:widget-setting name='showBacklinks'>true</b:widget-setting>
                              <b:widget-setting name='showInlineAds'>true</b:widget-setting>
                              <b:widget-setting name='showReactions'>false</b:widget-setting>
                            </b:widget-settings>
                            <b:includable id='main' var='this'>
          <div expr:class='data:view.isMultipleItems ? &quot;blog_posts&quot; : &quot;single_post&quot;' expr:id='data:view.isMultipleItems ? &quot;blog_posts&quot; : &quot;single_post&quot;'>
            <b:class name='hfeed'/>
            <b:class cond='data:view.isMultipleItems and !data:enableSidebar' name='uk-child-width-1-1 uk-child-width-1-2@m uk-child-width-1-3@l'/>
            <b:class cond='data:view.isMultipleItems and data:enableSidebar' name='uk-child-width-1-1 uk-child-width-1-2@m uk-child-width-1-2@l'/>
            <b:attr cond='data:view.isMultipleItems' name='data-uk-grid' value='masonry:true'/>
            <b:with value='3' var='maxNumAds'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include data='post' expr:name='data:view.isMultipleItems ? &quot;postGridsAndAd&quot; : &quot;postCommentsAndAd&quot;'/>
                <b:include cond='data:view.isMultipleItems' data='post' name='inlineAdGrid'/>
              </b:loop>
              <b:if cond='data:posts.length == 0'>
                <div class='uk-width'>
                  <div class='no_results'>
                    <span class='uk-margin-left' data-uk-icon='warning'/><data:messages.noResultsFound/>
                  </div>
                </div>
              </b:if>
            </b:with>
          </div>
          <b:include name='nextPageLink'/>
        </b:includable>
                            <b:includable id='aboutPostAuthor'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='addComments'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='commentAuthorAvatar'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='commentDeleteIcon'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='commentForm' var='post'>
          <div class='post_comments_form'>
            <b:if cond='data:this.messages.blogComment != &quot;&quot;'>
              <div class='post_comments_message'><span class='uk-margin-small-left' data-uk-icon='info'/><data:this.messages.blogComment/></div>
            </b:if>
            <b:include data='post' name='commentFormIframeSrc'/>
            <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight ?: &quot;90px&quot;' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
            <div class='comments_emotions' id='comments_emotions'/>
            <data:post.cmtfpIframe/>
            <script>BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);</script>
          </div>
        </b:includable>
                            <b:includable id='commentFormIframeSrc' var='post'>
  <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
</b:includable>
                            <b:includable id='commentItem' var='comment'>
          <li class='comment' expr:id='&quot;c&quot; + data:comment.id'>
            <div class='avatar-image-container'>
              <b:if cond='data:blog.enabledCommentProfileImages'>
                <img alt='author-avatar' expr:src='resizeImage(data:comment.authorAvatarSrc,80,&quot;1:1&quot;)'/>
              </b:if>
              <div class='comment-header'>
                <cite class='user blog-author'>
                  <b:if cond='data:comment.authorUrl'>
                    <a expr:href='data:comment.authorUrl' rel='nofollow'><data:comment.author/></a>
                    <b:else/>
                    <span><data:comment.author/></span>
                  </b:if>
                </cite>
                <span class='datetime secondary-text'>
                  <a expr:href='data:comment.url' rel='nofollow'><data:comment.timestamp/></a>
                </span>
              </div>
              <span class='comment-actions secondary-text'>
                <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
                  <b:if cond='data:showCmtPopup'>
                    <div class='goog-toggle-button'>
                      <div class='goog-inline-block comment-action-icon'/>
                    </div>
                    <b:else/>
                    <a expr:href='data:comment.deleteUrl' target='_self'>
                      <span class='uk-margin-small-left' data-uk-icon='trash'/><data:messages.deleteComment/></a>
                  </b:if>
                </span>
              </span>
            </div>
            <div class='comment-block'>
              <div expr:class='&quot;comment-body&quot; + (data:comment.isDeleted ? &quot; deleted-comment&quot; : &quot;&quot;)'>
                <data:comment.body/>
              </div>
            </div>
          </li>
        </b:includable>
                            <b:includable id='commentList'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='commentPicker' var='post'>
          <b:if cond='data:post.allowComments'>
            <div class='post_comments uk-margin-medium-top' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
              <b:if cond='data:post.commentSource != 1'>
                <b:class cond='data:post.showThreadedComments' name='threaded'/>
                <b:class cond='!data:post.showThreadedComments' name='not_threaded'/>
              </b:if>
              <b:include name='commentsTitle'/>
              <div class='post_comments_content'>
                <b:if cond='data:post.commentSource == 1'>
                  <b:include data='post' name='iframeComments'/>
                  <b:elseif cond='data:post.showThreadedComments'/>
                  <b:include data='post' name='threadedComments'/>
                  <b:else/>
                  <b:include data='post' name='comments'/>
                </b:if>
              </div>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='comments' var='post'>
          <b:class cond='!data:post.allowNewComments' name='comments_locked'/>
          <b:if cond='data:post.comments'>
            <div class='post_comments_holder' expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
              <b:include cond='data:post.comments' data='post.comments' name='commentList'/>
              <ol id='comments-block'>
                <b:loop values='data:post.comments' var='comment'>
                  <b:include data='comment' name='commentItem'/>
                </b:loop>
              </ol>
            </div>
          </b:if>
          <b:if cond='data:post.embedCommentForm'>
            <b:if cond='data:post.allowNewComments'>
              <b:include data='post' name='commentForm'/>
              <b:else/>
              <div class='post_comments_locked uk-margin-top uk-text-danger'>
                <span class='uk-margin-small-left' data-uk-icon='ban'/><span><data:post.noNewCommentsText/></span>
              </div>
            </b:if>
            <b:else/>
            <b:if cond='data:post.allowComments'>
              <div class='add_comments uk-margin-top'>
                <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
                  <span class='uk-margin-small-left' data-uk-icon='commenting'/><b:message name='messages.postAComment'/>
                </a>
              </div>
            </b:if>
          </b:if>
          <b:if cond='data:showCmtPopup'>
            <div id='comment-popup'>
              <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'/>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='commentsLink'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='commentsTitle'>
          <h3 class='post_comments_title'><span class='uk-margin-left' data-uk-icon='comments'/><data:messages.comments/></h3>
        </b:includable>
                            <b:includable id='emailPostIcon'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='feedLinks'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='feedLinksBody'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='footerBylines'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='headerByline'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='homePageLink'>
  <a class='home-link' expr:href='data:blog.homepageUrl'>
    <data:messages.home/>
  </a>
</b:includable>
                            <b:includable id='iframeComments' var='post'>
  <!-- G+ comments, no longer available. The includable is retained for backwards-compatibility. -->
</b:includable>
                            <b:includable id='inlineAd' var='post'>
  <b:if cond='!data:view.isPreview'>
    <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
      <!-- Ad -->
      <div class='inline-ad'>
        <b:if cond='data:this.adCode != &quot;&quot;'>
          <data:this.adCode/>
        <b:else/>
          <b:include cond='data:this.adClientId or data:blog.adsenseClientId' name='defaultAdUnit'/>
        </b:if>
      </div>
    </b:if>
  <b:else/>
    <div class='inline-ad'>
      <div class='inline-ad-placeholder'>
        <span><b:message name='messages.adsGoHere'/></span>
      </div>
    </div>
  </b:if>
</b:includable>
                            <b:includable id='inlineAdGrid' var='post'>
          <b:if cond='data:post.includeAd'>
            <b:if cond='not data:maxNumAds or data:post.adNumber lt data:maxNumAds'>
              <div class='post inline_ad'>
                <div class='uk-card uk-card-hover uk-card-default'>
                  <em><data:messages.adsGoHere/></em>
                  <div class='post_content uk-card-small uk-card-body'>
                    <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
                      <data:this.adCode/>
                      <b:else/>
                      <b:include data='{height: &quot;250px&quot;}' name='adverts-code'/>
                    </b:if>
                  </div>
                </div>
              </div>
            </b:if>
          </b:if>
        </b:includable>
                            <b:includable id='inlineAdPost' var='post'>
          <b:if cond='data:post.includeAd'>
            <b:if cond='not data:maxNumAds or data:post.adNumber lt data:maxNumAds'>
              <div class='inline_ad'>
                <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
                  <data:this.adCode/>
                  <b:else/>
                  <b:include data='{height: &quot;90px&quot;}' name='adverts-code'/>
                </b:if>
              </div>
            </b:if>
          </b:if>
        </b:includable>
                            <b:includable id='nextPageLink'>
          <b:if cond='data:view.isMultipleItems and data:olderPageUrl'>
            <div class='blog_pager uk-text-center uk-margin-large-top' id='blog_pager'>
              <a class='blog-pager-older-link uk-button uk-button-default' data-uk-icon='more' expr:href='data:olderPageUrl' expr:title='data:messages.morePosts'>
                <span class='uk-margin-small-left'><data:messages.morePosts/></span>
              </a>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='post'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='postAlignment' var='post'>
          <b:if cond='data:view.isPost'>
            <script class='js'>var labelsName = &quot;<b:loop values='data:post.labels' var='label'><data:label.name/> </b:loop>&quot;.trim().split(&quot; &quot;),postImage = &quot;<b:eval expr='resizeImage(data:post.featuredImage,1600,&quot;16:9&quot;)'/>&quot;;/*<![CDATA[*/eval(function(e,n,t,a,r,i){if(r=function(e){return(e<51?$salB[4]:r(parseInt(e/51)))+(35<(e%=51)?String[$salB[5]](e+29):e.toString(36))},!$salB[4][$salB[6]](/^/,String)){for(;t--;)i[r(t)]=a[t]||r(t);a=[function(e){return i[e]}],r=function(){return $salB[7]},t=1}for(;t--;)a[t]&&(e=e[$salB[6]](new RegExp($salB[8]+r(t)+$salB[8],$salB[9]),a[t]));return e}($salB[0],0,51,$salB[3][$salB[2]]($salB[1]),0,{}));//]]></script>
          </b:if>
        </b:includable>
                            <b:includable id='postAuthor'>
          <span class='post_author vcard uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_author_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:user;ratio:.75'/><data:byline.label/>
            </span>
            <span class='fn'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:if cond='data:post.author.profileUrl'>
                <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <span><data:post.author.name/></span>
                </a>
                <b:else/>
                <span><data:post.author.name/></span>
              </b:if>
            </span>
          </span>
        </b:includable>
                            <b:includable id='postBody' var='post'>
          <div class='post_body entry-content' expr:id='&quot;post_body_&quot; + data:post.id'>
            <b:class cond='data:view.isSingleItem' name='uk-margin-large-bottom'/>
            <data:post.body/>
          </div>
        </b:includable>
                            <b:includable id='postBodySnippet' var='post'>
  <b:include data='post' name='postBody'/>
</b:includable>
                            <b:includable id='postCommentsAndAd' var='post'>
          <article class='post hentry'>
            <b:include data='post' name='postMeta'/>
            <div class='post_content'>
              <b:include data='post' name='postTitle'/>
              <b:include data='post' name='postHeader'/>
              <b:include data='post' name='postAlignment'/>
              <b:include data='post' name='postBody'/>
              <b:include data='post' name='inlineAdPost'/>
              <b:include data='post' name='postRelated'/>
              <b:include data='post' name='postFooter'/>
            </div>
            <b:include data='post' name='commentPicker'/>
          </article>
        </b:includable>
                            <b:includable id='postCommentsLink'>
          <span class='post_comment_link uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_comment_link_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:comment;ratio:.75'/><data:byline.label/>
            </span>
            <a class='comment-link' expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
              <b:if cond='data:post.numberOfComments gt 0'>
                <b:message name='messages.numberOfComments'><b:param expr:value='data:post.numberOfComments' name='numComments'/></b:message>
                <b:else/>
                <data:messages.postAComment/>
              </b:if>
            </a>
          </span>
        </b:includable>
                            <b:includable id='postFooter' var='post'>
          <div class='post_footer uk-article-meta'>
            <b:loop index='i' values='data:widgets.Blog.first.footerBylines' var='region'>
              <b:if cond='data:region.items.any'>
                <div class='post_footer_line'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <b:class expr:name='&quot;post_footer_line_&quot; + (data:i + 1)'/>
                  <b:include data='region.items' name='bylineRegion'/>
                </div>
              </b:if>
            </b:loop>
            <b:include cond='!data:view.isPage' data='post' name='postFooterAuthorProfile'/>
          </div>
        </b:includable>
                            <b:includable id='postFooterAuthorProfile' var='post'>
          <b:if cond='data:post.author.aboutMe'>
            <div class='post_author_profile uk-margin-top'>
              <div class='uk-grid uk-grid-medium'>
                <b:if cond='data:post.author.authorPhoto.image'>
                  <div class='uk-width-auto uk-visible@m'>
                    <div class='post_author_profile_photo'>
                      <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                        <img alt='author photo' expr:src='data:post.author.authorPhoto.image'/>
                      </a>
                    </div>
                  </div>
                </b:if>
                <div class='uk-width-expand'>
                  <div class='post_author_profile_name uk-flex uk-flex-middle uk-margin-small-bottom uk-text-uppercase'>
                    <b:if cond='data:post.author.authorPhoto.image'>
                      <a class='g-profile uk-margin-left uk-hidden@m' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                        <img alt='author photo' expr:src='data:post.author.authorPhoto.image'/>
                      </a>
                    </b:if>
                    <a class='g-profile' expr:href='data:post.author.profileUrl' rel='author' title='author profile'>
                      <span><data:post.author.name/></span>
                    </a>
                  </div>
                  <div class='post_author_profile_desc'>
                    <span><data:post.author.aboutMe/></span>
                  </div>
                </div>
              </div>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='postGridsAndAd' var='post'>
          <article class='post hentry'>
            <b:attr expr:value='data:post.id' name='data-id'/>
            <script>
              var filterTags_<data:post.id/> = Object.values({<b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
            </script>
            <b:include data='post' name='postMeta'/>
            <div class='uk-card uk-card-hover uk-card-default'>
              <b:include name='postThumbnail'/>
              <div class='post_content uk-card-small uk-card-body'>
                <b:include data='post' name='postLabels'/>
                <b:include data='post' name='postTitle'/>
                <b:include data='post' name='postSnippet'/>
                <b:include data='post' name='postMetaInfo'/>
              </div>
            </div>
          </article>
        </b:includable>
                            <b:includable id='postHeader' var='post'>
          <div class='post_header uk-article-meta uk-margin-bottom'>
            <div class='post_header_line'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:loop index='i' values='data:widgets.Blog.first.headerByline' var='region'>
                <b:if cond='data:region.items.any'>
                  <b:include data='region.items' name='bylineRegion'/>
                </b:if>
              </b:loop>
            </div>
          </div>
        </b:includable>
                            <b:includable id='postJumpLink'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='postLabels'>
          <b:if cond='data:post.labels'>
            <b:if cond='data:view.isMultipleItems'>
              <div class='post_labels uk-panel uk-margin-small'>
                <b:attr name='b:whitespace' value='remove'/>
                <span class='uk-margin-small-left' data-uk-icon='icon:tag;ratio:.7'/>
                <b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                  <b:if cond='data:i &lt; 2'>
                    <b:if cond='data:i &gt; 0'><span class='uk-margin-xsmall-left'>, </span></b:if>
                    <a expr:href='data:label.url' rel='tag'>#<data:label.name/></a>
                  </b:if>
                </b:loop>
              </div>
              <b:else/>
              <span class='post_labels uk-margin-left uk-margin-small-bottom'>
                <b:attr name='b:whitespace' value='remove'/>
                <span class='post_labels_label'>
                  <b:attr name='b:whitespace' value='remove'/>
                  <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
                  <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:tag;ratio:.75'/><data:byline.label/>
                </span>
                <b:loop index='i' values='data:post.labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                  <b:if cond='data:i &gt; 0'><span class='uk-margin-xsmall-left'>, </span></b:if>
                  <a expr:href='data:label.url' rel='tag'>#<data:label.name/></a>
                </b:loop>
              </span>
            </b:if>
          </b:if>
        </b:includable>
                            <b:includable id='postLocation'>
          <span class='post_location uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_location_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:location;ratio:.75'/><data:byline.label/>
            </span>
            <a expr:href='data:post.location.mapsUrl' target='_blank'><data:post.location.name/></a>
          </span>
        </b:includable>
                            <b:includable id='postMeta' var='post'>
  <b:include data='post' name='postMetadataJSON'/>
</b:includable>
                            <b:includable id='postMetaInfo' var='post'>
          <div class='post_meta uk-grid uk-grid-small'>
            <div class='post_date uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='icon: clock; ratio: .7'/><span><time class='published' expr:datetime='data:post.date.iso8601' expr:title='data:post.date.iso8601'><data:post.date/></time></span></div>
            <b:if cond='data:post.numberOfComments &gt; 0'>
              <div class='post_comments uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='icon: comment; ratio: .7'/><span><data:post.numberOfComments/></span></div>
            </b:if>
            <b:if cond='data:post.shareUrl'>
              <div class='post_share uk-width-auto'>
                <span class='action'><span class='uk-margin-small-left' data-uk-icon='icon: social; ratio: .7'/><span><data:messages.share/></span></span>
              </div>
            </b:if>
          </div>
        </b:includable>
                            <b:includable id='postPagination'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='postReactions'>
          <span class='post_reactions uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_reactions_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:happy;ratio:.75'/><data:byline.label/>
            </span>
            <iframe allowtransparency='true' class='reactions-iframe' expr:src='data:post.reactionsUrl' frameborder='0' name='reactions' scrolling='no'/>
          </span>
        </b:includable>
                            <b:includable id='postRelated' var='post'>
          <b:if cond='data:theme.relatedPosts.enable and data:view.isPost'>
            <div class='post_related uk-text-center' expr:data-count='data:theme.relatedPosts.maxResults' expr:data-id='data:post.id' expr:data-title='data:theme.relatedPosts.title'>
              <div data-uk-spinner=''/>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='postShareButtons'>
          <b:tag class='post_share uk-margin-left uk-margin-small-bottom' cond='data:view.isSingleItem' name='div'>
            <b:attr cond='data:view.isSingleItem' name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isSingleItem'>
              <span class='post_share_label'>
                <b:attr name='b:whitespace' value='remove'/>
                <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
                <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:social;ratio:.75'/><data:messages.share/>
              </span>
            </b:if>
            <ul class='post_share_buttons uk-iconnav uk-text-center'>
              <b:class cond='data:view.isMultipleItems' name='uk-iconnav uk-position-center uk-animation-toggle'/>
              <b:loop values='data:blog.sharing.platforms' var='platform'>
                <b:if cond='data:platform.key not in {&quot;link&quot;,&quot;blogThis&quot;,&quot;googlePlus&quot;,&quot;email&quot;}'>
                  <li><span data-uk-tooltip='pos:top' expr:class='&quot;icon_&quot; + data:platform.key + &quot; uk-icon-button&quot;' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:data-uk-icon='data:platform.key' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
                <b:if cond='data:platform.key == &quot;googlePlus&quot;'>
                  <li><span class='icon_google-plus uk-icon-button' data-uk-icon='google-plus' data-uk-tooltip='pos:top' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
                <b:if cond='data:post.emailPostUrl and data:platform.key == &quot;email&quot;'>
                  <li><span class='icon_reddit uk-icon-button' data-uk-icon='reddit' data-uk-tooltip='pos:top' expr:data-href='appendParams(&quot;https://www.reddit.com/submit&quot;, { url: data:post.url, title: data:post.title } )' expr:title='data:theme.text.shareTo + &quot; Reddit&quot;' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                  <li><span class='icon_mail uk-icon-button' data-uk-icon='mail' data-uk-tooltip='pos:top' expr:data-href='appendParams(data:post.shareUrl, { target: data:platform.target } )' expr:title='data:platform.shareMessage' role='button'/><b:class cond='data:view.isMultipleItems' name='uk-align-right uk-margin-remove'/></li>
                </b:if>
              </b:loop>
            </ul>
          </b:tag>
        </b:includable>
                            <b:includable id='postSnippet' var='post'>
          <div class='post_snippet entry-summary uk-position-relative'>
            <p expr:id='&quot;body&quot; + data:post.id'>
              <textarea><b:eval expr='data:post.body snippet { length: 150, links: false, linebreaks: false, ellipsis: false }'/></textarea>
              <script class='js'>var postId = &quot;<data:post.id/>&quot;, postLink = &quot;<data:post.url/>&quot;,readMore = &quot;<data:messages.readMore/>&quot;;/*<![CDATA[*/eval(function(n,e,r,t,i,o){if(i=function(n){return n.toString(27)},!$salA[5][$salA[4]](/^/,String)){for(;r--;)o[i(r)]=t[r]||i(r);t=[function(n){return o[n]}],i=function(){return $salA[6]},r=1}for(;r--;)t[r]&&(n=n[$salA[4]](new RegExp($salA[7]+i(r)+$salA[7],$salA[8]),t[r]));return n}($salA[0],0,27,$salA[3][$salA[2]]($salA[1]),0,{}));//]]></script>
            </p>
            <b:include cond='data:post.shareUrl' data='post' name='postShareButtons'/>
          </div>
        </b:includable>
                            <b:includable id='postThumbnail'>
          <b:if cond='data:post.featuredImage'>
            <div class='post_thumbnail uk-card-media-top uk-text-center uk-position-relative uk-transition-toggle' expr:data-title='data:post.title'>
              <a expr:href='data:post.url'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <b:include data='{ image: data:post.featuredImage, imageSizes: [480], imageRatio: &quot;16:9&quot;, sourceSizes: &quot;480px&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                  <b:else/>
                  <b:if cond='data:theme.layout.enableImagesAutoHeight'>
                    <b:include data='{ image: data:post.featuredImage, imageSizes: [345,285,330,510], sourceSizes: &quot;(min-width: 1200px) 345px, (min-width: 992px) 285px, (min-width: 768px) 330px, (min-width: 576px) 510px, calc(100vw - 30px)&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                    <b:else/>
                    <b:include data='{ image: data:post.featuredImage, imageSizes: [345,285,330,510], imageRatio: &quot;16:9&quot;, sourceSizes: &quot;(min-width: 1200px) 345px, (min-width: 992px) 285px, (min-width: 768px) 330px, (min-width: 576px) 510px, calc(100vw - 30px)&quot;, enhancedSourceset: data:highRes }' name='responsiveImage'/>
                  </b:if>
                </b:if>
                <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
                <div class='uk-position-center'>
                  <b:if cond='data:post.featuredImage.isYoutube'>
                    <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:2.3'/>
                    <b:else/>
                    <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:2.3'/>
                  </b:if>
                </div>
              </a>
            </div>
          </b:if>
        </b:includable>
                            <b:includable id='postTimestamp'>
          <span class='post_timestamp uk-margin-left uk-margin-small-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <span class='post_timestamp_label'>
              <b:attr name='b:whitespace' value='remove'/>
              <b:class cond='data:byline.label != &quot;&quot;' name='uk-margin-xsmall-left'/>
              <span class='uk-icon uk-margin-small-left' data-uk-icon='icon:clock;ratio:.75'/><data:byline.label/>
            </span>
            <b:if cond='data:post.url'>
              <meta expr:content='data:post.url.canonical'/>
              <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'>
                <b:attr name='b:whitespace' value='remove'/>
                <time class='published' expr:datetime='data:post.date.iso8601' expr:title='data:post.date.iso8601'><data:post.date/></time>
              </a>
            </b:if>
          </span>
        </b:includable>
                            <b:includable id='postTitle' var='post'>
          <b:if cond='data:post.title != &quot;&quot;'>
            <b:if cond='data:view.isMultipleItems'>
              <h2 class='post_title entry-title uk-margin'>
                <b:if cond='data:post.link or (data:post.url and data:view.url != data:post.url)'>
                  <a expr:href='data:post.link ?: data:post.url' rel='bookmark'><data:post.title/></a>
                  <b:else/>
                  <data:post.title/>
                </b:if>
              </h2>
              <b:else/>
              <h1 class='post_title entry-title uk-article-title'><data:post.title/></h1>
            </b:if>
          </b:if>
        </b:includable>
                            <b:includable id='previousPageLink'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='threadedCommentForm'><b:comment>Removed</b:comment></b:includable>
                            <b:includable id='threadedCommentJs' var='post'>
          <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>
          <b:template-script inline='true' name='threaded_comments'/>
          <script type='text/javascript'>
            blogger.widgets.blog.initThreadedComments(
              <data:post.commentJso/>,
              <data:post.commentMsgs/>,
              <data:post.commentConfig/>);
          </script>
        </b:includable>
                            <b:includable id='threadedComments' var='post'>
          <b:class cond='!data:post.allowNewComments' name='comments_locked'/>
          <b:include cond='data:post.embedCommentForm' data='post' name='threadedCommentJs'/>
          <div class='post_comments_holder' id='comment-holder'>
            <data:post.commentHtml/>
            <script class='js'>/*<![CDATA[*/eval(function(e,n,r,t,a,i){if(a=function(e){return(e<43?$salC[4]:a(parseInt(e/43)))+(35<(e%=43)?String[$salC[5]](e+29):e.toString(36))},!$salC[4][$salC[6]](/^/,String)){for(;r--;)i[a(r)]=t[r]||a(r);t=[function(e){return i[e]}],a=function(){return $salC[7]},r=1}for(;r--;)t[r]&&(e=e[$salC[6]](new RegExp($salC[8]+a(r)+$salC[8],$salC[9]),t[r]));return e}($salC[0],0,43,$salC[3][$salC[2]]($salC[1]),0,{}));//]]></script>
          </div>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
            <b:else/>
            <div class='post_comments_locked uk-margin-top uk-text-danger'>
              <span class='uk-margin-small-left' data-uk-icon='ban'/><span><data:post.noNewCommentsText/></span>
            </div>
          </b:if>
          <b:if cond='data:showCmtPopup'>
            <div id='comment-popup'>
              <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'/>
            </div>
          </b:if>
        </b:includable>
                          </b:widget>
                        </b:section>
                      </b:tag>

                      <b:comment expr:render='data:enableIndexSidebar or data:enablePagesSidebar'> .sidebar </b:comment>
                      <b:section class='sidebar uk-width-1-3@l' cond='data:enableIndexSidebar or data:enablePagesSidebar' id='sidebar'>
                        <b:widget id='HTML3' locked='false' title='' type='HTML' visible='true'>
                          <b:widget-settings>
                            <b:widget-setting name='content'><![CDATA[<div style="max-width: 100%; margin: 0 auto; background: #f9f9f9; border: 1px dashed #e5e5e5; line-height: 250px; text-align: center; width: 300px; height: 250px; font-size: 14px;">إعلان 300 - 250</div>]]></b:widget-setting>
                          </b:widget-settings>
                          <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
                        </b:widget>
                        <b:widget id='FeaturedPost1' locked='false' title='موضوع مميز' type='FeaturedPost' visible='true'>
                          <b:widget-settings>
                            <b:widget-setting name='showSnippet'>true</b:widget-setting>
                            <b:widget-setting name='showPostTitle'>true</b:widget-setting>
                            <b:widget-setting name='postId'>3196389984615535120</b:widget-setting>
                            <b:widget-setting name='showFirstImage'>true</b:widget-setting>
                            <b:widget-setting name='useMostRecentPost'>false</b:widget-setting>
                          </b:widget-settings>
                          <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <div class='widget-content'>
    <b:include name='snippetedPosts'/>
  </div>
</b:includable>
                          <b:includable id='postSnippet'>
          <div class='item-snippet'><b:eval expr='data:post.snippets.short snippet { length: 80, links: false, linebreaks: false, ellipsis: true }'/></div>
        </b:includable>
                          <b:includable id='snippetedPostContent'>
          <div class='item-content'>
            <b:include cond='data:postDisplay.showFeaturedImage and data:post.featuredImage' name='snippetedPostThumbnail'/>
            <b:include cond='data:widget.type == &quot;FeaturedPost&quot; ? data:postDisplay.showTitle : true' name='snippetedPostTitle'/>
            <b:include cond='data:postDisplay.showSnippet' name='postSnippet'/>
          </div>
        </b:includable>
                          <b:includable id='snippetedPostThumbnail'>
          <div class='item-thumbnail uk-text-center uk-position-relative uk-transition-toggle'>
            <a expr:href='data:post.url'>
              <img alt='Image' expr:src='resizeImage(data:post.featuredImage,360,&quot;16:9&quot;)'/>
              <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
              <div class='uk-position-center'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:2.3'/>
                  <b:else/>
                  <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:2.3'/>
                </b:if>
              </div>
            </a>
          </div>
        </b:includable>
                          <b:includable id='snippetedPostTitle'>
          <div class='item-title'>
            <a expr:href='data:post.url'><data:post.title/></a>
          </div>
        </b:includable>
                          <b:includable id='snippetedPosts'>
          <ul>
            <b:loop values='data:posts' var='post'>
              <li>
                <b:include name='snippetedPostContent'/>
              </li>
            </b:loop>
          </ul>
        </b:includable>
                        </b:widget>
                        <b:widget id='Label3' locked='false' title='التسميات' type='Label' visible='true'>
                          <b:widget-settings>
                            <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                            <b:widget-setting name='display'>CLOUD</b:widget-setting>
                            <b:widget-setting name='selectedLabelsList'/>
                            <b:widget-setting name='showType'>ALL</b:widget-setting>
                            <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
                          </b:widget-settings>
                          <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                          <b:includable id='cloud'>
          <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
            <a class='label-name uk-button uk-button-default uk-button-small uk-margin-small-left uk-margin-small-bottom' expr:href='data:label.url'>
              <b:class expr:name='&quot;label-size-&quot; + data:label.cssSize'/>
              <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-margin-small-right'>_<data:label.count/></span></b:if>
            </a>
          </b:loop>
        </b:includable>
                          <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;main&quot;'>
            <b:include name='filter'/>
            <b:else/>
            <div class='widget-content'>
              <b:class expr:name='data:this.display + &quot;-label-widget-content&quot;'/>
              <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
              <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
            </div>
          </b:if>
        </b:includable>
                          <b:includable id='filter'>
          <div class='filtering_labels uk-grid uk-margin-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isHomepage'>
              <div class='select_label uk-width-expand@m'>
                <b:if cond='data:theme.layout.enableFilterOption'>
                  <script class='js'>
                    var filterTags = Object.values({<b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
                  </script>
                  <ul class='uk-list uk-list-inline uk-visible@l'>
                    <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='settings'/><span><data:theme.text.filter/></span></span></li>
                    <li><a class='uk-button uk-button-default uk-margin-bottom uk-active' data-uk-filter-control='' href='#!'><data:messages.viewAll/></a></li>
                    <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                      <li><a class='uk-button uk-button-default uk-margin-bottom' expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' href='#!'><data:label.name/></a></li>
                    </b:loop>
                  </ul>
                  <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                    <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='settings'/></div>
                    <div class='uk-width-auto@m uk-width-expand'>
                      <select class='uk-select'>
                        <option data-uk-filter-control='' value=''><data:messages.viewAll/></option>
                        <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                          <option expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' expr:value='&quot;.filter_&quot; + data:i'><data:label.name/></option>
                        </b:loop>
                      </select>
                    </div>
                  </div>
                </b:if>
              </div>
            </b:if>
            <b:if cond='data:view.isMultipleItems and !data:view.isHomepage'>
              <div class='breadcrumb uk-width-expand@m'>
                <ul class='uk-breadcrumb'>
                  <li><a href='/'><data:messages.home/></a></li>
                  <b:if cond='data:view.isSearch'>
                    <li><a href='/search'><data:messages.search/></a></li>
                    <b:if cond='data:view.isLabelSearch'>
                      <li class='uk-disabled'><span><data:messages.labels/></span></li>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                      <b:elseif cond='data:view.search.query'/>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                    </b:if>
                  </b:if>
                  <b:if cond='data:view.isArchive'>
                    <li class='uk-disabled'><span><data:messages.archive/></span></li>
                    <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                  </b:if>
                </ul>
              </div>
            </b:if>
            <b:if cond='data:theme.layout.enableViewOption'>
              <div class='select_view uk-width-exapnd uk-width-auto@m'>
                <b:class cond='!data:theme.layout.enableFilterOption' name='uk-margin-bottom'/>
                <ul class='uk-list uk-list-inline uk-visible@l'>
                  <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='cog'/><span><data:theme.text.view/></span></span></li>
                  <li class='uk-active'><a class='uk-icon-button' data-uk-icon='expand' data-uk-tooltip='pos:top' expr:title='data:theme.text.expandPosts' href='#!' id='view_e'/></li>
                  <li><a class='uk-icon-button' data-uk-icon='shrink' data-uk-tooltip='pos:top' expr:title='data:theme.text.shrinkPosts' href='#!' id='view_s'/></li>
                </ul>
                <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                  <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='cog'/></div>
                  <div class='uk-width-auto@m uk-width-expand'>
                    <select class='uk-select'>
                      <option value='expand'><data:theme.text.expandPosts/></option>
                      <option value='shrink'><data:theme.text.shrinkPosts/></option>
                    </select>
                  </div>
                </div>
                <script class='js'>/*<![CDATA[*/eval(function(e,c,r,t,d,i){if(d=function(e){return e.toString(16)},!$salD[5][$salD[4]](/^/,String)){for(;r--;)i[d(r)]=t[r]||d(r);t=[function(e){return i[e]}],d=function(){return $salD[6]},r=1}for(;r--;)t[r]&&(e=e[$salD[4]](new RegExp($salD[7]+d(r)+$salD[7],$salD[8]),t[r]));return e}($salD[0],0,16,$salD[3][$salD[2]]($salD[1]),0,{}));//]]></script>
              </div>
            </b:if>
          </div>
        </b:includable>
                          <b:includable id='list'>
          <ul class='uk-list uk-list-bullet uk-margin-remove'>
            <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
              <li>
                <a class='label-name' expr:href='data:label.url'>
                  <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-align-left uk-margin-remove'><data:label.count/></span></b:if>
                </a>
              </li>
            </b:loop>
          </ul>
        </b:includable>
                        </b:widget>
                        <b:widget id='PopularPosts1' locked='false' title='المواضيع الأكثر زيارة' type='PopularPosts' visible='true'>
                          <b:widget-settings>
                            <b:widget-setting name='numItemsToShow'>10</b:widget-setting>
                            <b:widget-setting name='showThumbnails'>true</b:widget-setting>
                            <b:widget-setting name='showSnippets'>true</b:widget-setting>
                            <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
                          </b:widget-settings>
                          <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <div class='widget-content'>
    <b:include name='snippetedPosts'/>
  </div>
</b:includable>
                          <b:includable id='postSnippet'>
          <div class='item-snippet'><b:eval expr='data:post.snippets.short snippet { length: 80, links: false, linebreaks: false, ellipsis: true }'/></div>
        </b:includable>
                          <b:includable id='snippetedPostContent'>
          <div class='item-content'>
            <b:include cond='data:postDisplay.showFeaturedImage and data:post.featuredImage' name='snippetedPostThumbnail'/>
            <b:include cond='data:widget.type == &quot;FeaturedPost&quot; ? data:postDisplay.showTitle : true' name='snippetedPostTitle'/>
            <b:include cond='data:postDisplay.showSnippet' name='postSnippet'/>
          </div>
        </b:includable>
                          <b:includable id='snippetedPostThumbnail'>
          <b:class name='uk-transition-toggle'/>
          <div class='item-thumbnail uk-text-center'>
            <a class='uk-position-relative uk-overflow-hidden' expr:href='data:post.url'>
              <img alt='Image' expr:src='resizeImage(data:post.featuredImage,72,&quot;1:1&quot;)'/>
              <div class='uk-position-cover uk-transition-fade uk-overlay-primary'/>
              <div class='uk-position-center'>
                <b:if cond='data:post.featuredImage.isYoutube'>
                  <span class='uk-transition-fade' data-uk-icon='icon:play-circle;ratio:1.5'/>
                  <b:else/>
                  <span class='uk-transition-fade' data-uk-icon='icon:image;ratio:1.5'/>
                </b:if>
              </div>
            </a>
          </div>
        </b:includable>
                          <b:includable id='snippetedPostTitle'>
          <div class='item-title'>
            <a expr:href='data:post.url'><data:post.title/></a>
          </div>
        </b:includable>
                          <b:includable id='snippetedPosts'>
          <ul>
            <b:loop values='data:posts' var='post'>
              <li>
                <b:include name='snippetedPostContent'/>
              </li>
            </b:loop>
          </ul>
        </b:includable>
                        </b:widget>
                        <b:widget id='HTML4' locked='false' title='' type='HTML' visible='true'>
                          <b:widget-settings>
                            <b:widget-setting name='content'><![CDATA[<div style="max-width: 100%; margin: 0 auto; background: #f9f9f9; border: 1px dashed #e5e5e5; line-height: 250px; text-align: center; width: 300px; height: 600px; font-size: 14px;">إعلان 300 - 600</div>]]></b:widget-setting>
                          </b:widget-settings>
                          <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
                        </b:widget>
                      </b:section>

                    </b:tag>
                  </b:with>
                </b:with>
              </b:with>
            </b:if>

            <b:if cond='data:view.isError'>
              <!-- .error -->
              <div class='error uk-width-1-1' id='error'>
                <div class='error_content uk-text-center'>
                  <h2 class='uk-flex@m uk-flex-middle@m uk-flex-center@m'>
                    <span><data:theme.errorPage.header1st/></span>
                    <span class='uk-margin-right' data-uk-icon='icon:bolt;ratio:2'/>
                    <span class='uk-margin-right'><data:theme.errorPage.header2nd/></span>
                  </h2>
                  <p><data:theme.errorPage.message/></p>
                  <div class='error_search uk-margin-xmedium-top'>
                    <form expr:action='data:blog.searchUrl'>
                      <b:attr cond='not data:view.isPreview' name='target' value='_top'/>
                      <b:include name='urlParamsAsFormInput'/>
                      <div class='search-input uk-width-1-1 uk-inline'>
                        <button class='search-action uk-form-icon uk-form-icon-flip' data-uk-icon='search' type='submit'/>
                        <input autocomplete='off' class='uk-input' expr:aria-label='data:messages.searchThisBlog' expr:placeholder='data:messages.searchThisBlog' expr:value='data:view.isSearch ? data:view.search.query.escaped : &quot;&quot;' name='q' type='text'/>
                      </div>
                    </form>
                  </div>
                </div>
                <b:if cond='data:theme.errorPage.enableFeaturedPosts'>
                  <div class='post_related uk-margin-large-top uk-text-center' expr:data-count='data:theme.errorPage.featuredPostsMaxResults'>
                    <div data-uk-spinner=''/>
                  </div>
                </b:if>
              </div>
            </b:if>

          </div>

          <b:if cond='data:theme.layout.enableWavyStyle'>
            <!-- .bottom_bg -->
            <div class='bottom_bg'>
              <b:include data='{ id: &quot;fill_2&quot;, isHeader: false }' name='background-svg'/>
            </div>
          </b:if>

        </main>

        <!-- footer -->
        <footer>
          <div class='uk-container'>

            <!-- .topgrid -->
            <div class='topgrid uk-grid'>
              <b:section class='topgrid_section uk-width-1-2@m uk-width-1-5@l' id='footer_section_1'>
                <b:widget id='Image1' locked='false' title='' type='Image' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='displayUrl'>http://3.bp.blogspot.com/-ITuTeV_Q4BQ/W0uW11uCWuI/AAAAAAAAGLs/iogjYPUO9ekF70lHB1CiLLFuEEe2v2PywCK4BGAYYCw/s1600/logo_icon.png</b:widget-setting>
                    <b:widget-setting name='displayHeight'>192</b:widget-setting>
                    <b:widget-setting name='sectionWidth'>150</b:widget-setting>
                    <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                    <b:widget-setting name='displayWidth'>162</b:widget-setting>
                    <b:widget-setting name='link'>/</b:widget-setting>
                    <b:widget-setting name='caption'/>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <div class='widget-content'>
            <b:tag cond='data:link' expr:href='data:link' name='a'>
              <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl' expr:width='data:width'/>
            </b:tag>
            <br/>
            <b:if cond='data:caption'>
              <span class='caption'><data:caption/></span>
            </b:if>
          </div>
        </b:includable>
                </b:widget>
              </b:section>
              <b:section class='topgrid_section uk-width-1-2@m uk-width-expand@l' id='footer_section_2'>
                <b:widget id='LinkList2' locked='false' title='عناصر مفيدة' type='LinkList' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='link-5'>#!</b:widget-setting>
                    <b:widget-setting name='link-3'>#!</b:widget-setting>
                    <b:widget-setting name='link-4'>#!</b:widget-setting>
                    <b:widget-setting name='text-1'>الخصوصية</b:widget-setting>
                    <b:widget-setting name='text-0'>المصادر</b:widget-setting>
                    <b:widget-setting name='text-3'>الشروط</b:widget-setting>
                    <b:widget-setting name='text-2'>المجتمع</b:widget-setting>
                    <b:widget-setting name='text-5'>اتصل بنا</b:widget-setting>
                    <b:widget-setting name='text-4'>المساعدة</b:widget-setting>
                    <b:widget-setting name='sorting'>NONE</b:widget-setting>
                    <b:widget-setting name='link-1'>#!</b:widget-setting>
                    <b:widget-setting name='link-2'>#!</b:widget-setting>
                    <b:widget-setting name='link-0'>#!</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;topnav&quot;'>
            <div class='uk-grid' data-uk-grid=''>
              <div class='sidenav_button uk-width-auto uk-margin-remove'>
                <a class='uk-button' data-uk-toggle='target:#sidenav' href='#!'>
                  <b:class expr:name='data:theme.layout.enableLightStyle ? &quot;uk-button-primary&quot; : &quot;uk-button-default&quot;'/>
                  <span data-uk-icon='thumbnails'/>
                  <span class='uk-margin-small-right'><data:theme.text.sideMenu/></span>
                </a>
              </div>
              <div class='topnav_social_wrapper uk-width-expand uk-margin-remove'>
                <div class='uk-align-left uk-margin-remove'>
                  <ul class='topnav_social uk-iconnav'>
                    <b:loop index='i' values='data:links' var='link'>
                      <li><a data-uk-tooltip='pos:bottom' expr:class='&quot;uk-icon-button icon_&quot; + data:link.name' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
                    </b:loop>
                  </ul>
                </div>
              </div>
            </div>
          </b:if>
          <b:if cond='data:widget.sectionId == &quot;social&quot;'>
            <ul class='social_social uk-iconnav'>
              <b:loop index='i' values='data:links' var='link'>
                  <li><a data-uk-tooltip='pos:top' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
              </b:loop>
            </ul>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;social&quot;,&quot;topnav&quot;}'>
            <div class='widget-content'>
              <b:class cond='!data:theme.layout.enableLightStyle and data:widget.sectionId in {&quot;footer_section_1&quot;,&quot;footer_section_2&quot;,&quot;footer_section_3&quot;,&quot;footer_section_4&quot;}' name='uk-light'/>
              <ul class='uk-list uk-list-bullet uk-margin-remove'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:href='data:link.target'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
              <b:section class='topgrid_section uk-width-1-2@m uk-width-expand@l' id='footer_section_3'>
                <b:widget id='LinkList3' locked='false' title='مصادر خارجية' type='LinkList' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='sorting'>NONE</b:widget-setting>
                    <b:widget-setting name='text-1'>Emma Leonil | Fiverr</b:widget-setting>
                    <b:widget-setting name='link-1'>https://www.fiverr.com/emmaleonil</b:widget-setting>
                    <b:widget-setting name='text-0'>ar-themes</b:widget-setting>
                    <b:widget-setting name='link-2'>https:///user/elyza/portfolio?ref=Elyza</b:widget-setting>
                    <b:widget-setting name='link-0'>https://ar-themes.blogspot.com/</b:widget-setting>
                    <b:widget-setting name='text-2'>Elyza | Androidlamine </b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;topnav&quot;'>
            <div class='uk-grid' data-uk-grid=''>
              <div class='sidenav_button uk-width-auto uk-margin-remove'>
                <a class='uk-button' data-uk-toggle='target:#sidenav' href='#!'>
                  <b:class expr:name='data:theme.layout.enableLightStyle ? &quot;uk-button-primary&quot; : &quot;uk-button-default&quot;'/>
                  <span data-uk-icon='thumbnails'/>
                  <span class='uk-margin-small-right'><data:theme.text.sideMenu/></span>
                </a>
              </div>
              <div class='topnav_social_wrapper uk-width-expand uk-margin-remove'>
                <div class='uk-align-left uk-margin-remove'>
                  <ul class='topnav_social uk-iconnav'>
                    <b:loop index='i' values='data:links' var='link'>
                      <li><a data-uk-tooltip='pos:bottom' expr:class='&quot;uk-icon-button icon_&quot; + data:link.name' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
                    </b:loop>
                  </ul>
                </div>
              </div>
            </div>
          </b:if>
          <b:if cond='data:widget.sectionId == &quot;social&quot;'>
            <ul class='social_social uk-iconnav'>
              <b:loop index='i' values='data:links' var='link'>
                  <li><a data-uk-tooltip='pos:top' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
              </b:loop>
            </ul>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;social&quot;,&quot;topnav&quot;}'>
            <div class='widget-content'>
              <b:class cond='!data:theme.layout.enableLightStyle and data:widget.sectionId in {&quot;footer_section_1&quot;,&quot;footer_section_2&quot;,&quot;footer_section_3&quot;,&quot;footer_section_4&quot;}' name='uk-light'/>
              <ul class='uk-list uk-list-bullet uk-margin-remove'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:href='data:link.target'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
              <b:section class='topgrid_section uk-width-1-2@m uk-width-1-3@l' id='footer_section_4'>
                <b:widget id='FollowByEmail1' locked='false' title='إشترك' type='FollowByEmail' visible='true'>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <div class='widget-content'>
            <div class='follow-by-email-inner'>
              <form action='https://feedburner.google.com/fb/a/mailverify' expr:onsubmit='&quot;window.open(\&quot;https://feedburner.google.com/fb/a/mailverify?uri=&quot; + data:feedPath + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' target='popupwindow'>
                <div class='uk-grid uk-grid-small uk-margin-bottom'>
                  <span class='uk-width-auto' data-uk-icon='icon:mail;ratio:2'/>
                  <span class='uk-width-expand'><data:theme.text.followByEmailMessage/></span>
                </div>
                <div class='search-input uk-width-1-1 uk-inline'>
                  <button class='search-action uk-form-icon uk-form-icon-flip' data-uk-icon='forward' type='submit'/>
                  <input autocomplete='off' class='follow-by-email-address uk-input' expr:placeholder='data:messages.emailAddress' name='email' type='email'/>
                </div>
                <input expr:value='data:feedPath' name='uri' type='hidden'/>
                <input name='loc' type='hidden' value='en_US'/>
              </form>
            </div>
          </div>
        </b:includable>
                </b:widget>
                <b:widget id='Image2' locked='false' title='' type='Image' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='displayUrl'>https://1.bp.blogspot.com/-jYMKUjYB5lQ/V7wI6kEMQnI/AAAAAAAAEPg/ujTYAKjaDYE7svCV1hvm-QKH21kCuqzxACK4B/s1600/ar-themes_logo.png</b:widget-setting>
                    <b:widget-setting name='displayHeight'>35</b:widget-setting>
                    <b:widget-setting name='sectionWidth'>767</b:widget-setting>
                    <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                    <b:widget-setting name='displayWidth'>175</b:widget-setting>
                    <b:widget-setting name='link'>https://ar-themes.blogspot.com</b:widget-setting>
                    <b:widget-setting name='caption'/>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <div class='widget-content'>
            <b:tag cond='data:link' expr:href='data:link' name='a'>
              <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl' expr:width='data:width'/>
            </b:tag>
            <br/>
            <b:if cond='data:caption'>
              <span class='caption'><data:caption/></span>
            </b:if>
          </div>
        </b:includable>
                </b:widget>
                <b:widget id='HTML5' locked='false' title='' type='HTML' visible='true'>
                  <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
            </div>

            <!-- .maingrid -->
            <div class='maingrid uk-grid uk-margin-xlarge-top'>
              <b:section class='copyrights uk-width-expand@m' id='copyrights' maxwidgets='1'>
                <b:widget id='HTML2' locked='true' title='معلومات حقوق الملكية' type='HTML' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='content'><![CDATA[جميع الحقوق محفوظة © 2019 <a href="https://www.star4tips.com">Star4Tips</a>]]></b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
          <b:if cond='data:widget.sectionId in {&quot;theme_options&quot;}'>
            &lt;script&gt;<data:content/>&lt;/script&gt;
          </b:if>
          <b:if cond='data:widget.sectionId in {&quot;mainnav&quot;}'>
            <b:class name='uk-margin-remove uk-width-expand'/>
            <nav class='mainnav_menu uk-navbar-container uk-align-left uk-margin-remove' data-uk-navbar='delay-hide:400;align:right;mode:click'>
              <ul class='uk-navbar-nav'>
                <data:content/>
                <li>
                  <a class='icon_search uk-navbar-toggle' data-uk-icon='search' data-uk-toggle='pos:bottom' data-uk-tooltip='pos:bottom' expr:title='data:messages.search' href='#search_modal'/>
                </li>
              </ul>
            </nav>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;theme_options&quot;,&quot;mainnav&quot;}'>
            <b:include name='widget-title'/>
            <div class='widget-content'><data:content/></div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
              <b:section class='social uk-width-auto@m' id='social' maxwidgets='1'>
                <b:widget id='LinkList4' locked='true' title='أيقونات التواصل الإجتماعي السفلى' type='LinkList' visible='true'>
                  <b:widget-settings>
                    <b:widget-setting name='link-5'>#!</b:widget-setting>
                    <b:widget-setting name='link-3'>#!</b:widget-setting>
                    <b:widget-setting name='link-4'>#!</b:widget-setting>
                    <b:widget-setting name='text-1'>vimeo</b:widget-setting>
                    <b:widget-setting name='text-0'>youtube</b:widget-setting>
                    <b:widget-setting name='text-3'>linkedin</b:widget-setting>
                    <b:widget-setting name='text-2'>tumblr</b:widget-setting>
                    <b:widget-setting name='text-5'>whatsapp</b:widget-setting>
                    <b:widget-setting name='text-4'>flickr</b:widget-setting>
                    <b:widget-setting name='sorting'>NONE</b:widget-setting>
                    <b:widget-setting name='link-1'>#!</b:widget-setting>
                    <b:widget-setting name='link-2'>#!</b:widget-setting>
                    <b:widget-setting name='link-0'>#!</b:widget-setting>
                  </b:widget-settings>
                  <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
                  <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;topnav&quot;'>
            <div class='uk-grid' data-uk-grid=''>
              <div class='sidenav_button uk-width-auto uk-margin-remove'>
                <a class='uk-button' data-uk-toggle='target:#sidenav' href='#!'>
                  <b:class expr:name='data:theme.layout.enableLightStyle ? &quot;uk-button-primary&quot; : &quot;uk-button-default&quot;'/>
                  <span data-uk-icon='thumbnails'/>
                  <span class='uk-margin-small-right'><data:theme.text.sideMenu/></span>
                </a>
              </div>
              <div class='topnav_social_wrapper uk-width-expand uk-margin-remove'>
                <div class='uk-align-left uk-margin-remove'>
                  <ul class='topnav_social uk-iconnav'>
                    <b:loop index='i' values='data:links' var='link'>
                      <li><a data-uk-tooltip='pos:bottom' expr:class='&quot;uk-icon-button icon_&quot; + data:link.name' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
                    </b:loop>
                  </ul>
                </div>
              </div>
            </div>
          </b:if>
          <b:if cond='data:widget.sectionId == &quot;social&quot;'>
            <ul class='social_social uk-iconnav'>
              <b:loop index='i' values='data:links' var='link'>
                  <li><a data-uk-tooltip='pos:top' expr:data-uk-icon='data:link.name' expr:href='data:link.target' expr:title='data:theme.text.followOn + &quot; &quot; + data:link.name' target='_blank'/></li>
              </b:loop>
            </ul>
          </b:if>
          <b:if cond='data:widget.sectionId not in {&quot;social&quot;,&quot;topnav&quot;}'>
            <div class='widget-content'>
              <b:class cond='!data:theme.layout.enableLightStyle and data:widget.sectionId in {&quot;footer_section_1&quot;,&quot;footer_section_2&quot;,&quot;footer_section_3&quot;,&quot;footer_section_4&quot;}' name='uk-light'/>
              <ul class='uk-list uk-list-bullet uk-margin-remove'>
                <b:loop values='data:links' var='link'>
                  <li><a expr:href='data:link.target'><data:link.name/></a></li>
                </b:loop>
              </ul>
            </div>
          </b:if>
        </b:includable>
                </b:widget>
              </b:section>
            </div>

          </div>
        </footer>

      </div>

      <!-- .sidenav -->
      <div class='sidenav' data-uk-offcanvas='overlay:true' id='sidenav'>
        <b:class expr:cond='!data:theme.layout.enableLightStyle' name='uk-light'/>
        <div class='uk-offcanvas-bar uk-padding-remove'>
          <b:class expr:cond='!data:theme.layout.enableLightStyle' name='uk-background-secondary'/>
          <button class='uk-icon-button uk-offcanvas-close' data-uk-close=''/>
          <b:section class='sidenav_section uk-padding' id='sidenav_section'>
            <b:widget id='Label2' locked='false' title='التسميات' type='Label' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                <b:widget-setting name='display'>CLOUD</b:widget-setting>
                <b:widget-setting name='selectedLabelsList'/>
                <b:widget-setting name='showType'>ALL</b:widget-setting>
                <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main' var='this'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
              <b:includable id='cloud'>
          <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
            <a class='label-name uk-button uk-button-default uk-button-small uk-margin-small-left uk-margin-small-bottom' expr:href='data:label.url'>
              <b:class expr:name='&quot;label-size-&quot; + data:label.cssSize'/>
              <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-margin-small-right'>_<data:label.count/></span></b:if>
            </a>
          </b:loop>
        </b:includable>
              <b:includable id='content'>
          <b:if cond='data:widget.sectionId == &quot;main&quot;'>
            <b:include name='filter'/>
            <b:else/>
            <div class='widget-content'>
              <b:class expr:name='data:this.display + &quot;-label-widget-content&quot;'/>
              <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
              <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
            </div>
          </b:if>
        </b:includable>
              <b:includable id='filter'>
          <div class='filtering_labels uk-grid uk-margin-bottom'>
            <b:attr name='b:whitespace' value='remove'/>
            <b:if cond='data:view.isHomepage'>
              <div class='select_label uk-width-expand@m'>
                <b:if cond='data:theme.layout.enableFilterOption'>
                  <script class='js'>
                    var filterTags = Object.values({<b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'><data:i/>: encodeURIComponent(&quot;<data:label.name/>&quot;),</b:loop>});
                  </script>
                  <ul class='uk-list uk-list-inline uk-visible@l'>
                    <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='settings'/><span><data:theme.text.filter/></span></span></li>
                    <li><a class='uk-button uk-button-default uk-margin-bottom uk-active' data-uk-filter-control='' href='#!'><data:messages.viewAll/></a></li>
                    <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                      <li><a class='uk-button uk-button-default uk-margin-bottom' expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' href='#!'><data:label.name/></a></li>
                    </b:loop>
                  </ul>
                  <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                    <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='settings'/></div>
                    <div class='uk-width-auto@m uk-width-expand'>
                      <select class='uk-select'>
                        <option data-uk-filter-control='' value=''><data:messages.viewAll/></option>
                        <b:loop index='i' values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
                          <option expr:data-uk-filter-control='&quot;.filter_&quot; + data:i' expr:value='&quot;.filter_&quot; + data:i'><data:label.name/></option>
                        </b:loop>
                      </select>
                    </div>
                  </div>
                </b:if>
              </div>
            </b:if>
            <b:if cond='data:view.isMultipleItems and !data:view.isHomepage'>
              <div class='breadcrumb uk-width-expand@m'>
                <ul class='uk-breadcrumb'>
                  <li><a href='/'><data:messages.home/></a></li>
                  <b:if cond='data:view.isSearch'>
                    <li><a href='/search'><data:messages.search/></a></li>
                    <b:if cond='data:view.isLabelSearch'>
                      <li class='uk-disabled'><span><data:messages.labels/></span></li>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                      <b:elseif cond='data:view.search.query'/>
                      <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                    </b:if>
                  </b:if>
                  <b:if cond='data:view.isArchive'>
                    <li class='uk-disabled'><span><data:messages.archive/></span></li>
                    <li class='uk-disabled'><span><data:blog.pageName/></span></li>
                  </b:if>
                </ul>
              </div>
            </b:if>
            <b:if cond='data:theme.layout.enableViewOption'>
              <div class='select_view uk-width-exapnd uk-width-auto@m'>
                <b:class cond='!data:theme.layout.enableFilterOption' name='uk-margin-bottom'/>
                <ul class='uk-list uk-list-inline uk-visible@l'>
                  <li><span class='mark uk-button'><span class='uk-margin-small-left' data-uk-icon='cog'/><span><data:theme.text.view/></span></span></li>
                  <li class='uk-active'><a class='uk-icon-button' data-uk-icon='expand' data-uk-tooltip='pos:top' expr:title='data:theme.text.expandPosts' href='#!' id='view_e'/></li>
                  <li><a class='uk-icon-button' data-uk-icon='shrink' data-uk-tooltip='pos:top' expr:title='data:theme.text.shrinkPosts' href='#!' id='view_s'/></li>
                </ul>
                <div class='uk-grid-small uk-hidden@l' data-uk-grid=''>
                  <div class='uk-width-auto'><span class='uk-margin-small-left' data-uk-icon='cog'/></div>
                  <div class='uk-width-auto@m uk-width-expand'>
                    <select class='uk-select'>
                      <option value='expand'><data:theme.text.expandPosts/></option>
                      <option value='shrink'><data:theme.text.shrinkPosts/></option>
                    </select>
                  </div>
                </div>
                <script class='js'>/*<![CDATA[*/eval(function(e,c,r,t,d,i){if(d=function(e){return e.toString(16)},!$salD[5][$salD[4]](/^/,String)){for(;r--;)i[d(r)]=t[r]||d(r);t=[function(e){return i[e]}],d=function(){return $salD[6]},r=1}for(;r--;)t[r]&&(e=e[$salD[4]](new RegExp($salD[7]+d(r)+$salD[7],$salD[8]),t[r]));return e}($salD[0],0,16,$salD[3][$salD[2]]($salD[1]),0,{}));//]]></script>
              </div>
            </b:if>
          </div>
        </b:includable>
              <b:includable id='list'>
          <ul class='uk-list uk-list-bullet uk-margin-remove'>
            <b:loop values='data:labels filter (label  =&gt; label.name  not in {&quot;full_title&quot;, &quot;right_side&quot;, &quot;no_side&quot;})' var='label'>
              <li>
                <a class='label-name' expr:href='data:label.url'>
                  <span class='label-text'><data:label.name/></span><b:if cond='data:this.showFreqNumbers'><span class='label-count uk-align-left uk-margin-remove'><data:label.count/></span></b:if>
                </a>
              </li>
            </b:loop>
          </ul>
        </b:includable>
            </b:widget>
            <b:widget id='ContactForm1' locked='false' title='نموذج الاتصال' type='ContactForm' visible='true'>
              <b:includable id='main'>
  <b:include name='widget-title'/>
  <b:include name='content'/>
</b:includable>
              <b:includable id='content'>
          <div class='contact-form-widget'>
            <div class='form'>
              <form name='contact-form'>
                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <span class='uk-form-icon uk-form-icon-flip' data-uk-icon='user'/>
                    <input class='contact-form-name uk-input' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' type='text' value=''/>
                  </div>
                </div>
                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <span class='uk-form-icon uk-form-icon-flip' data-uk-icon='mail'/>
                    <input class='contact-form-email uk-input' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg + &quot; *&quot;' name='email' type='text' value=''/>
                  </div>
                </div>

                <div class='uk-margin'>
                  <div class='uk-inline'>
                    <textarea class='contact-form-email-message uk-textarea' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg + &quot; *&quot;' name='email-message' rows='5'/>
                  </div>
                </div>
                <div class='uk-button uk-button-danger uk-width-1-1'>
                  <span><data:contactFormSendMsg/></span><span class='uk-margin-small-right uk-icon' data-uk-icon='forward'/><input class='class=&quot;contact-form-button contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' value=''/>
                </div>
                <div class='contact-form-message-box'>
                  <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
                  <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
                </div>
              </form>
            </div>
          </div>
        </b:includable>
            </b:widget>
          </b:section>
        </div>
      </div>

      <!-- script -->
      <script src='//ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js'/>
      <script src='//ar-themes.github.io/templates/themeforest/salbuta/plugins-1.1-rtl.min.js'/>

    </b:with>

  </body>
</html>
