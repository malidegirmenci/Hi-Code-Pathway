# En Çok Kullanılan HTML Etiketleri Nelerdir
HTML dilinde bir etiket nasıl oluşturulur? Etiketler küçüktür ve büyüktür işaretlerinin arasına yazılarak başlar. (örn. `<etiket>`) içeriği yazdıktan sonra etiketi kapatılması gerekir. Etiketi kapatmak için küçüktür, slash, etiket, büyüktür şeklinde yazılmalıdır. (örn. `</etiket>`) 
 
**(örn. `<etiket>` İçerik Yazılacak Alan `</etiket>`)**

Not: Bazı etiketler kapanmaya ihtiyaç duymazlar (örn. `<br>`, `<hr>`, `<meta>` vs.)

## HTML Etiketi
HTML etiketi, dosya içeriğinin HTML dilinde yazıldığını tarayıcımıza bildirir. Bu etiket, kendi altında mutlaka `<HEAD>` ve `<BODY>` etiketlerini barındırmalıdır. Eğer bir HTML dökümanı oluşturmak istenildiğinde ilk olarak `<html>` etiketi oluşturulur. Ardından HTML etiketi altına `<HEAD>` ve `<BODY>` etiketleri yazılmalıdır.

```html
<html>   
<head></head> 
<body></body>
</html>
```
### HEAD Etiketi
`<head>` etiketi, site ziyaretçileri tarafından görülmesi gerekmeyen kodları içerir. Bu etiket altına yazılan kodlar genellikle arama motorları ve örümcekler (Crawler veya Spider diye geçer) içindir. Head etiketi altında bütün etiketleri kullanabilmeniz mümkün değil.
Kullanılabilir etiketler;
```html
<title> (Bu etiketi kullanmak şarttır)
<meta>
<style>
<script>
<noscript>
<link>
<base>
```
```html
<html>   
<HEAD>
    <title> Sekmede Görülecek İsim </title>
    <meta name="Keywords" content="HTML,Kodluyoruz">
</HEAD> 
<BODY>
</BODY>
</html>
```
### BODY Etiketi
Web sayfamızda görmek istediğimiz bütün içerikleri `<body>` etiketi altına yazılır. Diğer etiketleri `<body>` etiketi içerisine yazılır.
```html
<html>   
<HEAD>
    <title> Sekmede Görülecek İsim </title>
    <meta name="Keywords" content="HTML,MADSoft">
</HEAD> 
<BODY>
    Site İçeriği
</BODY>
</html>
```
Not:

Şu ana kadar oluşturlan yapı idelerde kısayollar ile hızlıca oluşturulması mümkündür. Visual Studio Code (VSC) üzerinde "! + Enter" yazarak aşşağıdaki yapıyı hızlıca oluşturabilirsiniz.

