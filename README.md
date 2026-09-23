# Cep Langırtı

Telefonda oynanan langırt (kicker) oyunu. Tek bir `index.html` dosyasından oluşur; kurulum, kütüphane ya da derleme adımı yoktur.

## Nasıl oynanır

Üç mod var: **Bilgisayara karşı** (mavi takım sensin, kırmızıyı bilgisayar oynar), **2 kişi** (aynı telefonda arkadaşınla) ve **Online** (iki ayrı telefonda arkadaşınla). Seçtiğin gol sayısına (3, 5 ya da 7) ilk ulaşan maçı kazanır.

| Kontrol | Ne yapar |
| --- | --- |
| **▲ / ▼** (sol başparmak) | Aktif çubuğu (pirinç renkte parlayan çubuk) yukarı / aşağı kaydırır. Parmağını kaldırmadan ▲ ile ▼ arasında kaydırabilirsin. |
| **ŞUT** (sağ başparmak), dokun | Aktif çubuğun adamları hızlıca döner ve topa vurur. |
| **ŞUT**, basılı tut | Adamlar geriye yatar ve güç toplar (tuşun çevresindeki halka dolar). Bıraktığında daha sert vurur. |
| Vururken ▲/▼ | Kayan çubuk sürtünmeyle topa yan hız verir, top çapraz gider. |
| Ayağın kenarıyla vurmak | Ayak yuvarlak olduğu için top açılı seker. |
| Arka | Top aktif çubuğun hemen arkasında (1,2–6 cm) kaldıysa ŞUT'a bas: adamlar öne doğru tam tur döner, ayak topun arkasına iner ve topu ileri sürer. |
| **SÜPER** (ŞUT'un üstünde) | Göstergen dolunca süper şutu hazırlar; bir sonraki vuruşun süper şut olur (aşağıya bak). |
| **DEV** (ŞUT'un altında) | Kendi göstergesi dolunca kalecin 6 saniyeliğine dev olur (aşağıya bak). |
| **💬** (sol üst) | Rakibine laf atmak için ifade menüsünü açar (aşağıya bak). |

### Aktif çubuk

İsteğe bağlı bir özelliktir ve açık gelir. Menüdeki **Aktif çubuk** anahtarından ya da moladaki **Aktif çubuk** düğmesinden kapatabilirsin; seçimin hatırlanır.

- **Açık:** Yalnızca topa en yakın çubuk kayar ve vurur (ayrıntılar aşağıda).
- **Kapalı:** Bütün çubukların birlikte kayar ve birlikte vurur. Her çubuk kendi yol aralığının aynı oranında kayar, böylece çubuklar birbirinden kopmaz. Maç ortasında kapatırsan çubuklar yumuşakça aynı hizaya gelir. Bu modda kaleci zaten elinle birlikte hareket ettiği için otomatik kaleci devre dışıdır.
- 2 kişilik modda ayar iki oyuncuya da uygulanır. Bilgisayar her zaman aktif çubukla oynar.

Açıkken her an yalnızca bir çubuğunu kontrol edersin: topa en yakın ve topu önüne alabilecek çubuğu. Top başka bir çubuğun bölgesine geçince kontrol de kendiliğinden o çubuğa geçer. Diğer çubukların, bıraktığın yerde kalır.

- Top adamlarının arkasındaysa arkadaki çubuk için ek mesafe sayılır. Bu yüzden kontrol, topu ileri vurabilecek çubukta kalır.
- Top hızla kendi kalene geliyorsa kontrol, topun henüz geçmediği ilk çubuğa verilir.
- Kendi pasın ya da şutun ileri giderken kontrol, topun varacağı sıradaki çubuğuna geçer. Böylece o çubuğu top gelmeden hizalayabilirsin.
- Kontrol yalnızca güç toplarken ve vuruşun topa değebildiği kısa anda kilitli kalır. Adamlar topun üstüne kalkar kalkmaz kontrol sıradaki çubuğa geçebilir; vuran çubuk kendi kendine dikey konuma döner.
- Yeni çubuk açıkça daha uygunsa kontrol hemen geçer. Top iki çubuğun tam ortasında duruyorsa, titremesin diye kısa bir süre (0,06 sn) beklenir.
- Top yavaşlarken kontrolün iki çubuk arasında gidip gelmemesi için hız eşiklerinin açılma ve kapanma değerleri farklıdır: ileri pas 700 mm/s'de başlar, 350 mm/s'de biter.
- Bilgisayar da aynı kuralla oynar: o da aynı anda tek çubuğunu yönetir.

### Otomatik kaleci

Kontrol başka bir çubuktayken kalecin topu kendiliğinden izler. Böylece sert bir şutta kontrol kaleciye geçtiğinde kaleci boş kalenin kenarında beklemiyor olur. Yardım bilerek sınırlı tutuldu:

- Topu 0,25 saniye gecikmeyle görür, topun gideceği yeri tahmin etmez.
- Senin el hızının %45'iyle kayar.
- Kale ağzının dışına çıkmaz. Topu yalnızca kısmen izler: top şut menzilindeyken yaklaşık üçte iki oranında, uzaktayken daha az. Bu yüzden köşeler açık kalır.
- Kontrol kaleciye geçtiği anda kaleciyi yine sen oynarsın.

Açık gelir; kapatmak için menüdeki **Otomatik kaleci** anahtarını ya da moladaki **Oto kaleci** düğmesini kullan. Yalnızca aktif çubuk açıkken çalışır. Seçimin hatırlanır. Bilgisayara karşı modda yalnızca senin takımına, 2 kişilik modda iki takıma da uygulanır.

### Süper şut

Her takımın bir süper şut göstergesi vardır. Gösterge top oyundayken 40 saniyede dolar; gol yiyen takımın göstergesine ayrıca %30 eklenir.

- **Hazırlama:** Gösterge dolunca **SÜPER** tuşu turuncu parlar ve skor tabelasında takımın yanındaki şimşek yanar. Tuşa basınca süper şut hazırlanır: ŞUT tuşu da turuncu çerçeve alır. Dolmadan basarsan bir şey olmaz.
- **Ateşleme:** Hazırlanan süper, bir sonraki gerçek ileri vuruşunda ateşlenir. Tam tur (arka) vuruşu ya da yana giden vuruş onu harcamaz. Kullanınca gösterge sıfırlanır.
- **Etkisi:** Top normal şutun yaklaşık 1,5 katı hızla (en az 3,8 m/s) kaymadan gider. Rakibin defans, orta saha ve forvet adamlarının içinden geçer; geçtiği adamlar bir anlığına soluklaşır. Turuncu iz ve parıltı bırakır, gol olursa "Süper gol!" yazar.
- **Sınırları:** Kaleci süper şutu durdurabilir; kaleci dokunduğu an süper biter. Duvardan sekebilir. Hızı 1,5 m/s'nin altına düşünce ya da 1,6 saniye sonra normal topa döner.
- **Bilgisayar:** Aynı göstergeyle oynar ve süperini forvetiyle vururken kullanır. İki kişilik modda iki oyuncunun da ayrı göstergesi ve SÜPER tuşu vardır.

Menüdeki **Süper şut** anahtarıyla kapatılabilir; açık gelir ve seçimin hatırlanır. Kapalıyken tuşlar ve göstergeler gizlenir.

Simülasyonda gösterge 40 saniyede dolarken gollerin yaklaşık %30'u süper şuttan geldi. 22 saniyelik dolumla bu oran yarıyı geçiyordu ve oyun göstergeye bağlı kalıyordu.

### Dev kaleci

Süper şuttan ayrı, ikinci bir güçtür ve kendi göstergesi vardır. Gösterge top oyundayken 55 saniyede dolar; gol yiyen takıma %20 ek dolum verir.

- **Kullanma:** Gösterge dolunca **DEV** tuşu turkuaz parlar ve tabelada takımın yanındaki kalkan yanar. Basınca kaleci hemen büyür; hazırlama adımı yoktur.
- **Etkisi:** Kaleci 6 saniye boyunca çubuk boyunca yaklaşık 2,4 kat, derinlikte biraz genişler; etrafında turkuaz bir hale belirir. Bu sürede tuşun halkası kalan süreyi gösterir. Süre bitince kaleci küçülür ve gösterge yeniden dolmaya başlar.
- **Sınırları:** Kalecinin yine topla hizalanması gerekir; yalnızca kalenin çok daha büyük kısmını kapatır, bu yüzden kenara kaçan şutlar girebilir. Süper şutu durdurabilir; bu yüzden süper şutun doğal karşılığıdır.
- **Tuşların yeri:** Tek kişilik modda DEV tuşu, sol başparmak ▲▼'dan kalkmasın diye sağda ŞUT'un altında; SÜPER üstünde. İki kişilik modda her oyuncunun sütununun altında SÜPER ve DEV yan yana durur.
- **Bilgisayar:** Aynı göstergeyle oynar ve dev kalecisini senin süperin hazırken, top senin forvetindeyken ya da kalesine sert bir şut gelirken kullanır.

Menüdeki **Dev kaleci** anahtarıyla kapatılabilir; açık gelir ve seçimin hatırlanır.

Simülasyonda dev kaleci açıkken toplam gol yaklaşık %19, süper gol yaklaşık üçte bir azaldı. İlk denenen ayarda (7 saniye, 45 saniyede dolum) goller %35 azalıyordu; bu yüzden süre kısaltıldı, dolum yavaşlatıldı.

### Maç içi ifadeler (psikolojik harp)

Sol üstteki **💬** tuşu sekiz ifadelik bir menü açar. Seçtiğin ifade, masada senin kalenin olduğu uçta, takım renginde bir baloncuk ve kısa bir sesle belirir.

- **İfadeler:** 😂 Hahaha!, 😎 Çok kolay, 🥱 Uyuma!, 🧱 Geçemezsin, 🔥 Geliyor…, 🍀 Şans işte, 👏 İyi gol, 😤 Bekle sen!
- **Nerede görünür:** Baloncuk masanın üst kenarında 2,4 saniye kalır. Kendi ifaden solda, rakibinki sağda çıkar. Maç sonu ekranında kartın üstünde görünür.
- **Bekleme:** İki ifade arasında 2,5 saniye beklenir; bu sürede 💬 tuşunun halkası dolar. Menü, 4 saniye içinde seçim yapılmazsa ya da başka bir yere dokunulursa kapanır.
- **Gol sonrası:** Gol attığında 💬 tuşu 3 saniye parlar: laf atmanın tam zamanı.
- **Bilgisayar:** Bilgisayar da laf atar ve seviyesine göre konuşur. Acemi kibardır: kendi golüne "Şans işte", seninkine "İyi gol" der. Kulüp dengelidir. Usta kendini beğenmiştir: "Çok kolay", "Uyuma!". Gol atınca, gol yiyince, kalecisi sert bir şutu kurtarınca, süper şutunu hazırlayınca ve senin lafına cevap olarak konuşur, ama en fazla 7 saniyede bir. Maç bitince de kazandıysa ya da kaybettiyse bir şey söyler.
- **2 kişi:** Her oyuncunun kendi 💬 tuşu vardır: mavininki sol üstte, kırmızınınki sağ üstte mola tuşunun yanında. Bir oyuncunun menüsü, diğerinin tuşlara basmasıyla kapanmaz.
- **Online:** İfade rakibin telefonunda da görünür. Maç bitince sonuç ekranından da ifade gönderilebilir. Masayı açan telefon, rakipten saniyede birden sık gelen ifadeleri göstermez.
- **Kapatma:** Mola ekranındaki **İfadeler** tuşuyla kapatılır. Kapalıyken ne ifade gönderirsin ne de rakibinkini görürsün; bilgisayar da susar. Seçim hatırlanır.
- **Oyuna etkisi:** Yoktur; ifadeler yalnızca görüntü ve sestir.
- **Klavye:** `1`–`8` tuşları ifadeleri sırasıyla gönderir. 2 kişilik modda kırmızı için sayısal tuş takımındaki `1`–`8` kullanılır.

### Sesli spiker

Maçı Türkçe bir spiker anlatır. Telefonun kendi konuşma motoru kullanılır (Web Speech API); dosya indirilmez, internet gerekmez. iPhone'da Türkçe ses hazır gelir.

- **Ne zaman konuşur:** Maç başlangıcı, goller (kendi kalesine gol, süper gol, eşitlik, öne geçme, fark açma, maç topu), süper şut, kaleye 1,8 m/s'den hızlı gelen şutun kurtarılması, dev kaleci, ölü top ve son düdük. Uzun süre bir şey olmazsa ara sıra yorum yapar ("Orta sahada kıyasıya bir mücadele var.").
- **Kimi anar:** Seni Tablo sekmesindeki adınla anar. Rakibi seviyesiyle ("Usta bilgisayar") ya da online'da arkadaşının adıyla anar; 2 kişilik modda "Mavi" ve "Kırmızı" der. Skoru kelimeyle okur ("iki bir"). Kupa finalinde şampiyonu ilan eder.
- **Sıra:** Gol ve son düdük konuşmayı keser. Küçük anlar, bir cümle sürerken gelirse söylenmez; cümleler üst üste binmez. Aynı cümle arka arkaya tekrarlanmaz.
- **Altyazı:** Söylenen her cümle ekranın altında altyazı olarak da çıkar. Ses kapalıyken ya da cihazda Türkçe ses yoksa spiker yalnızca altyazı gösterir; Türkçe metni İngilizce sesle okumaz.
- **Online:** Her telefon maçı kendi açısından anlatır.
- **Kapatma:** Mola ekranındaki **Spiker** tuşu; seçim hatırlanır. **Ses: kapalı** spikeri de susturur. Molada ve uygulamadan çıkınca susar.

### Paylaşım kartı (Instagram / WhatsApp)

Maç bitince sonuç ekranındaki **Paylaş** tuşu, maçın görselini telefonun paylaşım menüsüne verir. Oradan tek dokunuşla Instagram hikâyesine, WhatsApp'a (sohbet ya da durum) veya başka bir uygulamaya gönderilir.

- **Boyut:** 1080 × 1920, hikâyelerin boyutu. JPEG, yaklaşık 200 KB.
- **İçinde ne var:**
  - Sonuç ("Kazandım!", "Kaybettim" ya da "Mavi kazandı!") ve maça göre bir alt başlık: "Gol yemeden kazandım!", "Geriden gelip kazandım!", "Usta bilgisayarı devirdim!", "Kıl payı ama benim!", "Rövanş geliyor…" gibi.
  - Büyük skor; kendi takımın solda.
  - Gollerin atılış sırası: süper gol turuncu halkalı, kendi kalesine gol içi boş.
  - Masanın kendisi; son gol kaybedenin kalesinde.
  - Süre, en uzun gol serisi, kalecinin kurtarışları (kaleye 1,8 m/s'den hızlı gelen şutlar) ve süper gol sayısı.
  - "Sen de oyna" ile oyunun adresi ve tarih.
- **Kimin açısından:** Bilgisayara karşı ve online maçta senin açından; online'da iki telefon da kendi kartını hazırlar. 2 kişilik modda kazananın açından.
- **Hikâye alanı:** Önemli yazılar, Instagram'ın üstteki profil satırının ve alttaki mesaj çubuğunun altında kalmayacak şekilde ortada durur.
- **claude.ai sayfasında:** Görsel, sayfanın indirme izniyle verilir: Claude iPhone uygulamasında paylaşım menüsü, tarayıcıda indirme onayı açılır.
- **Paylaşılamayan yerde:** Görsel dosya olarak paylaşılamazsa (örneğin bir bilgisayar tarayıcısında) kart ekranda açılır; basılı tutup kaydedebilir ya da **İndir**'e basabilirsin.
- **Neden yalnızca görsel:** Yanına yazı eklenince bazı uygulamalar (Instagram gibi) paylaşım menüsünde görünmüyor. Oyunun adresi görselin üstünde yazılı.
- Görsel maç biter bitmez hazırlanır; bu yüzden tuşa basınca paylaşım menüsü hemen açılır.

### Oyuncu profili ve istatistikler

Menünün sol üstünde avatarın, adın ve seviyen durur; dokununca görevler ekranının **Profil** sekmesi açılır.

- **Kimlik:** 16 emoji arasından avatar seçilir (avatara dokun). Ad buradan ya da Tablo sekmesinden değiştirilir; ikisi aynı addır.
- **Seviye:** Maçlardan kazanılan deneyimle yükselir.
  - XP: maç 10, galibiyet 25, gol 3, süper gol 5, gol yemeden galibiyet 15, geri dönüş 20, kupa şampiyonluğu 100, günlük görev 10.
  - Bir sonraki seviye için gereken XP her seviyede 50 artar (100, 150, 200…). Seviye 2 yaklaşık 3 maçta, seviye 5 yirmi küsur maçta gelir.
  - Unvanlar: Çaylak (1), Amatör (3), Yetenekli (5), Profesyonel (8), Yıldız (12), Usta (17), Efsane (23).
  - Seviye atlanınca maç sonunda "⬆️ Seviye 5: Yetenekli!" yazar.
  - XP, zaten tutulan toplam sayılardan hesaplanır; bu yüzden profilden önce oynayanlar kazandıkları seviyeyle başlar.
- **Özet:** Rozet, kupa, açılan tema ve en iyi günlük seri.
- **İstatistikler:**
  - Maç ve toplam oynama süresi; galibiyet ve kazanma yüzdesi; mağlubiyet.
  - Atılan ve yenilen gol, maç başı ortalamalarıyla.
  - Süper gol, kurtarış, gol yemeden galibiyet, geri dönüş, en uzun gol serisi, en farklı galibiyet ve kupa şampiyonlukları.
- **Rakibe göre:** Acemi, Kulüp, Usta ve online için galibiyet–mağlubiyet, yeşil bir kazanma çubuğuyla.
- **Son maçlar:** Son 10 maç, "G 3–1" ya da "M 0–3" olarak; bilgisayar seviyesi, online ya da kupa işaretiyle.
- **Ne sayılır:** Görevlerdeki gibi bilgisayara karşı ve online maçlar, maç bitince, kendi tarafından sayılır; 2 kişilik maçlar sayılmaz.
  - Profilden önce tutulmayan sayılar profil geldikten sonra başlar: yenilen gol, oynama süresi, rakibe göre kayıt, en farklı galibiyet ve son maçlar.
  - Yenilen gol ortalaması yalnızca bu maçlar üzerinden hesaplanır.

### Günlük görevler ve rozetler

Ana menüdeki **🎯 0/3 · ⭐ 0** düğmesi görevler, rozetler, temalar, kupa ve tablo ekranını açar (yanındaki **🏆** doğrudan kupaya gider); sağ üstte kaç yıldızın olduğu yazar. Maç sonu ekranında da o maçta tamamlanan görevler ve kazanılan rozetler görünür; onlara dokununca aynı ekran açılır.

- **Günlük görevler:** Her gün üç görev gelir: bir kolay (1⭐), bir orta (2⭐), bir zor (3⭐). Görevler tarihe göre seçilir, yani aynı gün herkes aynı görevleri alır; arkadaşınla yarışabilirsin. Gece yarısı yenilenir.
  - Kolay: bir maç bitir, bir maç kazan, 3 gol at, kalecinle 3 kurtarış yap, rakibine 3 ifade gönder.
  - Orta: 2 maç kazan, 8 gol at, süper şutla gol at, dev kaleciyi 2 kez kullan, Kulüp ya da Usta bilgisayarı yen, bir maçta üst üste 3 gol at, bir sonuç kartı paylaş.
  - Zor: gol yemeden bir maç kazan, Usta bilgisayarı yen, 2 gol geriden gelip kazan, bir maçta 2 süper gol at, bir maçta 3 kurtarış yap, 7 gollük bir maç kazan.
- **Günün bütün görevleri:** Üçü de bitince +2⭐ bonus gelir ve günlük seri 🔥 bir gün uzar. Bir gün atlanırsa seri sıfırlanır; en iyi seri saklanır.
- **Rozetler:** 17 rozet var. Çoğu üç seviyelidir: bronz (I), gümüş (II), altın (III). Bir rozete dokununca nasıl kazanıldığı ve ne kadar kaldığı görünür.

  | Rozet | I / II / III |
  | --- | --- |
  | 🏆 Galip | 1 / 10 / 50 maç kazan |
  | ⚽ Golcü | 10 / 100 / 500 gol at |
  | ⚡ Süper yıldız | 1 / 10 / 50 süper gol at |
  | 🧤 Eldiven | 10 / 50 / 200 kurtarış yap |
  | 🧱 Kale duvarı | Gol yemeden 1 / 5 / 25 maç kazan |
  | 🔄 Geri dönüş | 2 gol geriden gelip 1 / 5 / 20 maç kazan |
  | 🔥 Seri | Bir maçta üst üste 3 / 5 / 7 gol at |
  | 🤖 Makineyi yen | Acemi / Kulüp / Usta bilgisayarı yen |
  | 🌐 Online savaşçı | Online 1 / 10 / 50 maç kazan |
  | 🛡️ Dev duvar | Dev kaleciyle 1 / 5 / 20 süper şut durdur |
  | 😂 Psikolojik harp | 10 / 100 / 500 ifade gönder |
  | 📣 Viral | 1 / 10 / 50 sonuç kartı paylaş |
  | 🎯 Görev avcısı | 5 / 50 / 200 günlük görev tamamla |
  | 🗓️ Sadık oyuncu | 3 / 7 / 30 gün üst üste bütün görevleri bitir |
  | 💎 Kusursuz | 7 gollük maçı gol yemeden kazan (tek seviye) |
  | 🥇 Kupa şampiyonu | Haftalık kupayı 1 / 5 / 20 kez kazan |
  | 🎨 Koleksiyoncu | Yıldızlarla 1 / 4 / 10 tema aç |

- **Ne sayılır:**
  - Bilgisayara karşı ve online maçlar, maç bitince kendi tarafından sayılır; online'da iki telefon da kendi ilerlemesini tutar. Yarıda bırakılan maç sayılmaz.
  - 2 kişilik maçlar sayılmaz; tek başına iki tarafı oynayıp görev toplamak çok kolay olurdu.
  - Kendi kalesine atılan gol, golü kazanan tarafa "gol" olarak yazılmaz.
  - Kurtarış: kaleye 1,8 m/s'den hızlı gelen bir şutu kalecinin durdurması. Bilgisayarlar arası denemelerde bir maçta genelde 0–3 kurtarış oluyor; görev hedefleri buna göre seçildi.
  - İfade ve paylaşım görevleri anında ilerler. Paylaşım, paylaşım menüsünden bir uygulamaya gönderince ya da **İndir**'e basınca sayılır; her maçın kartı bir kez sayılır.
- **Saklama:** İlerleme o tarayıcıda saklanır (`localStorage`). Safari'de açılan oyun ile ana ekrana eklenen oyunun depoları ayrıdır; hep aynı yerden oyna. Tarayıcı verileri silinirse ilerleme de silinir.

### Temalar (yıldızla açılır)

Görevlerden kazanılan yıldızlar, görevler ekranının **Temalar** sekmesinde top ve masa temalarına harcanır. Açılan tema kalıcıdır; istediğin zaman başka bir açık temaya geçebilirsin.

| Top | ⭐ | Masa | ⭐ |
| --- | --- | --- | --- |
| Klasik (krem, kahve benekli) | ücretsiz | Klasik (yeşil çuha, kayın) | ücretsiz |
| Turuncu | 5 | Gece (lacivert çuha, ceviz) | 8 |
| Futbol (siyah beşgenli beyaz top) | 12 | Çim (şeritli çim, beyaz çerçeve) | 15 |
| Neon (yeşil, parlayan) | 20 | Bordo (bordo kadife, kiraz) | 30 |
| Altın (parlayan) | 35 | Buz (buz mavisi, gümüş) | 50 |
| Ateş topu (kızıl, parlayan, uzun iz) | 60 | Altın Salon (siyah çuha, altın çizgiler) | 90 |

- **Satın alma:** Kilitli bir temaya dokununca fiyatı sorulur; bir kez daha dokununca yıldızlar harcanır ve tema seçilir. Yıldızın yetmiyorsa kaç yıldız daha lazım olduğu yazar.
- **Nerede görünür:** Oyunda, menünün arkasındaki masada ve paylaşım kartında. Online'da her telefon kendi seçtiği temayı görür.
- **Oyuna etkisi:** Yoktur; yalnızca görünüş değişir. Süper şut hâlâ turuncu parlar; takım renkleri hep mavi ve kırmızıdır.
- **Ekonomi:** Bir günde görevlerden en çok 8⭐ kazanılır (1 + 2 + 3 + 2 bonus). Böylece ilk temalar birkaç günde, Altın Salon birkaç haftada açılır. Maç sonunda yeni bir temaya yetecek yıldızın olunca "🎨 Yeni tema açabilirsin" yazar.
- Açılan temalar ve seçimin, görev ilerlemesiyle birlikte bu tarayıcıda saklanır.

### Haftalık kupa ve liderlik tablosu

Menüdeki **🏆** düğmesi (ya da görevler ekranındaki **Kupa** sekmesi) haftanın kupasını açar.

- **Kupa:** Bilgisayara karşı üç tur oynanır: çeyrek final (Acemi, 100 puan), yarı final (Kulüp, 200 puan), final (Usta, 400 puan). Kazanılan maç, turun puanına ek olarak gol farkı başına 20 puan getirir; gol yenmezse 50 puan daha eklenir. Kaybedince koşu biter; o maçta atılan her gol 10 puan sayılır ve toplanan puan kalır.
- **Haftanın kuralı:** Her hafta beş kupadan biri gelir. Seçim haftaya göre yapıldığı için aynı hafta herkes aynı kupayı oynar.
  - Klasik Kupa: 5 gollük maçlar.
  - Hızlı Kupa: 3 gollük maçlar.
  - Süper Kupa: süper şut göstergesi iki kat hızlı dolar.
  - Dev Kupa: dev kaleci göstergesi iki kat hızlı dolar.
  - Maraton Kupası: 7 gollük maçlar.

  Kupa maçlarında süper şut ve dev kaleci her zaman açıktır. Rakip seviyesi turdan gelir. Kupadan çıkınca kendi ayarların geri gelir.
- **Puan:** Kupa istediğin kadar yeniden oynanabilir; haftanın en iyi koşusu sayılır. Sonuç ekranında "▶ Yarı final" tuşu sonraki tura, "Yeni koşu" yeni bir kupaya başlatır. Kupa maçında "Baştan başlat" yoktur. Maçı yarıda bırakmak ya da uygulamayı kapatmak o maçı kaybetmek sayılır.
- **Ödül:** Haftanın ilk şampiyonluğu +5⭐ getirir ve 🥇 Kupa şampiyonu rozetine sayılır. Kupa finali kazanılınca paylaşım kartında "Haftanın kupası benim!" yazar.
- **Tablo:** Tablo sekmesinde haftanın sıralaması iki görünümle gösterilir.
  - Kupa puanı: haftanın en iyi koşusu ve ulaşılan tur.
  - Online lig: bu hafta online maçlarda alınan galibiyet ve mağlubiyetler; galibiyet 3 puan.
  - Adını buradan değiştirebilirsin (en fazla 14 karakter).
- **Sunucu yok:** Oyun GitHub Pages'te durduğu için herkesin skorunu toplayan bir sunucu yoktur. Tabloda sen ve online oynadığın arkadaşların görünür.
  - İki telefon online bağlanınca tablolarını birbirine aktarır. Her satır için daha yeni olan kopya kalır, böylece arkadaşının oynadığı kişiler de sana gelir.
  - Her oyuncunun satırını yalnızca kendi telefonu değiştirir; başka bir telefondan gelen satır seninkinin yerine geçemez.
  - Gelen satırlar denetlenir: adlar düz yazı olarak gösterilir, sayılar makul sınırlara çekilir, en fazla 40 satır tutulur.
  - Tablo ve kupa her pazartesi 00:00'da (telefonun saatiyle) sıfırlanır.
  - Herkesin birbirini görebildiği küresel tablo için aşağıdaki **Dünya tablosu** bölümüne bak.

### Dünya tablosu (Firebase)

Bir Firebase projesi bağlanınca Tablo sekmesinde **Arkadaşlar / 🌍 Dünya** seçimi çıkar. Dünya görünümünde, o hafta kupa ya da online maç oynayan herkes aynı tabloda sıralanır.

- **Ne gösterir:** Haftanın ilk 50 oyuncusu, kupa puanına ya da online galibiyete göre. İlk 50'de değilsen kendi satırın ve sıran altta görünür, örneğin "Sıran: 49 / 56 oyuncu". Liste açılınca kendi satırına kayar.
- **Ne gönderilir:** Yalnızca adın, haftanın en iyi kupa puanı ve ulaştığın tur, online galibiyet ve mağlubiyetlerin. Bunlar değişince birkaç saniye içinde, internet yoksa sonra gönderilir. O hafta hiç oynamayan oyuncu tabloya girmez.
- **İstemeyen için:** Tablo sekmesindeki **Dünya tablosunda görün** anahtarı kapatılınca satırın silinir ve bir daha gönderilmez; diğerlerini yine görebilirsin.
- **Hesap:** Her telefon Firebase'e anonim olarak girer; e-posta ya da şifre yoktur. Hesap tarayıcıda saklanır, tarayıcı verileri silinirse yeni bir hesap açılır.
- **Güvenlik** ([`firestore.rules`](firestore.rules)):
  - Herkes tabloyu okuyabilir; herkes yalnızca kendi satırını yazıp silebilir.
  - Ad 1–14 karakter olmalı. Kupa puanı 0–1300 arasında olmalı; en iyi kupa koşusu 1270 puandır. Galibiyet ve mağlubiyet en çok 500 olabilir. Başka alan eklenemez.
  - Aynı hafta içinde puan, tur, galibiyet ve mağlubiyet düşürülemez. Bir satır en fazla 10 saniyede bir yazılabilir. Zaman damgasını sunucu koyar.
  - Oyun telefonda çalıştığı için değiştirilmiş bir oyunla kurallara uyan ama sahte bir puan göndermek yine de mümkündür; bu tür tablolarda bu önlenemez. Adlar denetlenmez, yalnızca düz yazı olarak gösterilir.
- **Sınırlar:** Firebase'in ücretsiz planı günde 50.000 okuma ve 20.000 yazma verir. Dünya görünümü bir açılışta yaklaşık 50 okuma yapar ve bir dakika önbellekte tutulur; arkadaş ölçeğinde fazlasıyla yeter.
- **claude.ai sayfası:** Dünya tablosu herkese açık adreste (GitHub Pages) çalışır; claude.ai sayfası dışarıya bağlanamayabilir.

Oyun `ceplangirti` Firebase projesine bağlı; aşağıdaki adımlar bu proje için yapıldı ve başka bir projeye geçmek gerekirse diye duruyor.

**Kurulum (bir kez, yaklaşık 10 dakika):**
1. [console.firebase.google.com](https://console.firebase.google.com) adresinde **Proje oluştur**'a bas, projeye bir ad ver (örneğin `cep-langirti`). Google Analytics'i kapatabilirsin.
2. **Authentication → Başlayın → Sign-in method** bölümünde **Anonim** (Anonymous) girişi aç ve kaydet.
3. **Firestore Database → Veritabanı oluştur** de; konumu Avrupa seç (örneğin `eur3` ya da `europe-west1`), **production mode** ile başlat.
4. Firestore'un **Kurallar** (Rules) sekmesine bu depodaki [`firestore.rules`](firestore.rules) dosyasının içeriğini yapıştırıp **Yayınla**'ya bas.
5. **Proje ayarları** (dişli simgesi) → **Genel → Uygulamalarınız** bölümünde web simgesine (`</>`) basıp bir web uygulaması ekle; hosting gerekmez. Çıkan `firebaseConfig` içindeki **apiKey** ve **projectId** değerleri, `index.html` içindeki `FIREBASE` satırına yazılır. Bu değerler her web uygulamasında herkese açıktır, gizli değildir; verileri koruyan 4. adımdaki kurallardır.
6. İstersen Google Cloud Console'da **API'ler ve Hizmetler → Kimlik bilgileri** bölümünden bu anahtarı yalnızca `https://resat2148-arch.github.io/*` adresinden kullanılacak şekilde (HTTP referrer) kısıtlayabilirsin.

### 2 kişi (aynı telefon)

Telefonu yatay olarak ikinizin arasına koyun. Mavi oyuncu sol uçta, kırmızı oyuncu sağ uçta oturur; herkesin kalesi kendi tarafındadır.

- Her uçta o oyuncuya ait bir tuş sütunu vardır: ▲, ŞUT ve ▼. Tuşlar takım renginde, ŞUT yazısı da o oyuncuya dönüktür.
- Tuşlar ekranın kenarı boyunca dizildiği için, telefonu ister karşılıklı ister yan yana tutun, basılan ok çubuğun kaydığı yönü gösterir.
- İki oyuncu aynı anda basabilir; ekran birden fazla parmağı ayrı ayrı izler.
- İki taraf da "topa en yakın çubuk" kuralıyla oynar; her takımın aktif çubuğu kendi renginde parlar.
- Otomatik kaleci açıksa iki takıma birden uygulanır.

### Online (iki telefon)

Menüde **Online**'a dokun. Biri **Masa aç** der ve 4 karakterlik bir kod alır; diğeri **Masaya katıl**'a dokunup bu kodu girer. Bağlantı kurulunca maç kendiliğinden başlar.

- **Nerede çalışır:**
  - **Herkese açık adres (hesap gerekmez):** Telefonlar doğrudan (WebRTC) bağlanır. Eşleştirme için PeerJS'in ücretsiz genel sunucusu kullanılır. Mobil veride doğrudan bağlantı kurulamazsa, PeerJS'in aktarma (TURN) sunucuları devreye girer. PeerJS kütüphanesi oyunun yanında gelir (`peerjs.min.js`).
  - **claude.ai'deki oyun sayfası:** Sayfanın canlı "oda" bağlantısı kullanılır. Bunun için iki oyuncunun da claude.ai hesabı olmalı ve sayfa Paylaş menüsünden paylaşılmalı.
  - İki oyuncu aynı adresi açmalıdır: biri claude.ai sayfasını, öbürü herkese açık adresi açarsa birbirlerini bulamazlar.
- **Herkese açık adres (GitHub Pages):** Oyun `https://resat2148-arch.github.io/1/` adresinde yayında. İkiniz de bu adresi Safari'de açın; sonra biri **Online → Masa aç**, diğeri **Online → Masaya katıl** der. Bu dala gönderilen her değişiklik bir iki dakika içinde adrese yansır. Kurulum adımları:
  1. Depo herkese açık olmalı; GitHub Pages ücretsiz planda yalnızca açık depolarda çalışır (**Settings → General → Danger Zone → Change repository visibility → Public**).
  2. **Settings → Pages** sayfasında **Build and deployment → Source: Deploy from a branch** seç. Dal olarak `claude/telefonda-kicker-oyunu-ik7r65`, klasör olarak `/ (root)` seçip **Save**'e bas.
  3. İlk yayın, dala yeni bir değişiklik gönderilince başlar. Depodaki `.nojekyll` dosyası, GitHub'ın dosyaları işlemeden olduğu gibi sunmasını sağlar.
- **Nasıl işler:**
  - Masayı açan telefon (mavi) bütün fiziği yürütür ve saniyede 30 kez masanın durumunu gönderir. Paket yaklaşık 700 bayttır.
  - Katılan telefon (kırmızı) tuşlarını gönderir ve gelen durumu 90 milisaniye geriden, yumuşatarak çizer.
  - Kısa dokunuşlar kaybolmasın diye ŞUT, SÜPER ve DEV basışları sayaçla gönderilir.
- **Katılanın ekranı:** 180° döndürülür. Böylece iki oyuncu da kendi kalesini solda görür, tabela da buna göre "Sen / Rakip" diye aynalanır.
- **Maç kuralları:** Gol sayısı, aktif çubuk, otomatik kaleci, süper şut ve dev kaleci ayarları masayı açanın ayarlarıdır. Katılanın kendi ayarları maçtan sonra geri gelir.
- **Mola:** Online maç durdurulamaz; mola ekranı yalnızca ses, ifade ve spiker ayarları ile maçtan çıkış içindir.
- **Rövanş:** Maç bitince iki telefonda da sonuç kendi açından gösterilir. Rövanş isteğini her iki taraf gönderebilir.
- **Bağlantı kopması:** Bir taraftan 6 saniye haber gelmezse ya da oyuncu çıkarsa, diğer telefon "Rakibin bağlantısı koptu" diyerek menüye döner.
- **Sınırlar:**
  - Gecikme iki telefonun bağlantısına bağlıdır. Katılan taraf kendi çubuğunun hareketini gecikmeyle görür.
  - Masayı açan telefonun ekranı açık kalmalıdır; kilitlenirse ya da uygulamadan çıkılırsa oyun iki taraf için de durur.
  - Bağlantı kodu iki tarayıcı sekmesi arasında denendi: claude.ai odasının taklidiyle ve yerelde çalıştırılan bir PeerJS sunucusu üzerinden gerçek WebRTC ile. Herkese açık adresten, PeerJS'in genel sunucusu üzerinden iki iPhone ile de oynandı.

Klavyeyle 2 kişi oynamak için mavi `W S` ve `Boşluk` (ya da `F`), kırmızı `↑ ↓` ve `Enter` (ya da `L`) tuşlarını kullanır. Süper şut mavi için `E`, kırmızı için `O` ya da sağ `Shift`; dev kaleci mavi için `R`, kırmızı için `I` ya da sağ `Ctrl`. İfadeler mavi için `1`–`8`, kırmızı için sayısal tuş takımında `1`–`8`.

Bilgisayara karşı modda klavyeyle de oynanır: `↑ ↓` ya da `W S` aktif çubuğu kaydırır, `Boşluk` şut çeker, `E` ya da `Q` süper şutu hazırlar, `R` dev kaleciyi açar, `1`–`8` ifade gönderir. İki modda da `P` ya da `Esc` molaya alır.

Oyun yatay ekran için tasarlandı. Telefon dik tutulursa sahne kendiliğinden 90° döner; telefonu yan çevirmen yeterli.

## Telefonda açmak

- **GitHub Pages:** Depo ayarlarında *Settings → Pages* bölümünden bu dalı ve kök klasörü (`/`) seç. Verilen adresi telefonda aç.
- **Yerel ağ:** Bilgisayarda depo klasöründe `npx http-server -p 8080` çalıştır, telefondan aynı Wi-Fi üzerinden `http://<bilgisayarın-IP-adresi>:8080` adresini aç.
- Tarayıcı menüsünden **Ana ekrana ekle** dersen oyun, `manifest.webmanifest` sayesinde tam ekran ve yatay açılır.

## Top fiziği

Bütün hesaplar gerçek masa ölçüleriyle, milimetre ve saniye cinsinden yapılır: 120 × 68 cm saha, 35 mm top, 20,5 cm kale ağzı, 15 cm çubuk aralığı. Çubuk düzeni gerçek masadaki gibidir: kaleci (1), defans (2), forvet (3) ve orta saha (5).

- **Kayma → yuvarlanma:** Vurulan top önce masada kayar. Sürtünme, topun dönüşünü doğrusal hızına eşitleyene kadar onu yavaşlatır, sonra top yuvarlanır. Dolu küre modeli kullanılır; kayma, doğrusal hızın 3,5 katı hızla söner. Bu yüzden duvardan kafa kafaya dönen top, önceki dönüşü ona ters çalıştığı için belirgin şekilde yavaşlar.
- **Yuvarlanma direnci ve hava sürtünmesi:** Top yuvarlanırken sabit bir yavaşlama ile hızla orantılı küçük bir sürtünme etki eder.
- **Vuruş:** Çubuk dönüş ekseni etrafında döner. Ayağın topa değdiği noktadaki hız `v = L · ω · cos θ` ile hesaplanır. Çarpışma, çarpma katsayılı ve sürtünmeli bir impuls olarak çözülür; bu da çubuğun kayma hızının topa yan hız olarak geçmesini sağlar. Kavisli ayak topu biraz üstten yakaladığı için topa bir miktar üst dönüş de verir.
- **Kalkan adamlar:** Adamlar yaklaşık 56°'den fazla döndüğünde ayaklar topun üstünden geçer ve çarpışma olmaz. Kendi pasın arkadan gelip adamlarından birine çarpacaksa o çubuk kalkar ve top altından geçer. Gerçek oyuncular da bunu içgüdüsel olarak yapar. Adamlar topun üstüne inerse top tuzağa düşer.
- **Duvarlar ve direkler:** Ahşap duvarlar ve yuvarlak kale direkleri farklı çarpma katsayılarına sahiptir.
- **Eğimli kenarlar:** Kenar rampaları ile köşe eğimleri, duran topu tekrar adamların erişebileceği yere yuvarlar. Kalecinin önündeki köşe eğimleri, kalecinin ulaşamadığı yanlardaki topu onun önüne getirir.
- **Oluklar:** Çubuk aralığı 15 cm, ayak ise ileriye ancak yaklaşık 8 cm uzanır. Bu yüzden masada duran topa hiçbir adamın vuramadığı şeritler kalır: kaleciyle defans arası ve iki takımın sırt sırta kaldığı iki boşluk. Bu şeritlerde saha hafif eğik (yaklaşık 1,2°, eski ve hafif eğilmiş gerçek masalardaki gibi). Orada duran top, bir çubuk çizgisini geçmesi gerekmeden en yakın oynanabilir noktaya, bir çubuğun önüne ya da hemen arkasına, yarım saniye içinde yuvarlanır. Eğim yuvarlanma direncini yenecek kadar güçlü, ama hızlı topu fark edilir şekilde saptırmayacak kadar hafiftir.
- **Tam tur vuruş:** Çubuğun hemen arkasındaki top için adamlar öne doğru tam tur döner: ayaklar üstten geçer, topun arkasına iner ve topu ileri sürer (yaklaşık 1,2 m/s).
- **Ölü top:** Hiçbir adamın ulaşamayacağı yerde duran top, kurala uygun biçimde orta sahadaki servis deliğinden yeniden oyuna girer. Oluklar ve tam tur vuruşla bu nadiren gerekir: simülasyonda 10 dakikalık maçlarda ölü top servisi 21–28'den 3–11'e, topun ulaşılamaz yerde durduğu süre 90–110 saniyeden 4–14 saniyeye indi.
- **Adım aralığı:** Fizik saniyede 480 sabit adımla hesaplanır. Böylece en sert şut bile bir adımda adamın içinden geçip gitmez.

## Bilgisayar rakip

Üç seviye vardır: **Acemi**, **Kulüp** ve **Usta**. Seviyeler şu değerlerde ayrışır:

- tepki süresi (topu 0,09–0,28 saniye gecikmeyle "görür")
- el hızı
- nişan hatası
- topun gideceği yeri önceden tahmin etme
- şut gücü
- açılı şut deneme sıklığı

Rakip, aktif çubuğunu topun o çubuğun hizasından geçeceği noktaya getirir. Top ayağının önündeyken kaleye doğru nişan alıp vurur. Çubuğunun hemen arkasına düşen topu tam tur vuruşla ileri oynar.

## Dosyalar

- `index.html`: oyunun tamamı (HTML, CSS, JavaScript; sesler Web Audio ile üretilir)
- `manifest.webmanifest`, `icon.svg`: ana ekrana eklemek için
- `peerjs.min.js`: online oyun için PeerJS 1.5.5 (MIT lisansı, © Michelle Bu ve Eric Zhang)
- `.nojekyll`: GitHub Pages dosyaları olduğu gibi sunsun diye
- `firestore.rules`: dünya tablosu için Firestore güvenlik kuralları
