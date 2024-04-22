#### Merhabalar, bu yazım basitçe keylogger tanımı, python ile keylogger genel mantığının gösterilmesi ve keylogger tespiti hakkında olacak.

##### Keylogger olarak bilinen bir yazılım, klavyenizdeki tuş vuruşlarını izleyen ve kaydeden bir tür izleme yazılımıdır. Bu yazılım, kullanıcıların klavyede ne yazdığını gizlice takip ederek, kullanıcıların etkinliklerini izlemeye ve kaydetmeye olanak tanır. Kullanım amacının ne olduğu tamamen kullanıcının sınırlarına ve neyi hedeflediğine bağlıdır. 

##### Python ile keylogger yazmayı ve kodu çalıştırdığımızda klavyedeki tüm tuşlamaların bir log.txt dosyasına kaydedilmesini istediğimizde bu tarz bir kod işimizi görebilir : 

![1](https://github.com/iclalsaritas/keylogger-tespiti/assets/97543719/78784547-ec84-4589-b703-906418f88ddb)

![2](https://github.com/iclalsaritas/keylogger-tespiti/assets/97543719/c26e32e2-7d23-423f-95f6-8737d1c09f24)




##### Windows kullanıyorsun ve bilgisayarında keylogger bulunup bulunmadığını merak ediyorsun. Bunu en hızlı ve en temel şekilde öğrenebilmenin yolları var, biraz bundan konuşalım.


##### 1- Windows pencereni aç, oradan c: 'ye gir. Windows klasörüne tıkla, System 32'yi bul, System 32'nin içinde iki dosya aratacağız şimdi. SystemDll32.log, SystemDll32.exe .


![2](https://github.com/iclalsaritas/keyloggerr/assets/97543719/5cb24924-d939-4d5a-b2c8-9b11c9280b2f)
![1](https://github.com/iclalsaritas/keyloggerr/assets/97543719/11020502-f17f-496e-b55f-0db6eaa88a9d)
##### Bu iki dosyayı arattığında sonuç dönüyorsa nur topu gibi bir keylogger sahibisin. Dll dosyaları, birden fazla program tarafından kullanılabilen ve programların işlevselliğini genişleten işlevleri içerebilir, bu yüzden log ve onun execute versiyonunu arattık. 
##### 2- Klavyedeki dört farklı tuştan bahsedeceğim. CTRL+ALT+SHIFT+X tuşları. bu dördünü aynı anda tuşla. Tuşladın ve hiçbir değişiklik olmadı mı? Öyleyse güzel. Ekranda şifre soran bir pencere mi açıldı? Muhtemelen keylogger mağdurusun.
##### 3- Pencereye gel ve arama kutusuna çalıştır yaz. cmd yazıp enter yap ve terminal açılsın. Terminale netstat -an | ":25" yazıp enter yap. Temel olarak, bilgisayarın ağ bağlantılarını, ağ arayüzlerini, yönlendirme tablolarını ve ağ istatistiklerini görüntülemek için netstat komutunu kullandık. Netstat çıktısını belirli bir formatta göstermek için -an komutundan yararlandık. -a tüm bağlantıları ve bağlantı bekleyen noktaları gösterirken -n sayısal formatta (IP adresleri ve bağlantı noktaları) gösterir. Yani -an, IP adresleri ve bağlantı noktalarının sayısal değerlerini (IP adresleri ve port numaralarını) okunabilir bir formatta sunar. 

![3](https://github.com/iclalsaritas/keyloggerr/assets/97543719/f9f47ac5-23f4-4c65-9627-01035f8e2d42)

![4](https://github.com/iclalsaritas/keyloggerr/assets/97543719/8e0ae490-d8ad-46bd-b494-ac3b7e30f13d)

##### Ezcümle bu komutu uyguladığında bir şeyler listelenmeye başladıysa bilgisayarında keylogger yüksek ihtimalle var.



##### 4- Görev yöneticisini aç. Ayrıntılara gir, ayrıntılardan services.exe adındaki arkadaşı bul.

![5](https://github.com/iclalsaritas/keyloggerr/assets/97543719/9ca72f0a-3c18-40a1-8465-d0b7f070a042)


![6](https://github.com/iclalsaritas/keyloggerr/assets/97543719/145ec8c3-2890-4e26-9dad-f809ad61c293)



##### Bu arkadaşın Kullanıcı adında SYSTEM dışında bir isim yazıyorsa keylogger ile başının dertte olması muhtemeldir.

##### // Peki keylogger ile başım dertte, nasıl kurtulacağım ? //
##### \\ Ya antivirüs programından faydalan ya da pc formatla. Muhtemelen sorun ortadan kalkacak, düzelme olmazsa forumda buluşalım. \\

