#Prefectly
Prefectly はHTMLとCSSだけを使って日本地図を簡単に表示できるシンボルフォントです。各都道府県はCSSで個別にスタイルをつけられるのでシンプルなビジュアライゼーションに利用できます。そして、フォントなので自由に拡大縮小できます。  
Prefectly is a symbol font that makes is easy to create a map of the Japan using only HTML and CSS. Each prefecture can be styled independently with CSS for making simple visualizations. And since it's a font, it scales bigger and smaller while staying sharp as a tack.


##Files
    map.svg      - SVG map used to create the font
    assets\font  - Folder containing the web-font files
    assets\sass  - Folder containing basic Sass files, including both Prefectly setup and prefectly.html demo customizations
    assets\css   - Folder containing compiled CSS files
    prefectly.html - Basic Demo
    prefectly.ttf  - TrueType font file
    

##What is Prefectly?
Each prefecture is a glyph within the font. Each prefecture is positioned and sized relative to the the rest of the prefectures, so that when each character is stacked on top of one another, it creates a full map.
The pertinent characters are uppercase A-Z and lowercase a-u with lowercase u generating Yamanashi prefecture and lowercase z generating a full Japan map.
For modern browsers ligatures are available and a prefecture's abbreviation is its ligature. For example, "st" generates the glyph of the prefecture of Saitama and 'hk' Hokkaido. Additionally, the ligature "jp" produces a character of the full Japan map.

##Basic Use Case
You can use Prefectly however you like, but some base Sass/CSS and HTML is included.
Download and add the Prefectly folder to your project which includes the base CSS and the web font files. Grab the prefectly folder and add it to your project. Then add the prefectly.css to the head of your document.

```html
<link rel="stylesheet" href="assets/css/prefectly.css">
```

Then add this markup to the page:

```html
<ul class="prefectly" id="plain">
	<li data-pref="ac" class="ac">A</li>
	<li data-pref="ak" class="ak">B</li>
	<li data-pref="am" class="am">C</li>
	<li data-pref="cb" class="cb">D</li>
	<li data-pref="eh" class="eh">E</li>
	<li data-pref="fk" class="fk">F</li>
	<li data-pref="fo" class="fo">G</li>
	<li data-pref="fs" class="fs">H</li>
	<li data-pref="gf" class="gf">I</li>
	<li data-pref="gm" class="gm">J</li>
	<li data-pref="hg" class="hg">K</li>
	<li data-pref="hk" class="hk">L</li>
	<li data-pref="hs" class="hs">M</li>
	<li data-pref="ig" class="ig">N</li>
	<li data-pref="ik" class="ik">O</li>
	<li data-pref="it" class="it">P</li>
	<li data-pref="ka" class="ka">Q</li>
	<li data-pref="kg" class="kg">R</li>
	<li data-pref="km" class="km">S</li>
	<li data-pref="kn" class="kn">T</li>
	<li data-pref="ko" class="ko">U</li>
	<li data-pref="kt" class="kt">V</li>
	<li data-pref="me" class="me">W</li>
	<li data-pref="mg" class="mg">X</li>
	<li data-pref="mz" class="mz">Y</li>
	<li data-pref="ng" class="ng">Z</li>
	<li data-pref="nn" class="nn">a</li>
	<li data-pref="nr" class="nr">b</li>
	<li data-pref="ns" class="ns">c</li>
	<li data-pref="on" class="on">d</li>
	<li data-pref="os" class="os">e</li>
	<li data-pref="ot" class="ot">f</li>
	<li data-pref="oy" class="oy">g</li>
	<li data-pref="sa" class="sa">h</li>
	<li data-pref="sg" class="sg">i</li>
	<li data-pref="sn" class="sn">j</li>
	<li data-pref="so" class="so">k</li>
	<li data-pref="st" class="st">l</li>
	<li data-pref="tg" class="tg">m</li>
	<li data-pref="tk" class="tk">n</li>
	<li data-pref="to" class="to">o</li>
	<li data-pref="tt" class="tt">p</li>
	<li data-pref="ty" class="ty">q</li>
	<li data-pref="wk" class="wk">r</li>
	<li data-pref="yg" class="yg">s</li>
	<li data-pref="ym" class="ym">t</li>
	<li data-pref="yn" class="yn">u</li>
</ul>
```
    
Set the size and base map color in your CSS:

```css
.prefectly{
    width: 300px;     /* width and font size must match */
    font-size: 300px; /*width and font size must match */
    color: #f0f0f0;
}
```
    
Style Individual Prefecture:

```css
.prefectly .ac,
.prefectly .hk,
.prefectly .st{ 
   color: #FF0000;
}
```
    
If you are not using Sass for your project, you can use and edit the compiled CSS files. The included files have been compiled using the `expanded` output style for readability.
    
##Live Example

[Prefectly Microsite](http://deform.jp/prefectly/)

##Resources

[Free Online Font Converter](http://www.freefontconverter.com) - For converting SVG to TTF  
[Font Squirrel](http://www.fontsquirrel.com/fontface/generator) - For converting TTF to web fonts (make sure you check 'no subsetting')  
[Intridea Blog: How to Make Your Own Symbol Font](http://www.intridea.com/blog/2012/4/24/symbol-font) - A good starting place

##Credits

Created by Hiroto Sugita at deform. 

Hiroto Sugita  
[Twitter](http://www.twitter.com/hrtsgt)  
[Website](http://args.in)  

deform  
[Twitter](http://www.twitter.com/deformjp)  
[Website](http://deform.jp)  

##License

MIT License. See LICENSE for details.

##Copyright

Copyright (c) 2013 deform.jp
