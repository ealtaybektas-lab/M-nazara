10 KASIM AR ANMA - NETLIFY PROJESİ
===================================

DOSYALAR
- index.html: AR web uygulaması
- duvar-isareti.png: Duvara basılacak takip işareti örneği
- targets.mind: MindAR hedef dosyası (SİZİN OLUŞTURMANIZ GEREKİYOR)

ÖNEMLİ: Bu proje 2D tarihî fotoğrafı işaretin üzerine sabitler. Gerçek, etrafında dolaşılabilen 3D Atatürk modeli değildir.
Atatürk görseli Wikimedia Commons'taki tarihî fotoğraftır. Kaynak sayfası:
https://commons.wikimedia.org/wiki/File:Mustafa_Kemal_Ataturk.jpg
Wikimedia sayfasında Türkiye için kamu malı olarak işaretlenmiştir. Görsel URL'si HTML içindedir.

1) DUVAR İŞARETİNİ HAZIRLAMA
- duvar-isareti.png dosyasını A4 veya daha büyük boyutta, mat kâğıda, mümkünse 1200x900 oranını bozmadan yazdırın.
- Parlak laminasyon yansımayı artırabileceği için mat baskı tercih edin.
- İşaretin tamamı düz ve iyi aydınlatılmış bir duvara asılsın. Önüne eşya gelmesin.

2) TARGETS.MIND OLUŞTURMA (ZORUNLU)
- https://hiukim.github.io/mind-ar-js-doc/tools/compile/ adresini açın.
- duvar-isareti.png dosyasını yükleyin.
- Compile/Start işlemini başlatın.
- İşlem bitince .mind dosyasını indirin.
- İndirdiğiniz dosyanın adını tam olarak targets.mind yapın.
- targets.mind dosyasını index.html ile aynı klasöre koyun.

Bu adım olmadan kamera açılır ama duvar işaretini tanıyamaz.

3) NETLIFY'A YÜKLEME
- Bu klasörde index.html, duvar-isareti.png ve targets.mind birlikte bulunmalı.
- https://app.netlify.com/drop adresine girin.
- Üç dosyayı içeren klasörü (veya ZIP'i açıp klasörü) Netlify Drop alanına sürükleyin.
- Netlify size https://....netlify.app biçiminde bir adres verir.
- Telefonla bu adresi açın; kamera izni verin.

4) QR KOD
- Netlify adresiniz oluştuktan sonra o adresi bir QR kod üreticisine girin.
- QR kodu etkinlik alanına asın. QR kod yalnızca siteyi açar; AR takip işareti ayrı olan duvar-isareti.png'dir.
- Ziyaretçi QR'ı okutur, sayfada Kamerayı Aç'a basar ve duvar işaretini gösterir.

5) TEST
- Önce aynı telefonla, gerçek etkinlik alanına gitmeden test edin.
- iPhone: Safari; Android: Chrome önerilir.
- Kamera izni ve HTTPS gerekir.
- İşareti çok uzaktan göstermeyin; iyi ışıkta, yansımayı önleyerek deneyin.
- Fotoğraf çekme düğmesi AR görüntü tuvalini PNG olarak indirmeyi dener. Bazı telefon/tarayıcı kombinasyonlarında tarayıcı güvenlik kısıtlamaları nedeniyle indirme çalışmayabilir; etkinlikten önce mutlaka test edin.

ATATÜRK GÖRSELİ / 3D MODEL NOTU
Bu sürüm, tarihî fotoğrafı işarete bağlı bir düzlem olarak gösterir. Gerçekçi 3D Atatürk için lisanslı/izinli bir .glb model gerekir. Böyle bir model bulunduğunda fotoğraf düzlemi kaldırılıp a-gltf-model eklenebilir; ancak modelin doğru ölçek, yön ve animasyon ayarı ayrıca yapılmalıdır.

MindAR dokümantasyonu:
https://hiukim.github.io/mind-ar-js-doc/quick-start/overview/
