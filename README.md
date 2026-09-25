# Cep Langırtı

Telefonda oynanan langırt (kicker) oyunu. Tek bir `index.html` dosyasından oluşur; kurulum, kütüphane ya da derleme adımı yoktur.

## Nasıl oynanır

Üç mod var: **Bilgisayara karşı** (mavi takım sensin, kırmızıyı bilgisayar oynar), **2 kişi** (aynı telefonda arkadaşınla) ve **Online** (iki ayrı telefonda arkadaşınla). Seçtiğin gol sayısına (3, 5 ya da 7) ilk ulaşan maçı kazanır.

**Süre: 90 saniye.** Skorun altındaki sayaç geri sayar. Sayaç yalnızca top oyundayken işler; gol sonrası ve servis beklerken, bu telefonda mola verilince durur.
- Son 10 saniyede sayaç kırmızı yanar ve spiker uyarır; son 5 saniyede her saniye tıkırdar.
- Süre bittiğinde önde olan kazanır ("Süre doldu").
- Skor eşitse **altın gol** oynanır: ilk atan kazanır.
- Kural bütün modlarda geçerlidir: bilgisayara karşı, 2 kişi, 2v2, kupa, turnuva ve online. Online'da süreyi masayı açan tutar, diğer telefonlar aynı sayacı görür.

**Dil:** Oyun Türkçe, İngilizce ve Almanca oynanabilir (aşağıya bak).

