# Seyrion indirmesini doğrula

Kaynak kod özel kalırken indirilen paketin bütünlüğünü kontrol edebilirsin. Bu kontroller, uygulamanın zararsız olduğunun garantisi değildir.

## 1. Resmî dosyaları indir

[Resmî Releases](https://github.com/Enes-Somuncular/Seyrion-Releases/releases) sayfasından portable ZIP'i ve **aynı sürümün** `SHA256SUMS.txt` dosyasını indir.

## 2. SHA-256 kontrolü

PowerShell'de, VERSION yerine indirdiğin sürümü yazarak:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Seyrion-VERSION-win-x64-portable.zip'
```

Sonuç `SHA256SUMS.txt` dosyasındaki ZIP satırıyla uyuşmalıdır. Uyuşmuyorsa çalıştırma. Aynı GitHub hesabından sunulan dosya ve hash, ele geçirilmiş hesaba karşı tek başına güvence değildir.

## 3. Değiştirilemez GitHub sürümleri

Sürüm **Immutable** olarak işaretliyse [GitHub CLI](https://cli.github.com/) kurup şu doğrulamaları çalıştırabilirsin:

```powershell
gh release verify vVERSION -R Enes-Somuncular/Seyrion-Releases
gh release verify-asset vVERSION '.\Seyrion-VERSION-win-x64-portable.zip' -R Enes-Somuncular/Seyrion-Releases
```

VERSION ve ZIP dosya adını gerçek sürüme göre değiştir. Önceden immutable olarak yayımlanmamış sürümler bu yöntemle doğrulanamayabilir.

## 4. Güvenlik hakkında

Mevcut paketler Authenticode imzalı değildir. Antivirüs taraması, ağ davranışı incelemesi veya sanal makinede test ek sinyaller verebilir; hiçbiri kusursuz garanti sağlamaz. [Güvenlik politikası](../SECURITY.md).
