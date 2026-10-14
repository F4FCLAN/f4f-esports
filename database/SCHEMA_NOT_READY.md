# Veri tabanı bağlantısı — henüz tamamlanmadı

İstenen gerçek özellikler için bir Supabase projesi ve uygulama kodu bağlantısı gerekir. Şu anda bu paket, gerçek veri tabanı bağlantısını içermiyor. Sadece GitHub Pages'e yüklemek form gönderimlerini site sahibine iletmez ve gerçek yönetici oturumu oluşturmaz.

Gerekli tablolar/işlevler:
- `players`: nick, rank, avatar yolu, aktiflik/sıra
- `matches`: rakip klan, tarih, saat, skor, sonuç
- `match_requests`: iki rank, rakip klan, iletişim, istenen tarih/saat, durum, takip kodu
- `join_applications`: oyun içi nick, ad soyad, yaş, rank, tanıtım, durum, takip kodu
- sunucu tarafında saat çakışmasını önleme
- yalnızca yetkili yöneticinin onay/red ve kadro düzenleme işlemi yapabilmesi
- herkese açık sorgularda başvuru sahiplerinin kişisel bilgilerinin gösterilmemesi

Bu şema/bağlantı uygulanmadan siteyi gerçek başvurular için kullanmayın.
