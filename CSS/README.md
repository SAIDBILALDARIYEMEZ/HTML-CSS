CSS

Ön tanımlı css

Ön tanımlı css’lerdir. Hali hazırda browser’in tanımladığı cıs komutlarıdır. Bunları kendi yazdığın css ile düzeltebilirsin veya ceset.css veya normalize.css ile düzeltebilirsin. Reset cıs cıs komutlarını 0’larken normalize css birden fazla browser’ın komutlarını inceleyip standart bir css ekler.

Display

Sitede kapladığı alandır.
display: inline; —> satır içidir. Yan yana gelebilir.
display: block; olarak iki tanedir.  —> blok blok’tur. Yan yan gelemez. Alt alta gelebilir.
.
.
.
.
.

Background (arka plan yapma)

Color (renklendirme)

Örnek

h1 {
  background-color: green;
}

div {
  background-color: lightblue;
}

p {
  background-color: yellow;
}


Opacity (opaklık şeffaflık ayarlama)

0,0 – 1,0 arasında değer alabilir.

Örnek

div {
  background-color: green;
  opacity: 0.3;
}

image ( resim ekleme)

Örnek

body {
  background-image: url("paper.gif");
}

background-repeat (arka plan tekrarı)

Örnek

background-image: url("gradient_bg.png");
  background-repeat: repeat-x;
(Yatay olarak tekrar ettirir)
background-repeat: repeat-y;
(Yatay olarak tekrar ettirir.)
background-repeat: no-repeat;
(Tekrar ettirmez.)

background-position (resmin konumunu ayarlar.)

Örmek

background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
(Pozisyonu sağ üste ayarladık.)


background-attachment (resmin tekrar edilip edilmemesini ayarlar.)

Örnek

background-image: url("img_tree.png");
  background-repeat: no-repeat;
  background-position: right top;
  background-attachment: fixed;
(Ekranla kaymaz sabit kalır.)
background-attachment: scroll;
(Ekran kayarken oda kayar.)

background-size (resmin boyutunu ayarlar.)

Örnek

background-size: auto;
(Tam sığar)
background-size: 300px 100px;
(Seçili alana tam sığar.)


border (kenar boşlukları)

border-style (kenarlık stilleri)

Örnek

p.dotted {border-style: dotted;}
(Bu şekilde yapılır.)

* dashed- Kesikli bir kenarlık tanımlar
* solid- Sağlam bir sınır tanımlar
* double- Çift kenarlık tanımlar
* groove- 3 boyutlu yivli bir kenarlık tanımlar. Efekt kenarlık rengi değerine bağlıdır
* ridge- 3 boyutlu çıkıntılı bir kenarlık tanımlar. Efekt kenarlık rengi değerine bağlıdır
* inset- 3 boyutlu bir iç kenarlık tanımlar. Efekt kenarlık rengi değerine bağlıdır
* outset- 3 boyutlu başlangıç sınırını tanımlar. Efekt kenarlık rengi değerine bağlıdır
* none- Hiçbir sınırı tanımlamaz
* hidden- Gizli bir kenarlık tanımlar
* dotted- Noktalı bir kenarlık tanımlar

border-width (kenar genişliği)


Örnek

p.four {
  border-style: dotted;
  border-width: thick; (kalın)
border-width: 25px 10px 4px 35px; /* 25px üst, 10px sağ, 4px alt ve 35px sol */
}


border-color (kenarlık rengi)

Örnek

p.three {
  border-style: dotted;
  border-color: blue;
border-color: red green blue yellow;
}

p {
  border: 5px solid red;
(Özel kısaltılmış kenarlıklar.)
}

border-radius (yuvarlaklaştırır)

Örnek

p {
  border: 2px solid red;
  border-radius: 5px;
(gibi)
}

Margins (kenar boşlukları)
Yani yazının alanının çerçeve veya pc ekranıyla arasındaki boşluktur.

Örnek

p {
  margin: 25px 50px 75px 100px;
margin: auto;
}


Padding (kenar dolgusu)
Yani kendi sınırları veya alanı içerisinde belirlenen yerlerdeki alandır.

Örnek

div {
  padding: 25px 50px 75px 100px;
}

height width (yükseklik genişlik)

