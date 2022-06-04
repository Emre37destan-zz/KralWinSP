## Feed.json kullanılarak Ortak Uygulamalara bir uygulama nasıl eklenir: ##

* Hem x64 hem de x86 varyantları için doğrudan bağlantılara ihtiyacınız olacak (x64 veya x86 kullanılamıyorsa, birini kullanın)
* Resmi uygulama başlığı
* Bir etiket, genellikle uygulama başlığı - boşluksuz - önünde bir 'c'
* PNG resmi - en fazla 256x256 olmalı, boyutu 50 kb'yi geçmemeli ve şeffaf arka plana sahip olmalıdır
* Uygulamanın dahil edileceği grup

## Mevcut gruplar: ##

* Sistem Araçları
* İnternet
* Kodlama
* GrafikSes

## Örnek: ##

``` json
{
  "Başlık": "Google Chrome",
  "Bağlantı": "<link_x86>",
  "Link64": "<link_x64>",
  "Etiket": "cChrome",
  "Resim": "<link_to_png>",
  "Grup": "İnternet"
}
```
