##### Windows kullanıyorsun ve bilgisayarında keylogger bulunup bulunmadığını merak ediyorsun. Bunu en hızlı ve en temel şekilde öğrenebilmenin yolları var, biraz bundan konuşalım.


##### 1- Windows pencereni aç, oradan c: 'ye gir. Windows klasörüne tıkla, System 32'yi bul, System 32'nin içinde iki dosya aratacağız şimdi. SystemDll32.log, SystemDll32.exe .

![2](https://github.com/iclalsaritas/keyloggerr/assets/97543719/5cb24924-d939-4d5a-b2c8-9b11c9280b2f)
![1](https://github.com/iclalsaritas/keyloggerr/assets/97543719/f4784061-df97-48a4-ba17-2c35ae3ecc2f)

##### Bu iki dosyayı arattığında sonuç dönüyorsa nur topu gibi bir keylogger sahibisin. Dll dosyaları, birden fazla program tarafından kullanılabilen ve programların işlevselliğini genişleten işlevleri içerebilir, bu yüzden log ve onun execute versiyonunu arattık. 
##### 2- Klavyedeki dört farklı tuştan bahsedeceğim. CTRL+ALT+SHIFT+X tuşları. bu dördünü aynı anda tuşla. Tuşladın ve hiçbir değişiklik olmadı mı? Öyleyse güzel. Ekranda şifre soran bir pencere mi açıldı? Muhtemelen keylogger mağdurusun.
##### 3- Pencereye gel ve arama kutusuna çalıştır yaz. cmd yazıp enter yap ve terminal açılsın. Terminale netstat -an | ":25" yazıp enter yap. Temel olarak, bilgisayarın ağ bağlantılarını, ağ arayüzlerini, yönlendirme tablolarını ve ağ istatistiklerini görüntülemek için netstat komutunu kullandık. Netstat çıktısını belirli bir formatta göstermek için -an komutundan yararlandık. -a tüm bağlantıları ve bağlantı bekleyen noktaları gösterirken -n sayısal formatta (IP adresleri ve bağlantı noktaları) gösterir. Yani -an, IP adresleri ve bağlantı noktalarının sayısal değerlerini (IP adresleri ve port numaralarını) okunabilir bir formatta sunar. Ezcümle bu komutu uyguladığında bir şeyler listelenmeye başladıysa bilgisayarında keylogger yüksek ihtimalle var.
##### 4- Görev yöneticisini aç. Ayrıntılara gir, ayrıntılardan services.exe adındaki arkadaşı bul. Bu arkadaşın Kullanıcı adında SYSTEM dışında bir isim yazıyorsa keylogger ile başının dertte olması muhtemeldir.

##### Peki keylogger ile başım dertte, nasıl kurtulacağım ? Ya antivirüs programından faydalan ya da pc formatla. Muhtemelen sorun ortadan kalkacak, düzelme olmazsa forumda buluşalım. 

