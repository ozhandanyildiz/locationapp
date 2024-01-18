Uygulamada en üstte bir navbar, altında bir harita ve haritanın altında kullanıcının konum bilgisini göstermeye ve gizlemeye yarayan bir buton bulunur. Kullanıcı ilk sayfayı yüklediğinde konum erişimi için sayfa ilk yüklendiğinde alert ile konum erişimi istenir. Eğer izin verirse, harita üzerinde bu konumu işaretler.
MapComponent: Bu, harita bileşenini temsil eder. Bu bileşen, kullanıcının konumunu gösteren bir harita sunar. Kullanıcı, "Show Location" düğmesine tıklayarak konumunu gösterebilir veya gizleyebilir.

useGeoLocation: Hook kullanıcının coğrafi konumunu alır. navigator.geolocation kullanarak konumu izler ve kullanıcı konumunu sağladığında veya hata oluştuğunda uygun durumları günceller.

Redux: Uygulama, Redux kullanarak merkez koordinat, yakınlaştırma seviyesi ve işaretçiler gibi harita durumlarını yönetir. Bu durum, kullanıcının haritayı nasıl görmesi gerektiğini belirler.

mapConfig: Harita konfigürasyonunu içerir.

App: Ana uygulama bileşenidir. react-router-dom kullanarak farklı sayfaları yönlendirir. Ayrıca Provider ile Redux mağazasını sağlar ve Navbar ile ana gezinme çubuğunu, Map, SignIn, ve SignUp ile farklı sayfaları oluşturur.
