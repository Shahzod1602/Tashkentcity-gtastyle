# Tashkent City — Windows test o‘yini

Tashkent City, AUT universiteti, park va Humo Arena atrofida haydash va erkin yurish uchun **alpha test versiyasi**. O‘zbekcha, English va Russian tillari mavjud.

## O‘yinni yuklash

### [⬇ Install.TashkentCity.exe — yangi versiyani yuklash](https://github.com/Shahzod1602/Tashkentcity-gtastyle/releases/download/alpha-20261006-street-combat/Install.TashkentCity.exe)

**Versiya: alpha-20261006-street-combat · 2026-10-06**

1. Yuqoridagi **bitta faylni** yuklab, oching.
2. O‘yin uchun papka tanlang va **O‘rnatish** tugmasini bosing.
3. Tugagach **O‘yinni ochish** tugmasini bosing. Ish stolida ham yorliq yaratiladi, agar belgisini olib tashlamasangiz.

![Tashkent City o‘rnatuvchisi](images/installer.png)

O‘rnatuvchi **32 KB**; u **3,34 GB** o‘yin paketini yuklaydi, fayllarni tekshiradi va avtomatik chiqaradi. Internet uzilsa, o‘rnatuvchini o‘sha papka bilan yana ochib davom ettiring. Papka tanlovi eslab qolinadi. Muvaffaqiyatli o‘rnatishdan keyin yuklash arxivlari avtomatik tozalanadi.

**Windows 64-bit**, internet va o‘rnatish davomida kamida **11 GB bo‘sh joy** kerak. O‘yin o‘rnatilgach taxminan **3,7 GB** joy egallaydi. GitHub hisobi, Unreal Editor va 7-Zip talab qilinmaydi. Bu alpha o‘rnatuvchi raqamli imzo bilan imzolanmagan; Windows ogohlantirish ko‘rsatishi mumkin.

O‘yin ochilmasa va `VCRUNTIME` yoki `MSVCP` yetishmasa, **O‘yin papkasi** orqali paketdagi `Install Runtime.cmd` ni oching. O‘yinda til va grafikani tanlang: **O‘ynash → Erkin yurish → mashina tanlash → boshlash**.

Oldingi o‘rnatish o‘z papkasida qoladi. Progress va sozlamalar avvalgi `%LOCALAPPDATA%\TashkentCityTest` katalogida saqlanadi. Yangi versiya bilan o‘ynash uchun yangi o‘rnatuvchi yaratgan o‘yin papkasini yoki yorliqni oching.

## Yangi imkoniyatlar

- Shaharda SCAR va PMX bilan otish, alohida o‘q zaxiralari, qayta o‘qlash, qurol tanlash va panaga kirish.
- Sog‘liq va bronya, xavfdan qochadigan piyodalar, mashinalarga o‘q zarari, politsiya ta’qibi va qidiruvi, yengilish yoki ushlanishdan keyin qayta jonlanish.
- Personaj tanlash: **Esc → Personaj**. Rul boshqaruvi yaxshilangan, drift paytida shina tutuni chiqadi.
- Alohida jang maydoni, erkin yurish va poyga rejimlari saqlangan.

**Jang boshqaruvi:** E bilan mashinadan tushing; **Tab** ni ushlab qurol tanlang; o‘ng sichqoncha — nishon; chap sichqoncha — otish; **R** — qayta o‘qlash; **C** — piyoda turganda pana; **F** — yengilgandan keyin qayta jonlanish. **Esc → Jang** orqali maydonga kirish yoki qidiruvsiz vaqtda bepul o‘q/bronya olish mumkin.

<details>
<summary>Muqobil usul: ZIP qismlarini qo‘lda yuklash</summary>

