<p align="right"><a href="README.md">Türkçe</a> · <strong>English</strong></p>
<div align="center">
<img src="brand/logo.svg" width="82" alt="Seyrion" />

# Seyrion
**See your system's rhythm.**

Live resource monitoring and a clear daily history for Windows 11.

**[Download stable](https://github.com/Enes-Somuncular/Seyrion-Releases/releases/latest)** · [Beta & all releases](https://github.com/Enes-Somuncular/Seyrion-Releases/releases)

<img src="brand/hero.svg" width="100%" alt="Seyrion brand illustration" />
</div>

CPU and RAM overview, grouped process usage, daily CPU time and private-memory summaries, process I/O, CSV export, a tray icon, and in-app portable updates. The current application interface is in Turkish.

Download **Seyrion-VERSION-win-x64-portable.zip**, extract everything to a writable folder, and run the top-level **Seyrion.exe**. Windows 11 x64 is required. No installer, administrator access or separate .NET installation is needed. Keep all portable files together.

Switch between **Stabil / Beta** in **Güncellemeler**. Use **Şimdi denetle → Güncellemeyi indir → Yeniden başlat ve güncelle** to update in place. Switching channels does not automatically downgrade. Beta users can receive newer stable releases too.

History and preferences live in **UserData** under the portable root, survive updates, and are not uploaded. Daily summaries are kept for up to 30 days. Optional automatic update checks contact GitHub on startup and every 30 minutes; downloads and restarts require a button press.

GPU/watt telemetry, FPS, game reports and automatic recommendations are planned, not included yet. Private memory is not physical RAM; process I/O is not separated into disk and network. Protected or short-lived processes may be missing. Long-running and multi-device validation is ongoing.

The application is currently unsigned with Authenticode, so Windows SmartScreen may show a warning. SHA256SUMS.txt is supplied for integrity checks. This repository contains **compiled downloads and product documentation only**. Application source is private. GitHub's automatic “Source code” archives are not application packages.