* auto- Bu varsayılandır. Tarayıcı yüksekliği ve genişliği hesaplar
* length- Yüksekliği/genişliği px, cm vb. cinsinden tanımlar.
* %- İçerdiği bloğun yüksekliğini/genişliğini yüzde olarak tanımlar
* initial- Yüksekliği/genişliği varsayılan değerine ayarlar
* inherit- Yükseklik/genişlik ana değerinden miras alınacaktır

Örnek

div {
  height: 200px;
  width: 50%;
  background-color: powderblue;
}

Dolguyu kenarlığı ve kenar boşluklarına dahil değildir.

Kutu modelinde content alanını etkiler.

Box Model
￼
Örnek

div {
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}

Outline (taslak)
sınırının dışına çizilen bir çizgidir.
￼

outline-style(taslağın sitili tarzıdır.)

* dotted- Noktalı bir taslak tanımlar
* dashed- Kesikli bir taslak tanımlar
* solid- Sağlam bir taslak tanımlar
* double- Çift taslak tanımlar
* groove- 3 boyutlu yivli bir taslağı tanımlar
* ridge- 3 boyutlu çıkıntılı bir taslağı tanımlar
* inset- 3 boyutlu bir iç metin taslağını tanımlar
* outset- 3 boyutlu başlangıç taslağını tanımlar
* none- Hiçbir taslak tanımlamaz
* hidden- Gizli bir taslak tanımlar

Örnek

p.dotted {outline-style: dotted;}

outline-width (taslağın kalınlığıdır.)

Örnek

p.ex1 {
  border: 1px solid black;
  outline-style: solid;
  outline-color: red;
  outline-width: thin;
}

outline-color (rengi)

Örnek

p.ex1 {
  border: 2px solid black;
  outline-style: solid;
  outline-color: red;
}

outline-offset (uzaklığı)

Örnek

p {
  margin: 30px;
  background: yellow;
  border: 1px solid black;
  outline: 1px solid red;
  outline-offset: 15px;
}

Text (yazı)

Text Color

Örnek

h1 {
  color: green;
}

Text Alignment (hizalanması)

Örnek

h1 {
  text-align: justify;
(Bütün satırları satıra 0a 0 ayarladık.)
}

vertical-align (dikey hizalama)

Örnek

img.a {
  vertical-align: baseline;
}

img.b {
  vertical-align: text-top;
}

img.c {
  vertical-align: text-bottom;
}

img.d {
  vertical-align: sub;
}

img.e {
  vertical-align: super;
}

text decoration (yazı dekorasyonu)

* text-decoration-line

