Women Who Code Tokyo Website
=====================
## ファイル構成
* css
    * global.css
    * normalize.css
    * simplegrid.css
    * style.css
* images 
* js
    * html5shiv.min.js
    * jquery-1.11.1.min.js
    * main.js
    * modernizr.js
* index.html
* style.css

##説明

### CSS

grobal.css－ページ全体に共通するスタイルを定義してあります。(見出しタグやフォントのサイズなど)   
normalize.css－ブラウザにはデフォルトでスタイルが当てられています。それをリセットするCSSです。   
simplegrid.css－スマートフォンで見たときに表示を最適化するためのライブラリです。 [Simple Grid](http://thisisdallas.github.io/Simple-Grid/ "Simple Grid")   
**style.css－ここにCSSを記述します。**  

###  Images
画像ファイルを使用する場合はこのディレクトリに置いてください
###  JS(Javascript)
html5shiv.min.js－html5をサポートしていないInternet Explore8で表示が崩れないようにするライブラリです。  
jquery-1.11.1.min.js－JSのライブラリである [jQuery](http://jquery.com/ "jQuery") です。JSより簡単な記述でいろいろなことができます。  
**main.js－Javascript(jQuery)はここに記述します。**  
modernizr.js－これも古いブラウザに対応するためのライブラリです。

### index.html
**HTMLをここに記述します。**

### style.css
CSSファイルを一本化するためにcssフォルダにあるファイルを@importを使って読み込んでいます。

##  コーディングするにあたって
###  基本的な進め方
htmlはindex.htmlに記述し、CSSはcssフォルダ直下のstyle.cssに書いていってください。

    index.html
    <!--header-->
    ここにコード
    <!--header END>

    css/style.css
    /*Header
    **********************:*/
    ここにコード


###  スタイルが共通する部分について
①見出しタグ(h1,h2タグ)、基本となるフォントサイズ、フォントカラーは指定してあるので個別に指定しなくて大丈夫です。  

大見出し(h1)と中見出し(h2)の記述の仕方

    <h1>About</h1>
    <h2><span>Our Mission<span></h2>

②記述例


### レスポンシブデザイン
PC以外のデバイスからWEBサイトを閲覧した時に、そのデバイスに表示が最適化されるデザインをレスポンシブデザインといいます。
この雛形も[Simple Grid](http://thisisdallas.github.io/Simple-Grid/ "Simple Grid") というCSSライブラリを読み込んでいるのでclass名を指定するだけで簡単にレスポンシブデザインが実現できます。(メニュー除く)　  
クラス名の指定の仕方

    <div class="grid grid-pad">　<!--コンテンツを中央寄せ&段落回り込み解除-->
	  <div class="col-1-2">ここにコンテンツ</div> <!--width:50%;-->
      <div class="col-1-2">ここにコンテンツ</div>  <!--width:50%;-->
    </div>
    


12カラム構成なので、そのうちいくつのカラムを1ブロックに使いたいかを指定します。
たとえば4ブロックを横に並べたい場合はcol-1-4と記述します。
詳しいサンプルはSimple Gridの[公式サイト](http://thisisdallas.github.io/Simple-Grid/ "Simple Grid") を参考にしてください。   
きちんとレスポンシブデザインになっているかどうかはブラウザサイズを縮小することで確認できます。

## 参考サイト
###  HTML
[HTML5リファレンス](http://www.htmq.com/html5/ "HTML5リファレンス") 　
### CSS
[CSSリファレンス](http://www.htmq.com/csskihon/001.shtml "CSSリファレンス")
### 実践的な用例
[HTML+CSSによるウェブページ制作例](http://www.htmq.com/csskihon/401.shtml "HTML+CSSによるウェブページ制作例")

[CSSでレイアウトするなら絶対覚えておきたい配置のルール：フロートや絶対配置、z-index とかいろいろ](http://webdesignrecipes.com/css-visual-formating-model/ "CSSでレイアウトするなら絶対覚えておきたい配置のルール：フロートや絶対配置、z-index とかいろいろ")
