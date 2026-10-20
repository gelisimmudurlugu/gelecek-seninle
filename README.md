# Gelecek Seninle — GitHub Pages sürümü

## Bilgisayarınızda açma
index.html dosyasını çift tıklayarak tarayıcıda açın. Ek kurulum veya internet bağlantısı gerekmez.

## GitHub Pages üzerinde yayınlama
1. GitHub hesabınızda `gelecek-seninle` adında yeni bir repository oluşturun. GitHub Free ile yayınlamak için Public seçin.
2. Add file > Upload files ile yalnızca bu paketin kökündeki `index.html` dosyasını yükleyin. Commit changes seçin.
3. Settings > Pages > Build and deployment > Source bölümünde Deploy from a branch seçin.
4. Branch: main; Folder: /(root); Save.
5. Yayın tamamlandığında adres aynı ekranda gösterilir. Genel biçimi: https://KULLANICI-ADINIZ.github.io/gelecek-seninle/

Resmi yönerge: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

GitHub Pages yayını internete açıktır. Kurum içi erişim için kurumunuzun barındırma/erişim çözümünü kullanın.

## Çalışan özellikler
10 ekranlık Story rehberi, ileri/geri geçiş, otomatik oynatma, yolculuk haritası, modül ve deneyim pencereleri, SSS araması ve program bilgi tabanıyla yanıt veren sohbet.

Bu sürüm harici API çağırmaz. Sohbet üretken AI değildir; program bilgileri üzerinden eşleştirme yapar. Kullanıcı sohbetleri yalnızca açık sayfanın belleğinde tutulur.

## Kaynak kodlarını düzenleme
- index.html: doğrudan açılan, tüm JavaScript ve CSS'i içeren yayın dosyası.
- editable-source/: bu tek dosyalık sürümün okunabilir React/TypeScript kaynakları. Home.tsx tasarım ve etkileşimleri; program.ts soru/yanıt ve Story metinlerini; styles.css görsel tasarımı içerir.
- original-site/: Codex'te oluşturulup yayınlanan özgün sitenin kaynak kodları. Bu proje Vinext/Cloudflare tabanlıdır; doğrudan GitHub Pages'e yüklenerek çalışmaz. Yayın için kökteki index.html dosyasını kullanın. Özgün Sites kimliği dışa aktarıma dahil edilmemiştir.

## Tek dosyayı yeniden üretme (teknik kullanıcılar için)
editable-source klasöründe Node.js 22+ kurulu bir bilgisayarda:
  npm install
  npm run build
Komut aynı klasörde yeni bir index.html üretir. Yeni index.html dosyasını GitHub repository köküne yükleyin.

İçerik bu dışa aktarım sırasında mevcut siteden alınmıştır. Programda sonraki değişiklikler kendiliğinden bu dosyaya yansımaz.