h1 {
  text-decoration-line: overline;
(Yazının üst tarafını  çizer)
  text-decoration-line: line-through;
(Üstünü cizer)
  text-decoration-line: underline;
(Altını çizer)
  text-decoration-line: overline underline;
(Hem altını hem üstünü çizer)

* text-decoration-color

h2 {
  text-decoration-line: line-through;
  text-decoration-color: blue;
}


* text-decoration-style (stilini belirler)

h1 {
  text-decoration-line: underline;
  text-decoration-style: solid;
}

* text-decoration-thickness (kalınlığını belirler)

h1 {
  text-decoration-line: underline;
  text-decoration-thickness: auto;
}


Text Spacing (metin aralığı)

* text-indent
  ilk satırının girintisini belirtmek için kullanılır

p {
  text-indent: 50px;
}

* letter-spacing
  karakterler arasındaki boşluğu belirtmek için kullanılır.

h1 {
  letter-spacing: 5px;
}

* line-height
  satırlar arasındaki boşluğu belirtmek için kullanılır:

p.small {
  line-height: 0.8;
}

* word-spacing
  kelimeler arasındaki boşluğu belirtmek için kullanılır.

p.one {
  word-spacing: 10px;
}

text-shadow (metni gölgelendirmek)

Örnek

h1 {
  text-shadow: 2px 2px 5px red;
(Gölge boyu 2-2, bulanıklık ekler, renk ekler.)
}

Fonts

Yazı stili

.p1 {
  font-family: "Times New Roman", Times, serif;
}

.p2 {
  font-family: Arial, Helvetica, sans-serif;
}

.p3 {
  font-family: "Lucida Console", "Courier New", monospace;
}

font-style (yazı stili)

p.normal {
  font-style: normal;
italic
oblique (eğik)
}

font-weight (ağırlığı)
p.normal {
  font-weight: normal;
}

p.thick {
  font-weight: bold; (kalın)
}

font-size(boyutu)

h1 {
  font-size: 40px;
}


Links

* a:link- normal, ziyaret edilmemiş bir bağlantı
* a:visited- kullanıcının ziyaret ettiği bir bağlantı
* a:hover- kullanıcı fareyi üzerine getirdiğinde bir bağlantı
* a:active- tıklandığı anda bir bağlantı

/* ziyaret edilmemiş bağlantı */
a:link {
  color: red;
}

/* ziyaret edilen bağlantı */
a:visited {
  color: green;
}

/* fareyi bağlantının üzerine getirin */
a:hover {
  color: hotpink;
}

/* seçilen bağlantı */
a:active {
  color: blue;
}

Tablolar

border (kenar kalınlığı)

table, th, td {
  border: 1px solid;
}

width (genişlik)

table {
  width: 100%;
}

border-collapse (kenarların çift kattan tek kat olması )
table {
  border-collapse: collapse;
}

text-align (hizalanmasını sağlar)

td {
  text-align: center;
text-align: left:
}

display (yapıların nasıl görüntüleneceğini belirtir.)

Varsayılan genelde ya inline veya block’dur.

İnline yan yana gelebilir
Block yan yana gelemez üst üstedir.
contents Kabı ortadan kaldırarak öğenin alt öğelerini DOM'da bir sonraki seviyeye yükseltir
flex Bir öğeyi blok düzeyinde esnek kapsayıcı olarak görüntüler
grid Bir öğeyi blok düzeyinde ızgara kapsayıcısı olarak görüntüler
inline-block Bir öğeyi satır içi düzeyde blok kapsayıcısı olarak görüntüler. Öğenin kendisi satır içi öğe olarak biçimlendirilmiştir ancak yükseklik ve genişlik değerlerini uygulayabilirsiniz.
inline-flex Bir öğeyi satır içi düzeyde esnek kapsayıcı olarak görüntüler
inline-grid Bir öğeyi satır içi düzey ızgara kapsayıcısı olarak görüntüler
table Öğenin bir <table> öğesi gibi davranmasına izin verin
none Öğe tamamen kaldırıldı
initial Bu özelliği varsayılan değerine ayarlar
inherit Bu özelliği üst öğesinden devralır


h1.hidden {
  visibility: hidden;
(Fotoyu yok eder ama konumunu korur.)

Display: none;
(Fotoyu yok eder ve konumunu korumaz.)
}



position Property (konum özelliği)

* static (statik)
  özel şekilde konumlandırılmamıştır; her zaman sayfanın normal akışına göre konumlandırılır:

* relative
  normal konumunu kaybetmeden konumlandırılır.

* fixed
  bu, sayfa kaydırılsa bile her zaman aynı yerde kalacağı anlamına gelir.

* absolute
  en yakın veya içinde bulunduğu konumdaki yapıya göre konumlandırılır. Normal konumunu kaybeder.

* sticky
  Sayfa nekadar kaydırılsada  yapı oraya yapışmış bir vaziyette sadece orda kalır.

Örnek

div.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 300px;
  border: 3px solid #73AD21;
}

z-index
Üst üste binip binemmesini ayarlar.

Örnek

img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}

overflow

* visible- Varsayılan. Taşma kırpılmaz. İçerik, öğenin kutusunun dışında işleniyor
* hidden- Taşma kırpılır ve içeriğin geri kalanı görünmez olur
* scroll- Taşma kırpıldı ve içeriğin geri kalanını görmek için bir kaydırma çubuğu eklendi
* auto- Benzeri scroll, ancak yalnızca gerektiğinde kaydırma çubukları ekler

Örnek

div {
  overflow: auto;
}

div {
  overflow-x: hidden; 
(Yatay kaydırma çubuğunu gizle)
  overflow-y: scroll;
(Dikey kaydırma çubuğu ekle)
}

Float

* left- Eleman bulunduğu kabın soluna doğru yüzer
* right- Eleman bulunduğu kabın sağına doğru yüzer
* none- Öğe yüzmez (metinde geçtiği yerde görüntülenecektir). Bu varsayılandır
* inherit- Eleman, ebeveyninin float değerini miras alır

Örnek

img {
  float: none;
}

Renk Anahtar Kelimeleri

* transparent
  (Arka planı şeffaf yapar)

body {
  background-image: url("paper.gif");
}

div {
  background-color: transparent;
}

* currentcolor
  (o anda kod tekrarına düşülmemesi için devrede kullanılan rengialır)