`<!DOCTYPE html>` : Dökümanımızın HTML dilinde olduğunu tarayıcımıza bildiren talimattır.
`<html lang="en">` : Site içeriğinin dilini belirten etiket, "en" yerine "tr" yazılabilir.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>
```
#### H Etiketleri
H etiketleri başlık etiketleridir. Büyükten küçüğe sırasıyla
```html
<h1> 
<h2>
<h3>
<h4>
<h5>
<h6>
```
şeklindedir.

Not: HTML otomatik olarak Başlık etiketlerinin öncesine ve sonrasına satır atlatır.

#### P Etiketi
`<p>` etiketi paragraf etiketidir. Sayfa içerisinde oluşturmak istenilen metinleri `<p>` etiketi ile yapılır. Aşağıdaki örnekte hem başlık etiketi hemde paragraf etiketi kullanılmıştır.

Not: HTML otomatik olarak Paragraf etiketinin öncesine ve sonrasına satır atlatır.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2>Kodluyoruz</h2>
    <p>HTML Etiketleri</p>
</body>
</html>
```
#### br Etiketi
`<br>` etiketi satır atlatma etiketidir ve kapatmaya ihtiyaç duymayan etiketlerden biridir. Atlatmak istenilen satır sayısı kadar `<br>` etiketi kullanılır. <br /> NOT: BR etiketinin farklı kullanımlarını görebilirsiniz. örn.(`<br>`,`<br/>`,`<br />` Hepsi aynı işlevi yerine getirir.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2>MADSoft</h2> <br>
    <p>HTML <br> Etiketleri</p>
</body>
</html>
```
#### a Etiketi
`<a>` etiketinin en önemli özelliği href özelliğidir. Bu etiket ile sayfalar arası bağlantı kurabilirsiniz. Etiket içerisine yazılan içerik sayfa üzerinde gösterilecek içeriktir. href içine yazılan ise tıklandığında gideceği URL'dir.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <a href="https://www.madsoft.org">Madsoft</a>
</body>
</html>
```
#### ul - ol - li Etiketi
`<ul>` ve `<ol>` etiketleri liste oluşturma etiketleridir. Listeyi oluşturduktan sonra içeriğini oluşturmak için `<li>` etiketi kullanılır

`<ul>` = "unordered list" sırasız liste anlamına gelir. 
`<ol>` = "ordered list" sıralı liste anlamına gelir.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
   
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
    
    <ol>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ol>
    
</body>
</html>
```
#### hr Etiketi
`<hr>` etiketi ekrana yatay bir çizgi çizer. Bu etiket kapanmaya ihtiyaç duymaz.
```html
<!DOCTYPE html> <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
   
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
    
    <hr>
    
    <ol>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ol>
    
</body>
</html>
```
#### strong ve b Etiketi
`<strong>` etiketi bir metinin arama motorlarına önemli olduğunu bildirmek için kullanılır. Kullanıldığı zaman metini kalın yapar. Eğer sadece metini kalınlaştırmak isterseniz `<b>` etiketini kullanabilirsiniz.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2><strong> Kodluyoruz </strong></h2>
    <p><b> HTML </b> Etiketleri </p>
</body>
</html>
```
#### Script Etiketi
`<script>` etiketi JavaScript kodlarını HTML içerisine yazılabilmesini sağlar.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        document.write("MADSoft")
    </script>
</body>
</html>
```
#### button Etiketi
`<button>` etiketini buton oluşturmak için kullanılır. Buton üzerine yazmak istediğiniz içeriği etiketin içine yazmanız yeterlidir.
```html
<!DOCTYPE html> <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <button> Buton </button>
</body>
</html>
```
#### img Etiketi
Resim eklemek için `<img>` etiketini kullanılır. 
`<br> <img src=”resim.jpg” alt=”açıklama yazısı” />` 
src="" kısmına eklemek istediğimiz görselin yolunu yani kaynağını yazılır. Eğer görsel ve HTML dosyası aynı klasörde ise görselin adını ve uzantısı yazılması yeterlidir. alt="" kısmına görselin açıklamasını yazılır fakat tercihe bağlıdır boş bırakılabilir. Bu etiket kapanmaya ihtiyaç duymaz.
```html
<!DOCTYPE html> <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img src=”img/madsoftmain.jpg” alt=MADSoft Bootcamp” />
</body>
</html>
```
#### iframe Etiketi
Belge içinde belge gösterilmesini sağlayan etikettir. Genelde başka bir sitedeki belgeyi kendi sayfamızda göstermek için kullanılır. örn: Youtube'dan bir videoyu sayfamızda göstermek istersek `<iframe>` kodlarını sayfamıza eklememiz yeterlidir.
```html
<!DOCTYPE html> <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <iframe width="1519" height="581" src="https://www.youtube.com/watch?v=hGIW2fDb0jg" frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen></iframe>
</body>
</html>
```

#### Yorum Satırı
HTML dilinde yorum satırı`<!-- ile başlar -->` ile biter.
```html
<!DOCTYPE html> 
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- Örnek Yorum Satırı -->
    
    <!-- 
        1. Örnek Yorum Satırı 
    -->   
</body>
</html>
```
# Kaynaklar
[w3schools](https://www.w3schools.com/tags/default.asp)
[patika.dev](https://academy.patika.dev/)