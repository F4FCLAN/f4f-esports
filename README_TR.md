# F4F Esports — Kurulum paketi

Bu paket F4F Esports sitesinin yeni tasarımlı HTML prototipini ve logo dosyalarını içerir.

## Dosyalar
- `index.html`: Site arayüzü prototipi.
- `assets/f4f-main-logo.jpeg`: Ana F4F logosu.
- `assets/f4f-controller-logo.jpeg`: Kontrolcü logolu görsel.
- `database/SCHEMA_NOT_READY.md`: Ortak veri tabanı bağlantısına dair önemli not.

## Önemli durum
Bu sürüm henüz canlı kullanıma hazır tam bir web uygulaması değildir. Arayüz prototipidir. Başvuruların bütün cihazlardan ortak görünmesi, gerçek yönetici girişi, dosya/fotoğraf yükleme, başvuru takip kodu ve aynı saate çift maç rezervasyonunu engelleyen sunucu tarafı kurallar için bir veri tabanı/arka uç bağlantısı tamamlanmalıdır. Bu pakette gerçek yönetici parolası veya gizli anahtar bulunmaz.

## GitHub Pages ile yalnızca arayüzü yayımlama
1. GitHub hesabı açın veya giriş yapın: https://github.com/
2. `New repository` ile `f4f-esports` adında yeni bir repository oluşturun.
3. Ücretsiz GitHub hesabında GitHub Pages yayımlaması için repository'yi `Public` seçin. Yayımlanan sayfa herkese açık olur; gizli bilgi yüklemeyin.
4. `Add file` → `Upload files` seçeneğiyle bu klasörün içindeki `index.html`, `README_TR.md` ve `assets` klasörünü yükleyin. `index.html` repository ana dizininde olmalı.
5. `Commit changes` düğmesine basın.
6. Repository içinde `Settings` → `Pages` bölümüne girin.
7. `Build and deployment` altında `Deploy from a branch` seçin; branch olarak `main`, klasör olarak `/(root)` seçip `Save` basın.
8. Birkaç dakika sonra aynı Pages bölümünde görünen site bağlantısını açın.

Bu adımlar sadece statik arayüzü yayımlar; veri tabanı ve yönetici paneli bağlantısını tamamlamaz.

## Güvenlik
- Yönetici parolası, Supabase `service_role` anahtarı veya başka gizli anahtarları GitHub'a koymayın.
- Kullanıcıların adı/soyadı ve yaş gibi kişisel bilgileri demo aşamasında gerçek kullanıcılarla toplamayın.
- Gerçek yayından önce kimlik doğrulama, yetkilendirme, veritabanı erişim politikaları ve form doğrulamaları tamamlanmalıdır.