div {
  color: blue;
  border: 10px solid currentcolor;
}

* inherit
  (kapsayıcısının kendi özelliği olan özelliği alır.)



Çoklu Sütunlar

* column-count
  (bir öğenin bölünmesi gereken sütun sayısını belirtir.)

div {
  column-count: 3;
}

* column-gap
  (sütunlar arasındaki boşluğu belirtir.)

div {
  column-gap: 40px;
}

* column-rule-style
  (sütunlar arasındaki kuralın stilini belirtir:)

div {
  column-rule-style: solid;
}

* column-rule-width
  (sütunlar arasındaki kuralın genişliğini belirtir:)

div {
  column-rule-width: 1px;
}

* column-rule-color
  (sütunlar arasındaki kuralın rengini belirtir:)

div {
  column-rule-color: lightblue;
}

* column-rule
  (yukarıdaki tüm sütun kuralı-* özelliklerini ayarlamak için kullanılan kısa bir özelliktir.)

div {
  column-rule: 1px solid lightblue;
}

* column-span
  (bir öğenin kaç sütuna yayılması gerektiğini belirtir.)

h2 {
  column-span: all;
}

* column-width
  (sütunlar için önerilen, en uygun genişliği belirtir.)

div {
  column-width: 100px;
}


var() İşlevi

:root içine yazılan değerler var ile başka bir kodun içine yazılarak ayarlanır.

Örnek


:root {
  --blue: #1e90ff;
  --white: #ffffff;
}

body { background-color: var(--blue); }

h2 { border-bottom: 2px solid var(--blue); }

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}


Box sizing

Kutu çevresine eklenen padding border vs ile kutu ortalanması gerek yeri kaydır. Bunun düzeltilmesi için bu kullanılır.

box-sizing: border-box;
Genişlik ve yüksekliğe padding ve border atama esnasında dahil eder

box-sizing: content-box;
Genişlik ve yüksekliğe padding ve border sonradan dahil eder


Site düzeni


￼

Section

* Bölümler
* giriiş
* Haber öğeleri
* İletişim bilgileri

article
* Forum gönderileri
* Blog gönderileri
* Kullanıcı yorumları
* Ürün kartları
* Gazete makaleleri

header
* bir veya daha fazla başlık öğesi (<h1> - <h6>)
* logo veya simge
* yazarlık bilgisi

footer
* yazarlık bilgisi
* telif hakkı bilgisi
* iletişim bilgileri
* site haritası
* üst bağlantılara dön
* alakalı dökümanlar

nav
* Gezinme bağlantısıdır.

aside
* Kenar çubuğudur.



￼
Content içeriktir

scss

https://sass-lang.com/

Kolay kod yazımı ve yanında gelen diğer kullanışlı parametreler sayesinde okunaklı css dosyaları yazmamızı sağlar.

Cascade & specificity (özgünlük)

cascade —> yukardan aşağıya koro css dosyasının okunması.

Diğeri ise güçlü olan sıralama  bakılmaksızın ezer geçer
Style > ıd > class > diğer




Projeden notlar



height: $Header-height;
/*alanın yüksekliği*/

    position: relative; 
/*konumandırıldığı top right vs yönlerini bu  komut sayesinde taşınır. konumlandırmak için gereklidir.*/

    display: flex;
/*esnek kapsayıcıdır. kutuları istediğin gibi haraket ettirri*/

    align-items: center; 
/* yatay olark hizalanmış ögelrei dikey ortalama sağlar.*/

    height: 100%; 
/*yükseklktir.*/

      width: 144px;
/*genişlik*/

    position: relative;
/*konumandırıldığı top right vs yönlerini bu  komut sayesinde taşınır. konumlandırmak için gereklidir.*/

    margin-left: auto;
/*yazımnın ekran veya kapsayıcısı arasındaki boşluğudur.*/

      display: none; 
/*ögeyi yok say*/

    pointer-events: none;
/*tıklanmaz hale gelir.*/

    display: flex; 
/*ögeler daha kolay ayarlanır.*/

    position: fixed;
/*kaosayıcısında sabit olaraak durur.*/

    padding-left: $gutter; 
/*kapsayıcı sınırını belirler*/

    flex-direction: column; 
/*sütun halinde dikey olarak hizalanır.*/

      pointer-events: auto; 
/*fare ile etkileşime açık*/

      pointer-events: auto; 
/*fare ile etkileşime açık*/

      margin-left: auto; 
