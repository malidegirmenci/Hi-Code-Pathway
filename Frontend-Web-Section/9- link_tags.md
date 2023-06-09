# Linklerle Çalışmak
Bir HTML dosyası içerisinde herhangi bir sayfaya, sayfa içine, bir websitesine, e-mail, telefon adreslerine ya da dosya yolu belirtilen herhangi bir dosyaya (resim, video, zip vb.) erişmek için kullanılan HTML etiketidir. Genel yapısı `<a></a>` şeklindedir.

## a etiketi
`<a href="gitmek istenilen yer">Gidilecek yer için isim tanımlaması</a>`

HTML sayfalar arası geçiş yapmak için linkler kullanılır. Şu an üzerinde çalıştığımız klasörün içerisinde bir linksayfasi.html adında dosya mevcut ve içerisine bir şeyler yazılı olduğunu düşünün. Şimdi HTML'de sayfalar arası linkleme ile yeni oluşturduğumuz sayfaya gitmek için link oluşturacağız
`<a href="linksayfasi.html">İkinci sayfaya git</a>`
Bunu oluşturduğumuzda tarayıcı ekranımızda İkinci sayfaya git diye bir link oluşacak (üzerine gelindiğinde mousenin el işaretine dönmesinden anlaşılabilir)

### Sayfa içerisinde kullanımı

Sayfa içerisinde herhangi bir başlığa ya da bölüme gitmek için linkler kullanılabilir. Aynı sayfada işlem yapacağımız için birden fazla satır ekleyeceğim ve en aşağıya scroll ile kaydırmak yerine link yardımı ile gideceğim. Bunun için de gidilecek bölüm için a tagine name özelliği verilmelidir:
```html
<a href="#sonbolum">Aşağı Git</a>
--------------------------------- <--Sayfa Başı-->
---------------------------------
--------------------------------- <--Sayfa Sonu-->
<a name="sonbolum"></a>`
```
### Website yönlendirmesinde kullanımı:
a etiketinde href özelliğine verilen herhangi bir websitesi adresine kolayca gidilebilir. Burada target özelliğini göreceğiz. Bu özellik, gitmek istediğimiz bağlantının geçerli pencerede mi yoksa yeni bir pencerede mi açılması için kullanılır. _self özelliği geçerli pencerede açılması içindir. Varsayılan olarak böyledir. _blank özelliği ise yeni bir pencerede açılması içindir. Kodluyoruz'un internet sitesine gidelim
```html
<a  href="https://www.google.com" target="_self">Google</a>
<a  href="https://www.google.com" target="_blank">Google</a>
```
### Mail ve telefon yönlendirmesinde kullanımı
a etiketinin href özelliğine verilen mailto: ve tel: özellikleri sayesinde direkt olarak herhangi bir e-mail adresine posta gönderilebilir ya da geçerli bir telefon numarası aranabilir. Kodluyoruz'un e-mailine gidelim ve rastgele bir numaraya gidelim.

`<a href="mailto:info@kodluyoruz.org">Bize Yazın</a>`
`<<a href="mailto:054657874541">Tel No</a>`>