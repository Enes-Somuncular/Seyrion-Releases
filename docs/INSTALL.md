# Portable kullanım ve güncelleme

Windows 11 x64. ZIP paketindeki .NET çalışma zamanı dahildir.

1. Sürüm varlıklarından `Seyrion-VERSION-win-x64-portable.zip` dosyasını indir.
2. Tamamını kendi kullanıcı hesabının yazabildiği bir klasöre çıkar. `Program Files` gibi korunan klasörler uygun değildir.
3. Ana klasördeki `Seyrion.exe` başlatıcısını aç. Sürüme ait alt klasörden açmak yerine her zaman bu başlatıcıyı kullan.
4. Tepsiye küçültmek izlemeyi devam ettirir; X/Çıkış ise kaydederek kapatır.

Güncelleme: uygulamada **Güncellemeler → Şimdi denetle → Güncellemeyi indir → Yeniden başlat ve güncelle**. Önce günlük veriler kaydedilir, ardından uygulama kapanıp yeni sürümle açılır. `UserData` klasöründeki geçmiş ve tercihler korunur. İndirme başarısızsa mevcut sürüm kullanılabilir.

Kanal: **Stabil** beta paketlerini almaz. **Beta** ön sürümleri ve daha yeni stabil sürümleri alabilir. Kanal değişikliği otomatik sürüm düşürmez. Beta sürümün numarası mevcut stabil sürümden yüksekse daha yeni stabil yayımlanana kadar beklenir.

Güncelleme denetimi için GitHub erişimi gerekir. Ağ yoksa veya GitHub istek sınırına ulaşılmışsa daha sonra yeniden dene. Ölçüm ve günlük geçmiş çevrimdışı çalışır. Otomatik denetim uygulamadan kapatılabilir.

Uygulama Authenticode imzalı değildir. SmartScreen uyarısı çıkabilir; indirdiğin paketin resmî depodan geldiğini ve dosya hash'ini doğrula. Windows güvenlik özelliklerini kapatman gerekmez.

PowerShell ile ZIP hash'i:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Seyrion-VERSION-win-x64-portable.zip'
```

Sonucu aynı sürümdeki `SHA256SUMS.txt` ile karşılaştır.

Kaldırmak için uygulamadan çıkıp portable klasörünü silebilirsin. Geçmişini korumak istersen önce **UserData** klasörünün yedeğini al. Eski İstatist geçmişi ilk varsayılan açılışta kopyalanır; eski kayıtlar silinmez.