/*yazımnın ekran veya kapsayıcısı arasındaki boşluğudur.*/

      flex-direction: row; 
/*satıra göre hizalanır.*/

      position: static; 
/* normal düzen nasılsa ona göre düzen sağlar.*/

      background-color: transparent;
/*arka plan görünmez olarak ayarlanır.*/

      padding-right: 0; 
/*kapsayıcı sınırını belirler.*/

      display: flex; 
/*kolay hizalanmasına olanak sağlar.*/

      flex-direction: column; 
/*sütun halinde dikey olarak hizalanır.*/

      align-items: center;
/* yatay olark hizalanmış ögelrei dikey ortalama sağlar.*/

        flex-direction: row; 
/*satıra göre hizalanır.*/

        display: inline-flex; 
/*satırda kolay hareket edişmesini sağlar.*/

        align-items: center; 
/* yatay olark hizalanmış ögelrei dikey ortalama sağlar.*/

        justify-content: center;
/*yatay eksnde sağa sola değil ortada kalmasını sağlar:*/

        padding-left: 20px; 
/*kapsayıcı sınırını belirler.*/

      margin-top: 20px;  
/*yazımnın ekran veya kapsayıcısı arasındaki boşluğudur.*/

      justify-content: center; 
/*yatay eksnde sağa sola değil ortada kalmasını sağlar:*/

      margin-top: 20px; 
/*yazımnın ekran veya kapsayıcısı arasındaki boşluğudur.*/

        appearance: none;
/*tataryıcının varsayılan görüntüsünü devre dışı bırakır.*/

        background-color: transparent;
/*arka plan rengini kaldırır*/

white-space: nowrap;
/*satır içindeki yazı uzadıkça satır atlamasını önler. gerekirse alanı gemübişletir */

font-weight: 500;
/*metnin kalınlığıdır. bold için 900 değeri verilebilir.*/

user-select: none;
/*metni seçmemsini veya kopyalayamamasını sağlar*/

column-gap: 30px;
/*satırlar arasındaki boşluktur*/

row-gap: 10px;
/*satırlar arası boşluktur*/

color: inherit;
/*kapsayıcısının rengini alır*/

text-decoration: underline;
/*seçili olan ögenin altını çizer*/

align-items: baseline;
/*alt kenarlarına göre hizalanırlar.*/

align-items: flex-start;
/*ögeyi üst sınıra göre hizalr*/

overflow: hidden;
/*taşan içeriği göstermez*/

overflow: visible;
/*taşan içeriğe izin verir.*/

content: "";
/*boş içerik olduğundan çakışmaz*/


position: absolute;
/*en yakın ögeye doğru konumlanır*/


background: white center center no-repeat / cover;
/*cover: resim arka plana sığar ama oranlar korunur.*/

clip-path: polygon(0 0, 100% 100%, 0 100%);
/*ögrnin görünümünü çokgene göre kırpmaya yarra*/

line-height: 1.6;
/*satır yüksekliğini ayarlar*/

flex-shrink: 0;
/*içindeki ögenin boyutu değişse bile kendi boyu değişmez*/

transition: transform .4s ease;
/*boyut değişikliğini daa hyumuşak bir şekilde yapabilmesini sağlar.*/

transform: scale(1.1);
/*ögenin boyutunu büyütür.*/



/*yazı için fazladan satır gerekirse satır atlamasını sağlar*/




Scroll-margin-top: 120px;
/*sayfa içinde kanca görevi gören linklerde tepede sabit olan menü çubuklarından dolayı görünmezse yukarıya görünmez bir boşluk koyar.*/



Grid yapıları
https://www.youtube.com/watch?v=kI77jbuMU1Y

Ekranı ızgara olarak böler.

Display: grid;
(Grid yapısını blok olarak oluşturur.)

Display: inline-grid;
(Satır içi olarak grid oluştururç)

Grid-template-rows: 150px (1. satır) 250px (2. satır);
(Satır boyutunu ayarlar)

Grid-template-colums: 150px (1. sütun) 250px (2. sütun);
(Sütun boyutunu ayarlar)

Grid-template: 150px 250px (satırlar) / 200px 300px  auto (sütunlar); (auto px değerlerini verdikten sonra ekranı doldurur.)
(Yukardaki iki ayarın kısaltılmış hali)

Order: -1;
(Sıralamayı ayarlar.)