| Kontrol | Ne yapar |
| --- | --- |
| **▲ / ▼** (sol başparmak) | Aktif çubuğu (pirinç renkte parlayan çubuk) yukarı / aşağı kaydırır. Parmağını kaldırmadan ▲ ile ▼ arasında kaydırabilirsin. |
| **ŞUT** (sağ başparmak), dokun | Aktif çubuğun adamları hızlıca döner ve topa vurur. Top ayağının önündeyse hemen vurur. Top sana doğru ya da arkadan gelirken biraz erken dokunursan (0,28 saniyeye kadar) vuruş topun gelmesini bekler. |
| **ŞUT**, basılı tut | Adamlar geriye yatar ve güç toplar (tuşun çevresindeki halka dolar). Bıraktığında daha sert vurur. Basılı tutarken hareket eden bir top ayağının önüne gelirse adamlar bırakmanı beklemeden, o ana kadar topladıkları güçle vurur. Duran ya da yavaş bir topta istediğin kadar güç toplayabilirsin. |
| Vururken ▲/▼ | Kayan çubuk sürtünmeyle topa yan hız verir, top çapraz gider. |
| Ayağın kenarıyla vurmak | Ayak yuvarlak olduğu için top açılı seker. |
| Arka | Top aktif çubuğun hemen arkasında (1–6 cm) kaldıysa ŞUT'a bas: adamlar öne doğru tam tur döner, ayak topun arkasına iner ve topu ileri sürer. Ayak topun üstüne inerse top sıkışıp ileri fırlar; ayağın yalnızca kenarı değerse yana kaçar. |
| Arkadan gelen pas | Kendi pasın arkadan gelirken adamlar ayaklarını geriye kaldırır, top altlarından geçer. O sırada ŞUT'a basarsan ayaklar topun arkasına iner ve topu tek vuruşta ileri gönderir. En iyisi top çubuğa varmadan basmaktır: hızlı bir pas çubuğu geçtikten sonra ayak ona yetişemez. |
| **SÜPER** (ŞUT'un üstünde) | Göstergen dolunca süper şutu hazırlar; bir sonraki vuruşun süper şut olur (aşağıya bak). |
| **DEV** (ŞUT'un altında) | Kendi göstergesi dolunca kalecin 6 saniyeliğine dev olur (aşağıya bak). |
| **💬** (sol üst) | Rakibine laf atmak için ifade menüsünü açar (aşağıya bak). |

### Dil (Türkçe · English · Deutsch)

Menüde oyunun adının altındaki **🌐 Türkçe · English · Deutsch** satırından dil seçilir.
- **Seçim:** Seçim kaydedilir ve sayfa o dilde yeniden açılır. Diğer ayarlar (seviye, gol sayısı, diziliş…) olduğu gibi kalır. Dil menüden değiştirilir, maç sırasında değil.
- **İlk açılış:** Oyun ilk açılışta telefonun dilini izler: Türkçe telefonda Türkçe, Almanca telefonda Almanca, diğerlerinde İngilizce açılır. Daha önce oynamış olan biri (ilerlemesi kayıtlı) Türkçe devam eder.
- **Ne çevrilir:** Menüler, bildirimler, görevler, rozetler, yetenekler, mağaza, takım editörü, kupa, turnuva, online ekranları, özel ligler ve sohbet ekranı, paylaşım kartı ve lig davetleri. Oyunun adı İngilizcede **Pocket Foosball**, Almancada **Taschenkicker** olur.
  - Sayılar, yüzdeler (%40 · 40% · 40 %) ve tarihler her dilin kendi yazımıyla gösterilir.
  - Bilgisayar takımlarının ve rastgele rakiplerin adları da dile uyar.
- **Spiker:** Seçilen dilde konuşur ve telefonun o dildeki sesini kullanır. Telefonda o dilin sesi yoksa yalnızca altyazı gösterir.
- **Online:** Her telefon kendi dilinde görür, farklı dillerdeki oyuncular birlikte oynayabilir. Sohbet mesajları yazıldığı dilde gider; hazır mesajlar yazanın dilindedir. Oyuncu ve lig adları gibi senin yazdıkların çevrilmez.
- **Geliştirici notu:** Metinler kodda Türkçe yazılır ve `__('...')` ile çevrilir; `{0}`, `{1}` gibi yerler değerlerle dolar. İngilizce ve Almanca karşılıkları `index.html` başındaki `I18N` sözlüğündedir. Çevirisi olmayan bir metin Türkçe görünür; yeni bir metin eklenirken iki dile de çeviri eklenmelidir.

### Aktif çubuk

İsteğe bağlı bir özelliktir ve açık gelir. Menüdeki **Aktif çubuk** anahtarından ya da moladaki **Aktif çubuk** düğmesinden kapatabilirsin; seçimin hatırlanır.

- **Açık:** Yalnızca topa en yakın çubuk kayar ve vurur (ayrıntılar aşağıda).
- **Kapalı:** Bütün çubukların birlikte kayar ve birlikte vurur. Her çubuk kendi yol aralığının aynı oranında kayar, böylece çubuklar birbirinden kopmaz. Maç ortasında kapatırsan çubuklar yumuşakça aynı hizaya gelir. Bu modda kaleci zaten elinle birlikte hareket ettiği için otomatik kaleci devre dışıdır.
- 2 kişilik modda ayar iki oyuncuya da uygulanır. Bilgisayar her zaman aktif çubukla oynar.

Açıkken her an yalnızca bir çubuğunu kontrol edersin: topa en yakın ve topu önüne alabilecek çubuğu. Top başka bir çubuğun bölgesine geçince kontrol de kendiliğinden o çubuğa geçer. Diğer çubukların, bıraktığın yerde kalır.

- Top adamlarının arkasındaysa arkadaki çubuk için ek mesafe sayılır. Bu yüzden kontrol, topu ileri vurabilecek çubukta kalır. Top arka vuruşla (tam tur) yetişilecek kadar yakınsa (6 cm) bu ek mesafe küçüktür; kontrol, topu önünde tutan ama ona yetişemeyen arkadaki çubuğa geçmez.
- Top hızla kendi kalene geliyorsa kontrol, topun henüz geçmediği ilk çubuğa verilir.
- Kendi pasın ya da şutun ileri giderken kontrol, topun varacağı sıradaki çubuğuna geçer. Böylece o çubuğu top gelmeden hizalayabilirsin.
- Kontrol yalnızca güç toplarken ve vuruşun topa değebildiği kısa anda kilitli kalır. Adamlar topun üstüne kalkar kalkmaz kontrol sıradaki çubuğa geçebilir; vuran çubuk kendi kendine dikey konuma döner.
- Yeni çubuk açıkça daha uygunsa kontrol hemen geçer. Top iki çubuğun tam ortasında duruyorsa, titremesin diye kısa bir süre (0,06 sn) beklenir.
- Top yavaşlarken kontrolün iki çubuk arasında gidip gelmemesi için hız eşiklerinin açılma ve kapanma değerleri farklıdır: ileri pas 700 mm/s'de başlar, 350 mm/s'de biter.
- Bilgisayar da aynı kuralla oynar: o da aynı anda tek çubuğunu yönetir.

### Ölü top

- **Eğimler:** Masanın kenarları ve köşeleri hafif eğimlidir; duran top oynanabilecek bir yere yuvarlanır. Kalecinin önündeki köşe eğimleri kalecinin ayağının yetişemediği bölgeyi de kapsar, bu yüzden oradaki top kalecinin önüne döner.
- **Yeniden servis:** Top durur ve kimse oynamazsa "Ölü top" denir ve servis yeniden atılır. Bekleme süresi topun yerine göre değişir: hiçbir ayağın yetişemediği yerde 2,2 saniye, yalnızca geriye yatan bir ayağın yetişebildiği yerde (bir çubuğun 6–8 cm arkası) 4 saniye, bir ayağın vurabildiği yerde 12 saniye.
- **Bilgisayar:** Arkasında kalan topu arka vuruşla oynar. Çubuğu sonuna dayandığı için ayağını topla tam hizalayamasa da top ayağının kenarındaysa vurur. Simülasyonda bilgisayar–bilgisayar maçlarında ölü top dakikada 0,6–1,2'den (seviyeye göre) sıfıra indi.

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

### Diziliş (taktik)

Gerçek langırt masası 1-2-5-3 dizilir: kaleci, 2'li defans, 5'li orta saha, 3'lü forvet. Burada takımını başka dizilişle de sahaya çıkarabilirsin. Kaleci her dizilişte tektir; değişen, defans, orta saha ve forvet çubuklarındaki adam sayısıdır.

| Diziliş | Adı | Ne işe yarar |
| --- | --- | --- |
| **2-5-3** | Klasik | Gerçek langırt masası: ikili defans, beşli orta saha, üçlü forvet. |
| **4-4-2** | Dengeli | Dörtlü defans, dörtlü orta saha, iki forvet. |
| **4-3-3** | Hücum | Dörtlü defansın önünde üç forvet. |
| **3-4-3** | Atak | Üçlü defans, dörtlü orta saha, üç forvet. |
| **3-5-2** | Orta saha | Kalabalık orta saha, iki forvet. |
| **5-3-2** | Kale önü | Beşli defans duvarı, iki forvet. |
| **4-5-1** | Kontra | Kalabalık orta saha, bütün hattı gezen tek forvet. |

- **Seçmek:** Menüde gol sayısının yanındaki **diziliş** düğmesi seçim ekranını açar. Her dizilişin yanında takımının küçük bir masa çizimi görünür. Seçimin hatırlanır.
- **Maç ortasında:** Moladaki **Diziliş** düğmesiyle taktiği değiştirebilirsin. Yeni diziliş hemen sahaya çıkar.
- **Adam sayısı ile kayma:** Çubukta adam arttıkça adamlar sıklaşır ve çubuk daha az kayar. Adam azaldıkça aralık açılır ve çubuk daha çok yol gider. Adamlar arası aralık ve kayma yolu şöyledir:
  - 5 adam: 12 cm aralık, ±7,6 cm kayma
  - 4 adam: 15,3 cm aralık, ±8,7 cm
  - 3 adam: 20,5 cm aralık, ±11,1 cm
  - 2 adam: 24 cm aralık, ±19,6 cm
  - Tek forvet: bütün masayı gezer.
- **Bilgisayar rakip:** Her maça rastgele bir dizilişle çıkar. Maç başındaki yazıda rakibin dizilişi görünür (ör. "rakip 4-3-3").
- **2 kişi:** İki takım da seçili dizilişle oynar.
- **2v2:** Roller aynı kalır. Savunmacı kaleciyle defans çubuğunu, hücumcu orta sahayla forvet çubuğunu yönetir; kaç adam olursa olsun.
- **Online:** Her oyuncu kendi dizilişiyle çıkar ve iki telefon da iki takımın dizilişini görür. Maç ortasında moladan yapılan değişiklik rakibin ekranına da yansır. 2v2 masada ve turnuvada takımın dizilişini o takımın ilk oyuncusu seçer. Rakip bulunamayınca gelen rakip de kendi dizilişiyle oynar.

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
- **Özet:** Rozet, kupa, mağazadan alınan eşya ve en iyi günlük seri.
- **İstatistikler:**
  - Maç ve toplam oynama süresi; galibiyet ve kazanma yüzdesi; mağlubiyet.
  - Atılan ve yenilen gol, maç başı ortalamalarıyla.
  - Süper gol, kurtarış, gol yemeden galibiyet, geri dönüş, en uzun gol serisi, en farklı galibiyet ve kupa şampiyonlukları.
- **Rakibe göre:** Acemi, Kulüp, Usta ve online için galibiyet–mağlubiyet, yeşil bir kazanma çubuğuyla.
- **Son maçlar:** Son 10 maç, "G 3–1" ya da "M 0–3" olarak; bilgisayar seviyesi, online ya da kupa işaretiyle.
- **Ne sayılır:** Görevlerdeki gibi bilgisayara karşı ve online maçlar, maç bitince, kendi tarafından sayılır; 2 kişilik maçlar sayılmaz.
  - Profilden önce tutulmayan sayılar profil geldikten sonra başlar: yenilen gol, oynama süresi, rakibe göre kayıt, en farklı galibiyet ve son maçlar.
  - Yenilen gol ortalaması yalnızca bu maçlar üzerinden hesaplanır.

### Yetenek ağacı

Görevler ekranının **Yetenek** sekmesi. Seviye 1'in üstündeki her seviye 1 yetenek puanı verir. Harcanmamış puan varsa menüdeki profil rozetinde "+1" yazar ve rozete dokununca doğrudan bu sekme açılır. Seviye atlanınca maç sonu çipi de puanı haber verir ("⬆️ Seviye 5: Yetenekli! +1 yetenek puanı").

Üç dal, her dalda dört düğüm var. Bir düğümü açmak için aynı dalda bir öncekine en az 1 puan vermiş olmak gerekir. Düğüme dokununca ne yaptığı ve sonraki kademesi görünür; **Geliştir** ile 1 puan harcanır.

| Dal | Düğüm | Kademe | Etki (kademe başına) |
|---|---|---|---|
| 🔥 Hücum | Sert Şut | 3 | şut gücü +%4 |
| | Hızlı Kurma | 2 | güç toplama %10 daha kısa |
| | Süper Şarj | 2 | süper şut göstergesi %15 daha hızlı dolar |
| | Seri Katili | 2 | gol atınca süper şut göstergesi +%8 |
| 🛡️ Savunma | Çevik Bilek | 3 | çubuk hızı +%5 |
| | Refleks | 2 | otomatik kaleci %15 daha çabuk görür, %10 daha hızlı kayar |
| | Dev Şarj | 2 | dev kaleci göstergesi %15 daha hızlı dolar |
| | Uzun Dev | 2 | dev kaleci 1 saniye daha uzun sürer |
| 🧠 Taktik | Tam Tur Ustası | 2 | tam tur vuruşu %15 daha güçlü |
| | Hazır Başla | 1 | maça süper şut göstergesi %25 dolu başlarsın |
| | Soğukkanlı | 1 | 2 gol gerideyken göstergeler %30 daha hızlı dolar |
| | Son Kale | 1 | rakip maç topuna gelince dev kaleci göstergen bir kez anında dolar |

- **Toplam:** Ağacın tamamı 23 puan; hepsi seviye 24'te açılır. Bu yüzden erken seviyelerde hangi dala yatırım yapacağını seçmek gerekir.
- **Geri alma:** "Puanları geri al" bütün puanları ücretsiz geri verir; başka bir dal denenebilir.
- **Nerede geçer:** Yalnızca bilgisayara karşı maçlarda ve haftalık kupada, yalnızca senin takımında. Online ve 2 kişilik maçlarda iki taraf da eşittir; yetenekler kapalıdır.
- **Denge:** Etkiler küçük tutuldu (en fazla +%12 şut, +%15 çubuk hızı). Oyunu yine el becerisi kazandırır; yetenekler zor bilgisayar seviyelerinde küçük bir avantaj sağlar.
- Süper şut ya da dev kaleci ayarda kapalıysa ilgili düğümler etkisizdir.

### Günlük görevler ve rozetler

Ana menüdeki **🎯 0/3 · ⭐ 0** düğmesi görevler, rozetler, kupa ve tablo ekranını açar (yanındaki **🏆** doğrudan kupaya, **🛒** mağazaya gider); sağ üstte kaç yıldızın olduğu yazar. Maç sonu ekranında da o maçta tamamlanan görevler ve kazanılan rozetler görünür; onlara dokununca aynı ekran açılır.

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
  | 🎨 Koleksiyoncu | Mağazadan 1 / 5 / 15 eşya al |

- **Ne sayılır:**
  - Bilgisayara karşı ve online maçlar, maç bitince kendi tarafından sayılır; online'da iki telefon da kendi ilerlemesini tutar. Yarıda bırakılan maç sayılmaz.
  - 2 kişilik maçlar sayılmaz; tek başına iki tarafı oynayıp görev toplamak çok kolay olurdu.
  - Kendi kalesine atılan gol, golü kazanan tarafa "gol" olarak yazılmaz.
  - Kurtarış: kaleye 1,8 m/s'den hızlı gelen bir şutu kalecinin durdurması. Bilgisayarlar arası denemelerde bir maçta genelde 0–3 kurtarış oluyor; görev hedefleri buna göre seçildi.
  - İfade ve paylaşım görevleri anında ilerler. Paylaşım, paylaşım menüsünden bir uygulamaya gönderince ya da **İndir**'e basınca sayılır; her maçın kartı bir kez sayılır.
- **Saklama:** İlerleme o tarayıcıda saklanır (`localStorage`). Safari'de açılan oyun ile ana ekrana eklenen oyunun depoları ayrıdır; hep aynı yerden oyna. Tarayıcı verileri silinirse ilerleme de silinir.

### Takım ve forma editörü

Ana menüdeki arma düğmesi (ilk açılışta **🛡️**) mağaza ekranının **Takımım** bölümünü açar. Burada kendi takımın kurulur ve değişiklikler anında kaydedilir:

- **Takım adı** (en çok 14 harf) ve **kısaltma** (3 harf). Kısaltma kendin yazmadıkça addan çıkar: "Sarı Kartallar" → SAR.
- **Ana renk:** Formanın rengi. 14 renk var: mavi, lacivert, gök mavisi, turkuaz, fıstık yeşili, sarı, turuncu, kırmızı, bordo, mor, pembe, siyah, beyaz, altın.
- **İkinci renk:** Adamların kafaları ve desen. Çubuklu formada çizgiler, Yıldızlı formada yıldız bu renkte olur.
- **Figür tasarımları:** Bazı formalar adamların kendisini değiştirir. Hepsi takımın renginde kalır, böylece iki taraf maçta karışmaz.
  - **Retro:** İnce çizgili eski usul forma, krem yaka ve omuzlar.
  - **Piksel:** 8-bit oyunlardaki gibi kare piksellerden adamlar; kafada iki piksel göz rakip kaleye bakar.
  - **Robot:** Teneke kare kafa, rakip kaleye bakan parlayan LED gözler, antenin ucu ve göğüs paneli takım renginde, köşelerde cıvatalar.
  - **Şövalye:** Çelik miğfer (vizör yarığı öne bakar), takım renginde sorguç; zırhın üstünde takım renginde arma ve ikinci renkte haç.
- **Desen:** Mağazadan aldığın formalar. Kilitli bir desene dokununca mağazada o forma açılır.
- **Arma:** 16 simgeden biri. Ana ve ikinci renkle bir kalkanın içinde görünür.
- Sağdaki önizlemede armanı ve formanı giymiş adamları görürsün. **Varsayılan takıma dön** her şeyi klasik maviye çevirir.

Takımın nerede görünür:
- Menüdeki düğme armanı, takımının renklerinde gösterir.
- Maçta adamlar takımının renklerini giyer. Skor tablosunda armanla kısaltman yazar (🦅 SKR), skor ve boncuklar da takımının renginde olur.
- Maç sonu ekranında ve paylaşım kartında da takımının adı ve rengi yer alır.
- Bilgisayara karşı ve kupada takımınla oynarsın. Online'da telefonlar takımlarını birbirine gönderir, iki taraf da kendi takımıyla çıkar. 2 kişilik maç mavi–kırmızı kalır.

**Renk çakışması:** İki takımın formaları birbirine çok benzerse kırmızı taraf (bilgisayar ya da online misafir) deplasman renkleriyle oynar.
- İkinci rengi yeterince farklıysa renklerini değiştirir: ikinci rengi formaya, ana rengi detaylara geçer.
- Değilse kırmızı, mavi, beyaz, siyah ve sarı arasından diğer takıma en uzak olanı giyer.
- İki telefon aynı hesabı yaptığı için iki ekran da aynı renkleri gösterir. Editör, rengin bilgisayarınkiyle çakışıyorsa bunu yazar.

### Mağaza

Görevlerden ve kupadan kazanılan yıldızlar mağazada harcanır. Mağaza, ana menüdeki **🛒** düğmesiyle açılır. Günün yeni fırsatları henüz görülmediyse düğmede turuncu bir nokta yanar.

Ekranın üç bölümü var:
- **Solda bölümler:** Fırsatlar, Top, Masa, Forma, Gol şovu ve Avatar.
- **Ortada eşyalar:** Her birinin küçük bir resmi ve fiyatı vardır. Sende olanlarda "Sende", kullandığında "Kullanılıyor" yazar.
- **Sağda önizleme:** Seçtiğin eşya kullanılırken görünür. Top masada yuvarlanır, forma çubuktaki adamlarda sallanır, gol şovu kalede patlar, avatar profil rozetinde görünür. Altında açıklaması, düğmesi ve bir not vardır.

Satın almak için eşyaya dokunup **Satın al · 12⭐** düğmesine basmak yeter. Aldığın eşya hemen kullanılır. Sende olan bir eşyaya **Kullan** ile ücretsiz geri dönersin. Yıldızın yetmiyorsa düğmede kaç yıldız eksik olduğu yazar. Sağ üstteki **⭐ +** cüzdanı, yıldız kazanılan günlük görevlere götürür.

| Bölüm | Eşyalar (⭐) | Kim görür |
| --- | --- | --- |
| ⚽ Top | Klasik (ücretsiz), Turuncu 5, Futbol 12, Neon 20, Altın 35, Ateş topu 60 | Yalnızca sen; online'da her telefon kendi topunu görür |
| 🟩 Masa | Klasik (ücretsiz), Gece 8, Çim 15, Bordo 30, Buz 50, Altın Salon 90 | Yalnızca sen |
| 👕 Forma | Klasik (ücretsiz), Çubuklu 6, Yıldızlı 12, Retro 16, Gece 20, Piksel 28, Neon 32, Robot 40, Şampiyon 50, Şövalye 60 | Sen ve online rakibin |
| 🎆 Gol şovu | Konfeti (ücretsiz), Yıldız yağmuru 8, Kalpler 14, Havai fişek 24, Alev 36, Şimşek 55 | Sen ve online rakibin |
| 😎 Avatar | 🦄 4, 🥷 6, 🧙 6, 👽 8, 🦖 8, 🐙 10, 👾 10, 🦸 12 | Profil ve menü |

- **Forma:** Takımının adamları giyer. Desen formadan gelir, renk takımınkidir. Böylece mavi hep mavi, kırmızı hep kırmızı kalır ve iki taraf hiç karışmaz.
  - Bilgisayara karşı sen formanı giyersin, bilgisayar klasik formayla oynar.
  - Online'da iki telefon birbirine formasını ve gol şovunu gönderir, iki taraf da kendi seçtiğiyle oynar.
  - 2 kişilik maçta iki taraf da klasik formayla oynar.
  - Formanı menünün arkasındaki masada ve paylaşım kartında da görürsün.
- **Gol şovu:** Senin attığın gollerde kalede oynar. Hareketi azaltma ayarı açık telefonlarda gol şovu gösterilmez; önizleme de hareketsiz bir kare olur.
- **Avatar:** Ücretsiz 16 avatar profilde durur. Mağazadan alınanlar da oraya eklenir. Profildeki seçicinin sonundaki **🛒** mağazanın Avatar bölümünü açar.
- **Günün fırsatları:** Her gün, henüz sende olmayan eşyalardan üçü indirime girer: biri %40, ikisi %25. Fırsatlar gece yarısı yenilenir; ne kadar kaldığı yazar.
- **Paketler:** Bir takım eşyayı tek tek almaktan %25 ucuza verir.
  - 🎁 Başlangıç: Turuncu top, Çubuklu forma, Yıldız yağmuru, 🦄 (23⭐ yerine 17⭐).
  - 🌙 Gece: Gece masası, Neon top, Gece forması (48⭐ yerine 36⭐).
  - 🔥 Ateş: Ateş topu, Alev, Bordo masa (126⭐ yerine 95⭐).
  - 👑 Şampiyon: Altın Salon, Altın top, Şampiyon forma, Havai fişek (199⭐ yerine 149⭐).
  - Paketteki eşyalardan bazıları zaten sendeyse onlar fiyattan düşülür. Paketi alınca hepsi birden kullanılır.
- **Oyuna etkisi:** Yoktur; yalnızca görünüş değişir.
- **Ekonomi:** Bir günde görevlerden en çok 8⭐ kazanılır (1 + 2 + 3 + 2 bonus). Haftanın ilk kupa şampiyonluğu da 5⭐ verir. Maç sonunda bir şey almaya yetecek yıldızın olunca "🛒 Mağazada alabileceğin var" yazar ve dokununca mağaza açılır.
- **Saklama:** Aldıkların, kullandıkların ve günün fırsatları bu tarayıcıda saklanır. Eskiden açılan top ve masa temaları aynen kalır.

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
4. Firestore'un **Kurallar** (Rules) sekmesine bu depodaki [`firestore.rules`](firestore.rules) dosyasının içeriğini yapıştırıp **Yayınla**'ya bas. Kurallar değişince (örneğin özel ligler eklenince) bu adım yeniden yapılır; yapılmazsa ligler bulutsuz, telefondan telefona çalışmaya devam eder.
5. **Proje ayarları** (dişli simgesi) → **Genel → Uygulamalarınız** bölümünde web simgesine (`</>`) basıp bir web uygulaması ekle; hosting gerekmez. Çıkan `firebaseConfig` içindeki **apiKey** ve **projectId** değerleri, `index.html` içindeki `FIREBASE` satırına yazılır. Bu değerler her web uygulamasında herkese açıktır, gizli değildir; verileri koruyan 4. adımdaki kurallardır.
6. İstersen Google Cloud Console'da **API'ler ve Hizmetler → Kimlik bilgileri** bölümünden bu anahtarı yalnızca `https://resat2148-arch.github.io/*` adresinden kullanılacak şekilde (HTTP referrer) kısıtlayabilirsin.

### Turnuva (eleme ağacı)

Menüdeki **Turnuva** düğmesi, arkadaşlarla tek telefonda oynanan bir eleme turnuvası kurar.
- **Kurulum:**
  - **4** ya da **8** takım seçilir.
  - Oyuncuların adları yazılır: sen ⭐ ile başta durursun, **+ Oyuncu ekle** ile diğerleri eklenir.
  - Kalan yerleri adlı bilgisayar takımları doldurur (⚡ Kara Şimşekler, 🐺 Gece Kurtları, 🦈 Köpek Balıkları…). Bu takımların seviyesi seçilebilir: karışık, Acemi, Kulüp ya da Usta.
  - Gol hedefi menüdeki ayardır.
  - **Kura çek ve başla** eşleşmeleri rastgele çeker.
- **Ağaç:**
  - 8 takımda çeyrek final, yarı final ve final; 4 takımda yarı final ve final sütunları vardır, en sağda şampiyon kutusu durur.
  - Her maç kutusunda iki takım ve skor yazar. Kazanan parlak, elenen soluk görünür; oyuncuların adları sarıdır. Sıradaki maçın çerçevesi yanar.
- **Maçlar:**
  - **Oyuncu – bilgisayar:** Oyuncu mavide, bilgisayar takımın seviyesinde oynar.
  - **Oyuncu – oyuncu:** Bu telefonda 2 kişilik oynanır.
  - **Bilgisayar – bilgisayar:** **Bilgisayar maçlarını oynat** ile sonuçlar birer birer gelir. Güçlü takım daha sık kazanır.
- **Maçta:** Skor tablosunda, spikerde ve paylaşım kartında takımların adları geçer ("Turnuva · Yarı final"). Maç sonunda "🏟️ Ali finalde" yazar; **▶ Turnuva ağacı** ağaca döndürür.
- **Final:** Final bitince spiker şampiyonu ilan eder ve ağaçta 🏆 şampiyonun adıyla parlar.
- **Kayıt:** Turnuva ilerlemeyle birlikte saklanır. Menüye dönülüp başka gün devam edilebilir: Turnuva düğmesi ağacı açar. Yarıda bırakılan maç yeniden oynanır. Süren bir turnuvada **Yeni turnuva** bir kez onay ister.
- **İlerleme:** Görevlere, profile, yeteneklere ve forma/takım görünümüne yalnızca senin bilgisayara karşı maçların sayılır. İki kişilik maçlar ve başka oyuncuların bilgisayara karşı maçları sayılmaz. Haftalık kupa ayrıdır.

### Özel lig (arkadaşlar, iş yeri)

Menünün üstündeki **👥** düğmesi (ya da turnuva kurulumundaki **👥 Özel lig**) arkadaş grubuna ya da iş yerine özel, uzun soluklu bir lig ya da kupa kurar. Turnuvadan farkı şu: herkes kendi telefonundan katılır ve maçlar günlere yayılır.

- **Kurmak:** **+ Yeni lig kur** ile bir ad verilir ve biçim seçilir.
  - **Lig:** Herkes herkesle oynar. Tek devrede her ikili bir kez, çift devrede iki kez karşılaşır. En fazla 12 kişi.
  - **Kupa (eleme):** En fazla 8 kişi. Herkes katılınca kurayı kurucu çeker. Kaybeden elenir; sayı tutmazsa bazı oyunculara ilk turda bay geçer.
  - Maçların kaç gole kadar oynanacağı (3, 5 ya da 7) lig için bir kez seçilir. Her maç yine 90 saniyedir.
- **Davet:** Her ligin 6 harflik bir kodu vardır (ör. `K7M2PX`). **📨 Davet et** ligin bağlantısını ve uzun davet kodunu WhatsApp, e-posta gibi uygulamalarla paylaşır; paylaşma yoksa panoya kopyalar.
  - Bağlantıyı açan ya da uzun kodu **Katıl** kutusuna yapıştıran lige girer. Bu her zaman çalışır.
  - 6 harflik kod tek başına, oyun buluta (Firebase) bağlanabildiğinde yeter.
  - Bir telefon en fazla 8 ligde olabilir.
- **Tablo:** O (oynanan), G, M, AV (averaj) ve P (puan). Galibiyet 3 puandır; eşitlikte averaja, sonra atılan gole bakılır. Kupada tablo yerine eleme ağacı görünür.
- **Maçlar:** **Maçlar** sekmesinde önce senin kalan maçların, sonra diğerleri ve sonuçlar durur. Bir lig maçı iki şekilde oynanır:
  - **🌐 Online:** Rakibinle aynı anda biriniz **Masa aç** der, diğeri **Koda katıl** ile masanın kodunu girer. Maç kendiliğinden lig maçı olur: aranızdaki sıradaki maç sayılır, gol hedefi ligin ayarıdır. İki telefon da maç başında "🏅 lig maçı" yazar ve sonucu kaydeder. Aranızda oynanacak maç kalmadıysa maç dostluk maçı sayılır. Çift devrede rövanş ikinci devre olur.
  - **📱 Bu telefonda:** İki üye aynı telefonda 2 kişilik oynar; skor tablosunda ikisinin adı yazar. Bunu her maç için, başka iki üyenin maçı için de yapabilirsin; ofiste tek telefonla oynayanlar için. Maç sonunda **▶ Lig** lige döner.
- **Sonuç ekranı:** Lig maçından sonra ligin adı ve senin sıran yazar (ör. "🏅 Ofis Ligi · Ayşe kazandı · sıran: 2.").
- **Sohbet:** Her ligin bir **Sohbet** sekmesi var. Üyeler maç saatini ayarlar, birbirine laf atar.
  - Mesajlar en fazla 200 karakterdir. Hazır mesajlar tek dokunuşla gider: "Maça var mısın? ⚽", "Masa açtım, gel! 🌐", "Rövanş? 🔥", "Tebrikler 👏"…
  - Sohbette maç sonuçları ("⚽ Ayşe 3–1 Burak") ve lige katılanlar da kısa satırlar olarak akar.
  - Yeni mesaj gelince menüde bir bildirim çıkar ("💬 Ofis Ligi · Ayşe: Maça var mısın?"). 👥 düğmesinde turuncu bir nokta, lig listesinde "💬 2 yeni mesaj", sekmede okunmamış sayısı görünür. Maç oynarken bildirim gelmez.
  - Bir mesaja dokununca **Sil** çıkar. Herkes kendi mesajını, kurucu herkesinkini silebilir; yerinde "bir mesajı sildi" yazar.
  - Her ligin son 200 mesajı saklanır.
- **Sezon:** Ligde bütün maçlar oynanınca lider öne çıkar. Kurucu **Üyeler → Sezonu bitir** deyince lider şampiyon ilan edilir, tablo sıfırlanır ve yeni sezon başlar. Kupada finali kazanan şampiyondur; yeni sezonda kura yeniden çekilir. Eski şampiyonlar tablonun altında listelenir.
- **Kurucunun yetkileri:** Yanlış girilmiş bir sonucu silebilir (maç yeniden oynanır), bir üyeyi ligden çıkarabilir, kupada kurayı çeker ve sezonu bitirir. Silme ve çıkarma bir kez onay ister.
- **Ayrılmak:** **Ligden çık** ligi bu telefondan kaldırır. Oynadığın maçlar tabloda kalır, oynanmamış maçların düşer. Kupada ayrılan oyuncunun rakibi hükmen tur atlar.
- **Telefonlar nasıl eşitlenir:**
  - Her üyenin telefonu ligin tamamını saklar. İnternet olmasa da sonuçlar kaybolmaz.
  - **Bulut:** Oyun Firebase'e ulaşabildiğinde (GitHub Pages adresi) kurucunun ayarları, üyeler ve sonuçlar buluta yazılır. Lig ekranı açıkken her 30 saniyede bir güncellenir; sonuçlar herkese birkaç saniyede ulaşır.
  - **Telefondan telefona:** İki üye online oynadığında (lig maçı olsun olmasın) telefonlar ortak liglerini karşılaştırır. Eksik üyeleri ve sonuçları birbirine aktarırlar, her kayıt için daha yeni olan kalır. Bulutun olmadığı claude.ai sayfasında ligler bu yolla yayılır: kim kiminle oynarsa, bildiği sonuçlar ona geçer.
  - **Canlı (claude.ai):** Sayfası aynı anda açık olan üyeler birbirinin yeni mesajlarını, sonuçlarını ve yeni üyelerini bulut olmadan da anında görür. Her telefon liglerinin en yeni birkaç kaydını claude.ai odasındaki durumuna koyar; bunlar ligin kodundan türetilen bir anahtarla şifrelidir, yani sayfayı açık olan ama ligde olmayan biri okuyamaz. Online maç sırasında bu durdurulur, maç bitince sürer. Başka bir üyeden duyulan haber de böylece yayılır.
  - **Sohbet bulutta:** Lig sohbeti açıkken yeni mesajlar 6 saniyede bir, menüdeyken dakikada bir sorulur. Sunucunun saatine göre yalnızca yeni mesajlar istenir; yeni mesaj yoksa bu tek bir okuma sayılır.
  - Bir telefon diğer üyelerin hepsinden haber almamış olabilir. Bu yüzden ligde şampiyonu tablo değil, kurucunun sezonu bitirmesi belirler.
  - Başka telefonlara liglerin kendisi değil, yalnızca karıştırılmış kimlikleri gider. Bir lig, yalnızca iki telefon da o ligin üyesiyse aktarılır.
- **Güvenlik** ([`firestore.rules`](firestore.rules)):
  - Bir lig yalnızca kodunu bilen tarafından okunabilir; ligler listelenemez.
  - Ayarları yalnızca kurucu değiştirir. Herkes yalnızca kendi üyeliğini yazar; kurucu bir üyeyi çıkarabilir.
  - Sonuçları üyeler yazar. Yazılmış bir sonucu yalnızca kurucu değiştirebilir ya da silebilir.
  - Sohbeti yalnızca üyeler okur. Mesaj yazanın kendi üyeliğiyle yazılır; başkası adına yazılamaz. Yazılmış bir mesaj değiştirilemez; yalnızca yazarı ya da kurucu silebilir.
  - Adlar ve sayılar sınırlıdır (ad en fazla 24 karakter, skor 0–30).
  - Arkadaş ligi olduğu için değiştirilmiş bir oyunla sahte sonuç girmek yine de mümkündür. Kurucu yanlış sonucu silebilir.

### 2v2 (rol paylaşımı)

Gerçek turnuvalardaki kural: her takımda iki oyuncu vardır ve takımın dört çubuğu ikiye bölünür.
1. **Savunma:** Kaleci ve 2'li defans çubuğu.
2. **Hücum:** 5'li orta saha ve 3'lü forvet çubuğu.

Menüdeki **2v2** düğmesi seçim ekranını açar. Her seçeneğin yanında senin çubuklarının parladığı küçük bir masa görünür. Rakip takımda iki bilgisayar oyuncusu vardır; seviyeleri menüde seçili seviyedir.
- **🛡️ Savunma:** Kaleci ve 2'li defans senin, orta saha ile forveti bilgisayar takım arkadaşın oynar.
- **⚔️ Hücum:** 5'li orta saha ve 3'lü forvet senin, kaleyi ve defansı bilgisayar takım arkadaşın korur.
- **👥 İki kişi:** Tek telefonda iki kişi aynı takımda. Soldaki tuşlar savunmayı (sarı), sağdakiler hücumu (turkuaz) yönetir. Klavyede savunma W S Boşluk R, hücum ↑ ↓ Enter O.

Kurallar:
- Her oyuncu yalnızca kendi iki çubuğunu yönetir. Aktif çubuk açıkken iki çubuğundan topa en uygun olanı parlar. Kapalıyken iki çubuğu birlikte kayar.
- Senin çubuklarının tamponları maç boyunca hafifçe renkli kalır.
- Otomatik kaleci savunma oyuncusunun kalecisini izler.
- **Dev kaleci** savunmacının, **süper şut** hücumcunun düğmesidir. İki kişilik oyunda DEV soldaki, SÜPER sağdaki sütunda durur. Göstergeler takımındır.
- Bilgisayar takımlarında da iki ayrı oyuncu vardır. Savunmacı kendi çubuklarını, hücumcu kendi çubuklarını hazırlar; bu yüzden iki çubuk aynı anda hareket edebilir.
- 2v2 maçları bilgisayara karşı maç sayılır: görevler, rozetler, profil ve yetenekler geçerlidir. Rövanş aynı rollerle oynanır; menüdeki "Bilgisayara karşı" yeniden bire bir başlatır. Kupa hep bire birdir.

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

#### Rakip bul (rastgele eşleşme)

Online ekranındaki **Rakip bul**, kod paylaşmadan rastgele biriyle eşleştirir. Arama sırasında dönen bir halka ve geçen süre görünür; **Geri** aramayı bırakır.
- **Nasıl eşleşir:** Arayan telefon kendine özel kodla bir masa açar ve o sırada arayan başka birini bekler.
  - claude.ai odasında (ve aynı tarayıcının sekmeleri arasında) arayanlar birbirini görür; sonra gelen, önce gelenin masasına oturur.
  - PeerJS'te ilk arayan ortak bir "lobi" kimliğini tutar ve masasının kodunu sonraki arayana verir.
  - Eşleşince normal 1v1 online maç başlar; önce aramaya başlayan masayı açan olur.
- **Kimse yoksa:** 7–13 saniye içinde gerçek bir rakip bulunamazsa "Rakip bulundu: …" diye bir yedek rakip gelir. Oyuncuya o da gerçek bir online rakip gibi görünür:
  - bir oyuncu adı, bazen kendi forması, gol şovu ya da takımı
  - "Sen – Rakip" skor tablosu, "Maç bitti · Online", spikerde adı, ifadeler ve maç sonu ifade şeridi
  - Rövanşı çoğu zaman kabul eder; arada bir maçtan sonra "Rakibin bağlantısı koptu" diye ayrılır.
  - Gücü, oyuncunun online galibiyet oranına göre Acemi ile Usta arasında ayarlanır; ifadeleri bilgisayar rakibinkinden biraz seyrektir.
  - İnternet yoksa yedek rakip de gelmez; "bağlantı kurulamadı" hatası görünür.
- **Sayılma:** Yedek rakiple oynanan maç, profil, görevler, rozetler ve haftalık "Online lig" için normal bir online maç sayılır.
- **Bilinen fark:** Yedek rakip "Arkadaşlar" tablosuna satır göndermez; gerçek bir rakibin satırı maçtan sonra orada belirir.
- **Ayar:** Bekleme süresi kodda `MM.wait`'tedir.

#### Online 2v2 (dört telefon)

Online ekranındaki **2v2 masa aç** dört koltuklu bir masa açar: Mavi savunma, Mavi hücum, Kırmızı savunma, Kırmızı hücum. Diğerleri aynı **Masaya katıl** ile masa koduyla girer.
- **Koltuklar:** Masayı açan mavi savunmada oturur; mavi hücuma geçebilir. Gelenler önce karşı takıma, sonra boş yerlere oturur, yani iki telefon birbirine karşı oynar. Herkes boş bir koltuğa dokunarak yer değiştirebilir. Koltuklarda oyuncuların adları görünür.
- **Başlatma:** Masada en az iki kişi olunca masayı açan **Maçı başlat**'a basar. Boş koltuklarda bilgisayar oynar (masayı açanın seçtiği seviyede); gol hedefi de onun ayarıdır. Böylece 2v2 iki, üç ya da dört telefonla oynanabilir.
- **Maçta:** Herkes yalnızca kendi iki çubuğunu yönetir. Dev kaleci savunmacının, süper şut hücumcunun düğmesidir.
  - Kırmızı takımdakilerin ekranı ters döner; herkes kendi kalesini solda görür.
  - Skor tablosunda kendi takımın "Siz" diye yazar. Spiker iki takımın oyuncularını adlarıyla anar.
  - İfadeleri dört oyuncu da görür.
  - Her takım, ilk oyuncusunun (savunmacı, yoksa hücumcu) takımını, formasını ve gol şovunu giyer.
- **Bağlantı kopunca:** Maç sırasında bağlantısı kopan oyuncunun koltuğuna bilgisayar geçer ve maç sürer. Lobiden ayrılanın koltuğu boşalır.
- **Maç sonu:** Rövanş aynı koltuklarla oynanır. Masayı açanın **Menü** düğmesi herkesi koltuklara geri götürür; orada yer değiştirip yeni maça başlanabilir. Masayı açan moladan "Menüye dön" derse masa kapanır.
- 2v2 online maçları online maç sayılır; kazanan takımdakiler galibiyet, kaybedenler mağlubiyet alır.
- Bağlantı 1v1 ile aynıdır: claude.ai odası ya da PeerJS. Masa en çok dört telefonu alır; dolu bir masaya giren "Bu masa dolu" mesajını görür.

#### Online turnuva (sekiz telefona kadar)

Online ekranındaki **Turnuva masası aç** herkesin kendi telefonundan katıldığı bir eleme turnuvası açar. Diğerleri **Masaya katıl** ile masa koduyla girer.
- **Masa:**
  - Katılanların adları listelenir; en çok sekiz kişi oturabilir.
  - Masayı açan takım sayısını (4 ya da 8; dörtten fazla kişi varsa 8) ve bilgisayar takımlarının seviyesini seçer. Diğerleri bu seçimi görür.
  - En az iki kişiyle **Kura çek ve başla** ağacı çeker; boş yerleri adlı bilgisayar takımları doldurur.
  - Kura çekildikten sonra masaya yeni oyuncu alınmaz.
- **Maçlar:** Maçlar sırayla, masayı açan telefonun masasında oynanır.
  - Sıradaki maçın iki oyuncusu kendi telefonlarından oynar. Bilgisayar takımına karşı oynayan, o takımın seviyesiyle karşılaşır.
  - Masadaki herkes maçı canlı izler: izleyenlerin tuşları gizlenir ve köşede "👁 İzliyorsun" yazar.
  - Masayı açan da kendi maçı yoksa izler.
  - Kırmızı taraftaki oyuncunun ekranı ters döner. Skor tablosunda ve spikerde takım adları geçer.
- **Akış:**
  - Ağaç herkesin ekranında aynıdır. Sıradaki maçı yalnızca masayı açan başlatır; bilgisayar – bilgisayar maçlarını da o sonuçlandırır.
  - Ağaçta kendi adının yanında "(sen)" yazar; alttaki satır sıranın sende mi olduğunu, yoksa izleyeceğini söyler.
  - Maç bitince masayı açan **▶ Turnuva ağacı** ile herkesi ağaca döndürür. Final bitince herkes şampiyonu görür.
  - Ağaç kapatılırsa oyuncu listesine dönülür; **Ağacı göster** ağacı yeniden açar.
- **Bağlantı kopunca:** Kopan oyuncunun yerine, onun adıyla 🤖 bir bilgisayar takımı (Kulüp) oynar. Maç sırasındaysa maç sürer.
- **İlerleme:** Her telefon yalnızca kendi oynadığı maçları online maç olarak sayar; izlenen maçlar sayılmaz. Masayı açanın telefonda süren tek telefonluk turnuvası bozulmaz.

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
- `firestore.rules`: dünya tablosu ve özel ligler için Firestore güvenlik kuralları
