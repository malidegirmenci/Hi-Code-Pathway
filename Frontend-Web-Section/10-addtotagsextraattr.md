# Etiketlerine Ekstra Özellikler Eklemek
Bu ek özellikler Türkçe kaynaklarda HTML etiketlerinin nitelikleri, özellikleri veya öznitelikleri diye geçmektedir.

## Özellikleri:
Tüm HTML elementleri nitelik alabilirler.
Her zaman başlangıç elemanının içine yazılır.
<a href =""></a>
Bu nitelikler, etiketler konusunda ekstra özellik bilgisi sağlar.
Kelimeler arasında tire işareti koyarak(html-etiketi) veya camel case(htmlEtiketi) şeklinde kullanılabilir. HTML'de genellikle -(tire) kullanılır.
**class veya id gibi özniteliklerin ismi belirlerken Türkçe karakter tercih edilmemelidir. (ş,ç,ö,ü,ğ,büyük İ ve küçük ı)**
Kullanabilmek için özniteliği yazdıktan sonra ="" kullanılıp istediğimiz özelliği tırnakların içine yazılmalıdır..
İngilizce bir kaynakta aramak istiyorsanız "HTML attributes" diye aratmak gerekir.

`<img src ="" alt = "">`
HTML dosyasına bir resim eklemek istersek img etiketini kullanırız. img, İngilizcedeki image(resim) kelimesinin kısaltmasıdır. Bu etiketin yanında ise src ve alt özniteliklerini ekleyebiliriz. src **(source = kaynak)** ekleyeceğimiz resmi nereden alacağını belirttiğimiz yerdir. alt (alernative = alternatif) ise eğer bir nedenden resim görüntülenemez ise resme alternatif olarak ne yazması gerektiğidir.

`<a href =""></a>`
Eğer bir bağlantının URL sini vermek istiyorsak `<a>` (anchor) etiketini kullanırız. href teki iki tırnağın arası URL'yi girdiğimiz yerdir.

Her etikete id ve class özniteliklerini ekleyebiliriz.
```html
<img src ="" alt = "" id =""> 
<img src ="" alt = "" class ="" id ="">
<a href ="" id="" class ="" data-id ="" ></a>
```
## id (identity = kimlik)
id kullanılan etiketin kimliğini belirtir. Biriciktir*(unique)* yani dökümanın içindeki bir etikete yalnızca bir kez o id ismi verilebilir.
`<a href ="https://www.facebook.com/" id ="facebook-URL" ><a>`
Buradaki id yi kullanarak direkt olarak bu HTML etiketine ulaşabiliriz.

Not: id biricik olduğu için istisna olarak id = facebook-URL şeklinde yazarak tırnak işareti kullanmayabiliriz.

## class (sınıf)
class, HTML etkietinin hangi sınıfta olduğunu belirmemizi sağlar. Aynı sınıf adını birden fazla HTML etiketine verebiliriz.
`<img src ="" class ="documents"> <a href ="" class ="documents" ></a>`
Burada görüldüğü gibi iki HTML etiketi de(img ve a) documents sınıfında bulunmaktadır. Daha sonrasında aynı sınıfta bulunan bu iki etikete CSS ile aynı anda değişiklik yapılabilir.