Grid-row-start: 2;
Grid-row-end: 3;
Grid-column-start: 2;
Grid-column-start: 2;
(Belirtilen satır ve sütun çizgilerine göre konumunu ayarlar.)

Grid-row: 2 / 3;
Grid-column: 2 / 3;
(Yukardaki işlemin kısaltılmış hali)



Grid-row-gap: 10px;
(Satırlar arasında 10px boşluk oluşturuldu)

Grid-column-gap: 10px;
(Sütunlar arasında 10px boşluk oluşturuldu)

Grid-gap: 10px 20px;
(Yukardakinin kısa hali)


Css ölçü birimleri

Px
Ayarlanan boyut ekranın boyutuna oranla değişmez. Hep aynı kalır. Eğer ki ekrana 600 * 800 bir kutu çizcek olsan bu boyut ekran 27 inc de olsa 32 veya 13 inc de olsa değişmez.

Em
Kapsayıcısına oranla büyür. Yani eğerki kapsayıcısı 16 px ise ve em değerli değişken 1 em ise 16 px’e eşittir. Eğerki 2 em ise 2*16’dan 32 px’e eşittir.  
Bu bir tehlike arz eder ki iç içe yapılarda bu değer katlanır. Mesela 3 ul yapısı iç içe olsun. Var sayılan px değerimiz 16px ve ul değerlerimim 2 em olursa sonuç şöyle gelişir.  İlk ul yapısı 2*16, 2. Ul yapısı 2*2*16, 3. Ul yapısı 2*2*2*16dır. bu yüzden bu tip değerlerde (font size) rem değeri kullanılmalı ve em değeri ise padding veya margin gibi yapılarda kullanılmalı.

Rem (root em)
Bu ise kapsayıcısına değil ana kapsayıcısına veya html deki ana değere göre kendini konumlar. Bu da font-size için daha  uygundur.

v w (v width) genişlik
Geniliği ekranın değeri kadar olur. Mesela 100 v w verilen değerde ekranın gemnişliğini 100% kadar ayarlar.

vh (v height) uzunluk
Uzunluğu ekranın değeri kadar olur. Mesela 100 vh ise ekranın uzunluğunun 100% kadar olur.

vmin
En küçük ekran hangisi ise onu referans alarak ona göre diğer kenarda ayarlanır

vmax
E büyük kenar hangisi ise diğer kenarda ona göre ayae



Pseudo Elemanlar ( ::after | ::before ) ve Sınıflar ( :hover | nth-child(n) )

P::after { color: red;}
(Paragraftan sonrasını etkiler.)

P::before { color: red;}
(Paragraftan öncesini etkiler.)

P::first-line {color: red;}
(Sadece ilk satış etkiler)

P:nth-last-child(2) {color: red;}
(Sondan ikinci elemanı etkiler)



Medya sorguları

@media özelliğini kullanarak genişliğin boyutuna göre ayarlanmalar gerçekleşecek

body {
background-color: lightblue;
}

    @media screen and (min-width: 400px) {
    body {
        background-color: lightgreen;
    }
    }

    @media screen and (min-width: 800px) {
    body {
        background-color: lavender;
    }
    } 


(Yatay konumda bu rengi alır)
@media only screen and (orientation: landscape) {
body {
background-color: lightblue;
}
}

(Dikey konumda bu rengi alır.)
@media only screen and (orientation: portrait) {
body {
background-color: lightblue;
}
}



Birden fazla sorgu birleştirilebilir

    ( 900 ve 600 px arasında isen veya 1100 ün üstünde isen bu komutlar işler )
    @media screen and (max-width: 900px) and (min-width: 600px), (min-width: 1100px) {
        div.example {
            font-size: 50px;
            padding: 50px;
            border: 8px solid black;
            background: yellow;
        }
    }




Flexbox


Parent Element(Container)->display: flex | inline-flex
---------------------------
flex-direction: row(yatay hizalanma) | row-reverse (ters yatay hizalanma) | column(dikey hizalanam) | column-reverse (ters dikey hizalanma)
(Ana ekseni ve yönü belirtir)
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-direction&preval=row
￼

flex-wrap: nowrap (kaydırma işlemini yapmaz)| wrap(kaydırma işlemini düz bir şekilde yapar.) | wrap-reverse(kaydırma işlemini ters yapar.)
(Ana eksene sığmayan elemanları bi alt satıra kaydırır)
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-wrap&preval=nowrap
￼

