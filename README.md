# Bilnex Dashboard — güncelleme kaynağı

Bu depo sadece `apps.json` dosyasını barındırır: uygulamanın sürüm bilgisi ve
indirme adresi. Uygulamanın kendisi (ipa) burada değil, ofis sunucusunda durur.

Telefonda AltStore/SideStore'a eklenecek kaynak adresi:

```
https://raw.githubusercontent.com/myste123/bilnex-dashboard-source/main/apps.json
```

Bu adres hiç değişmez. `apps.json` içindeki indirme adresi ofis sunucusunun
Cloudflare tüneline işaret eder ve tünel adresi değiştiğinde
`.github/workflows/sync_source.yml` tarafından yarım saatte bir otomatik
güncellenir.
