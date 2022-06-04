## KralWinSP'yi Windows Server 2008-2012-2016-2019-2022'de Çalıştırabilirsiniz ##
#### Bazı seçenekler düzgün çalışmayabilir ####
- ```KralWinSP.exe /unsafe```

## Windows 10 1903 ve sonraki sürümlerde Windows Defender nasıl devre dışı bırakılır ##
#### https://docs.microsoft.com/en-us/windows-hardware/customize/desktop/unattend/security-malware-windows-defender-disableantispyware "DisableAntiSpyware" artık üretilmiyor ve istemci cihazlarda yoksayılacak, 1903 sürümünden itibaren. ####

- GÜVENLİ MODDA yeniden başlatın
- Yürüt: ```KralWinSP.exe /disabledefender```

-VEYA-

- Yürütün: ```KralWinSP.exe /restart=disabledefender``` ve gerisini KralWinSP'in otomatik olarak yapmasına izin verin

## Windows Defender nasıl yeniden etkinleştirilir ##

- GÜVENLİ MODDA yeniden başlatın
- Yürüt: ```KralWinSP.exe /enabledefender```

-VEYA-

- Yürütün: ```KralWinSP.exe /restart=enabledefender``` ve gerisini KralWinSP'in otomatik olarak yapmasına izin verin

## GÜVENLİ MOD / NORMAL'de kolayca nasıl yeniden başlatılır ##

- ```KralWinSP.exe /restart=safemode```
- ```KralWinSP.exe /restart=normal```

## Aşağıdakileri kullanarak komut satırından sürüm bilgilerini görüntüleyin:

- ```KralWinSP.exe /version```

## Sorun giderme amacıyla belirli araçları devre dışı bırakabilirsiniz ##
#### Mevcut liste: ####

* Donanım inceleme programı (```indicium```)
* Ortak Uygulamalar indirme aracı (```apps```)
* HOSTS Editör aracı (```hosts```)
* UWP Uygulama Kaldırıcı (```uwp```)
* Başlangıç ​​öğeleri aracı (```startup```)
* Temizleyici yardımcı programı (```cleaner```)
* Entegratör aracı (```entegratör```)
* Pinger aracı (```pinger```)

#### Örnekler ####

- ```KralWinSP.exe /disable=indicium,uwp```
- ```KralWinSP.exe /disable=indicium,uwp,hosts```

## Optimize Ediciyi Sıfırla yapılandırması açılamadığında düzeltebilir ##
```KralWinSP.exe /reset```

## Windows Hazırda Bekletme işlevi komut satırından nasıl devre dışı bırakılır/etkinleştirilir ##

- ```KralWinSP.exe /disablehibernate```
- ```KralWinSP.exe /enablehibernate```

## Bir yapılandırma dosyasına göre ince ayarlar uygulayarak KralWinSP'yi sessizce çalıştırabilirsiniz. ##

Windows sürümünüze göre yapılandırma dosyasını indirin ve buna göre düzenleyin.

* ```true```: belirli seçeneği uygular
* ```false```: belirli seçeneği sıfırlar
* ```null```: belirli seçeneği yok sayar

Ardından, bunu şu şekilde yürütün: ```KralWinSP.exe /win10.conf```

### Windows 7 için: ###
https://github.com/Emre37destan/KralWinSP/blob/master/confs/win7.conf

### Windows 8/8.1 için: ###
https://github.com/Emre37destan/KralWinSP/blob/master/confs/win8.conf

### Windows 10 için: ###
https://github.com/Emre37destan/KralWinSP/blob/master/confs/win10.conf

### Windows 11 için: ###
https://github.com/Emre37destan/KralWinSP/blob/master/confs/win11.conf