flex-flow: flex-direction flex-wrap ->(shorthand(kısaltma)) (iki tane özelliği eklemek içim yapar. )
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-flow

justify-content: flex-start(başlangıca ayarlar) | flex-end(sona ayarlar) | center(ortalar) | space-between(sağa sola tam yapışırlar ve ortada kalan kısım ise boşluklar eşit dağılır) | space-arround(sağ ve sollarından eşit boşluklar alırlar.) | space-evenly (kenarlar dahil her yerden eşit boşluk bırakırlar.)
(Flex-direction olarak belirlenen ana eksende hizalanmadan sonra konumunu ayarlar)
https://www.w3schools.com/cssref/playit.asp?filename=playcss_justify-content&preval=flex-start
￼

align-items: stretch (kapladığı alana kadar y ekseninde uzar.)| center | flex-start (y ekseninde başa gelir)| flex-end | baseline (yazıya göre hizalanır. Yazının alt tarafını referans alır. )
(Karşıt eksende işlem yapar ama tek satırda kullanılır. Tabi önce flex-direction ile yön belirlenir. )
https://www.w3schools.com/cssref/playit.asp?filename=playcss_align-items&preval=stretch
￼

NOT:align-items özelliğini geçersiz kılmak için align-self kullanılabilir

align-content: stretch | center(ortalar) | flex-start (sahip Olduğu eksende Başa yapışır.) | flex-end (sona yapışır.)| space-between(her iki uca yapıştırır.ortadakilerdede eşit boşluklar bırakır.) | space-around (başta ve sonda boşluk bırakıp ortalardakinde yine eşit boşluk yapar.)
(Wrap ile kaydırma işlemi yapıldığında çoklu satırlarda işe yarar.)
https://www.w3schools.com/cssref/playit.asp?filename=playcss_align-content&preval=stretch
￼

NOT:content çoklu satırlar için kullanılır

Flex Items
-------------
order: number(0) | initial | inherit ->sıralama
(Sıralama ayarlanır. Sıralamada en küçük değeri alan en başa geçer. )
https://www.w3schools.com/cssref/tryit.asp?filename=trycss3_order

flex-grow: number(0) | initial | inherit ->büyüklük değeri genişletme işi
(0 olan değer yerine verilen değerlerde değer saysı arttıkça eksen toplam değere bölünür ve herkes sahip olduğu değer kadar alır. )
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-grow&preval=1

flex-shrink: number(1) | initial | inherit ->küçüklük değeri daraltma işi
(100px den 3 kutu düşünülsün ve bunlar 250px lik bir kutuya girsin. Hepsi sıkışacaktır ama 0 değeri alan kutuya 0 değerini vererek sıkışması önlenilir. Eğerki 3’üne de 0 değeri verilirse zaman taşma gerçekleşir. )
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-shrink&preval=1

flex-basis: auto | number | initial | inherit ->başlangıç genişliği
(Dahil olduğu. Eksende % delik değerine göre o oranla genişler ve önceden sahip olduğu değeri ezer ama max boyutlar hariç. Onları ezemez. Ve  o max değerler içerisinde bölünür.)
https://www.w3schools.com/cssref/playit.asp?filename=playcss_flex-basis&preval=10px

flex: flex-grow flex-shrink flex-basis | auto | initial | inherit ->kısaltma

            flex: 0 1 auto -> varsayılan
            flex: 1 ->flex-grow
            flex: 300px ->flex-basis
            flex: 1 200% ->flex-grow flex-basis
            flex: 1 1 ->flex-grow flex-shrink
            flex: 1 0 200%


align-self: auto | stretch | center | flex-start | flex-end | baseline ->seçili eleman için hizalama
Normal akışı ezerek eski konumuna gelir.
https://www.w3schools.com/cssref/playit.asp?filename=playcss_align-self&preval=auto



Tavsiye:
https://css-tricks.com/snippets/css/a-guide-to-flexbox/

https://codepen.io/enxaneta/full/adLPwv


Transform-Transition-Animation

https://www.w3schools.com/cssref/css3_pr_transform.asp

