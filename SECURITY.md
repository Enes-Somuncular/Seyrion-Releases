# Seyrion güvenlik politikası

Seyrion'un kaynak kodu özeldir. Bu depo yalnızca derlenmiş uygulamayı ve ürün belgelerini yayımlar.

## Güvenlik açığı bildirimi

Güvenlik açığı ayrıntılarını, özel bilgileri veya çalıştırılabilir istismar kodunu herkese açık issue olarak paylaşma. Security sekmesinde **Report a vulnerability** varsa özel bildirim kullan; yoksa [geliştiricinin GitHub profili](https://github.com/Enes-Somuncular) üzerinden özel bir iletişim kanalı iste.

## Doğrulama sınırları

SHA-256 dosya eşleşmesini kontrol eder. GitHub **Immutable** sürümleri GitHub CLI ile ayrıca doğrulanabilir. Bunlar yazılımın zararsız olduğunu veya kaynak kodun bağımsız denetlendiğini kanıtlamaz.

Seyrion'un mevcut sürümleri Authenticode imzalı değildir. Windows güvenlik özelliklerini kapatman gerekmez. [Doğrulama rehberi](docs/VERIFY.md).