1. [Release sahifasidan](https://github.com/Shahzod1602/Tashkentcity-gtastyle/releases/tag/alpha-20261006-street-combat) quyidagi **5 faylni bitta papkaga** yuklang:
   - `TashkentCity-alpha-20261006-street-combat.zip.001`
   - `TashkentCity-alpha-20261006-street-combat.zip.002`
   - `Join.Test.ZIP.cmd`
   - `Join-Test-ZIP.ps1`
   - `TEST_PARTS.json`
2. `Join.Test.ZIP.cmd` ni oching. U qismlarni tekshiradi va ZIP faylini yig‘adi.
3. ZIP ichidagi barcha fayllarni chiqaring va `Play Tashkent City.cmd` ni oching.

GitHub’ning avtomatik `Source code (zip/tar.gz)` fayllari o‘yin paketi emas. Qo‘lda yuklangan arxivlarni o‘zingiz tozalashingiz mumkin.

</details>

## Tester uchun

Avval **Muvozanatli / Balanced** grafikada sinang. 20–30 daqiqa davomida kunduz/tun, haydash, drift, piyodalar, faralar, svetoforlar, personaj tanlash, shahar jangi, politsiyadan qochish, poyga va saqlab qayta ochishni tekshiring.

Muammo topsangiz [Issues](https://github.com/Shahzod1602/Tashkentcity-gtastyle/issues) bo‘limida PC tarkibi, grafik sozlamalari, FPS, takrorlash qadamlari va rasm yoki qisqa videoni yuboring. `FEEDBACK_TEMPLATE.txt` paket ichida bor. Hech qanday fikr yoki log avtomatik yuborilmaydi.

Boshqaruv: **WASD** harakat/haydash; **E** interaksiya/mashinaga kirish; **Space** sakrash/qo‘l tormozi; **C** mashinada kamera, piyoda pana; **M** xarita; **G** garaj; **B** radio; **N** keyingi trek; **L** faralar; **Esc** pauza. Tugmalarni Sozlamalar → Boshqaruv’dan o‘zgartirish mumkin.

Progress, sozlamalar va loglar `%LOCALAPPDATA%\TashkentCityTest` ostida saqlanadi. Repository’da Unreal loyihasining manba kodi joylanmagan.

## Joriy cheklovlar

- Bu tugallanmagan **Development alpha**; shahar hali to‘liq 1:1 rekonstruksiya emas.
- Vertolyot, SWAT, mashinadan otish va maxsus pana animatsiyalari hozircha yo‘q. Politsiya mavjud shahar odami modeli bilan ishlaydi.
- Yakuniy o‘yin faylida **382 ta** gameplay/regressiya tekshiruvi o‘tgan, **8 ta** o‘yin tasviri ko‘z bilan tekshirilgan. O‘rnatuvchining **24 ta** tekshiruvi ham o‘tdi; o‘rnatilgan **107 ta** payload fayli asl paket bilan hajmi va SHA-256 bo‘yicha mos.
- Yangi versiya uchun FPS/p95/p99 qayta o‘lchanmagan. Oldingi 3-oktabr alpha’da RTX 3050 Laptop 4 GB, Ryzen 5 6600H, 16 GB RAM, 1280×720 Balanced o‘lchovi taxminan **49 FPS**, p95 **28,5–28,8 ms** edi. Bu boshqa PC uchun kafolat yoki minimal talab emas; RTX 5080 hali sinovdan o‘tmagan.
- Avtomatik poyga tekshiruvi to‘liq fizik aylanani qamramaydi. Toza PC’da runtime o‘rnatilishi ham tester tekshiruvi talab qiladi.
- Asset manbalari va mavjud litsenziya qaydlari paketdagi `SourceNotices` papkasida. Bu repository uchinchi tomon assetlariga yangi litsenziya bermaydi.

## English quick start

[Download Install.TashkentCity.exe](https://github.com/Shahzod1602/Tashkentcity-gtastyle/releases/download/alpha-20261006-street-combat/Install.TashkentCity.exe), open it, choose a folder and click **O‘rnatish** (Install). It downloads, verifies and extracts the game automatically. Click **O‘yinni ochish** (Open game) when finished. Interrupted downloads resume when you retry with the same folder.

The installer is 32 KB; the game download is 3.34 GB. Windows x64 and 11 GB free space during installation are needed. GitHub login, Unreal Editor and 7-Zip are not required. The alpha installer is unsigned. If the game reports missing VCRUNTIME/MSVCP, use the bundled `Install Runtime.cmd`.

Start with Balanced graphics. Please report PC specifications, settings, FPS and reproduction steps in Issues. This is an unfinished alpha, with no RTX 5080 benchmark or guaranteed performance on other PCs.

New: city gunplay, police pursuit, pedestrian reactions, cover, health/armor, character selection and drift smoke. Leave the car with E; hold Tab for weapons; right mouse aim, left mouse fire, R reload, C cover. Existing saves remain under `%LOCALAPPDATA%\TashkentCityTest`. No new FPS benchmark was run for this release.