CSS 2D Transforms
-----------------------
transform:translate(50px,100px) ->Konumlandırma (50px sağa,100px aşağı)
transform:translateX(10px)
transform:translateY(20px)
transform:rotate(20deg) ->20 derece saat yönünde döndür
transform:scale(2,2) ->Boyutu X ve Y eksenin 2 katına çıkar
transform:scaleX(2)
transform:scaleY(2)
transform:skew(10deg,10deg) ->10 derece x ekseninde 10 derece y ekseninde eğ
transform:skewX()
transform:skewY()
transform:matrix(scaleX(),skewY(),skewX(),scaleY(),translateX(),translateY())

transfrom-origin:x y z->Dönüştürülmüş elemanı konumlandırma - varsayılan (50% 50% 0)

CSS 3D Transforms
-----------------------
transform:translate3d(x,y,z)
transform:translateX(x)
transform:translateY(y)
transform:translateZ(z)
transform:scale3d(x,y,z)
transform:scaleX(x)
transform:scaleY(y)
transform:scaleZ(z)
transform:rotate3d(x,y,z,angle)
transform:rotateX(20deg)
transform:rotateY()
transform:rotateZ()
transform:perspective(100px) ->ögenin ne kadar uzağa yerleştirileceği

transfrom-origin:x y z->Dönüştürülmüş elemanı konumlandırma - varsayılan (50% 50% 0)

CSS Transitions
-----------------------
transition:property duration timing-function delay

transition-property:(all) | property | none
transition-duration:(0s) 5s | 2ms
transition-timing-function:(ease)|linear|ease-in|ease-out|...|cubic-bezier(n,n,n,n)
transition-delay:(0s) 5s | 2ms

property:Geçiş işleminin uygulanacağı CSS özelliğini belirtir (örn:width)
duration:Geçiş efektinin tamamlanması için kaç saniye veya milisaniye gerektiğini belirtir
timing-function:Geçiş efektinin hız eğrisini belirtir
delay:Gecikme süresi (saniye veya milisaniye)

CSS Animations
--------------------------
Hangi CSS Özellikleri Animasyona Uygun?
https://www.w3schools.com/cssref/css_animatable.asp

@keyframes mymove {
from {top: 0px;}
to {top: 200px;}
}
div {
width: 100px;
height: 100px;
background: red;
position: relative;
animation: mymove 5s infinite; ->Asıl animasyon özelliğinin uygulandığı yer
}
@keyframes mymove {
0%   {top: 0px; left: 0px; background: red;}
25%  {top: 0px; left: 100px; background: blue;!important} ->!important ifadesi alan bir kare yok sayılır
50%  {top: 100px; left: 100px; background: yellow;}
75%  {top: 100px; left: 0px; background: green;}
100% {top: 0px; left: 0px; background: red;}
}


animation:name duration timing-function delay iteration-count direction fill-mode play-state;
(none    0           ease        0          1          normal     none     running)

animation-name:(none) ->bağlamak istediğiniz anakare(keyframe) adı
animation-duration:(0s) ->animasyonun tamamlanma süresi (s/ms)
animation-timing-function:(ease) ->linear|ease|ease-in|...|steps(int,start|end)|cubic-bezier(n,n,n,n)
animation-delay:(0s) ->gecikme süresi (s/ms)
animation-iteration-count:(1) | infinite ->tekrarlama sayısı
animation-direction:(normal)|reverse|alternate|alternate-reverse ->hareket yönü
animation-fill-mode:(none)|forwards|backwards|both ->animasyon bitince gerçekleşecek işlem
animation-play-state:(running) | paused ->animasyonu duraklatmak ve çalıştırmak için kullanılır


Object-fit

Css de fotoğraf veya videonun kabı uygun konumlandırılmasıdır.

img {
  width: 200px;
  height: 300px;
  object-fit: cover;
}


Görüntünün 200x300 piksellik kaba sığacak şekilde sıkıştırıldığını görüyoruz (orijinal en boy oranı bozuldu).
İşte burada object-fitözellik devreye giriyor. object-fitÖzellik aşağıdaki değerlerden birini alabilir:
* fill- Bu varsayılandır. Görüntü, verilen boyutu dolduracak şekilde yeniden boyutlandırılır. Gerekirse görüntü sığacak şekilde uzatılacak veya sıkıştırılacaktır.
* contain- Görüntü en boy oranını korur ancak verilen boyuta sığacak şekilde yeniden boyutlandırılır
* cover- Görüntü en boy oranını korur ve verilen boyutu doldurur. Resim sığacak şekilde kırpılacak
* none- Resim yeniden boyutlandırılmaz
* scale-downnone- resim veya'nin en küçük versiyonuna küçültülür contain
















