# Tashkent City — Windows test o‘yini

Tashkent City, AUT universiteti, park va Humo Arena atrofida haydash va erkin yurish uchun **alpha test versiyasi**. Uzbek, English va Russian tillari mavjud. Bu repository tayyor o‘yin paketini va tester yo‘riqnomasini tarqatadi.

**[O‘yinni yuklash — alpha-20261003-aut1](https://github.com/Shahzod1602/Tashkentcity_-gtastyle/releases/tag/alpha-20261003-aut1)**

## Yuklash va ochish

1. Release sahifasidan quyidagi **5 faylni bitta papkaga** yuklang:
   - `TashkentCity-alpha-20261003-aut1.zip.001`
   - `TashkentCity-alpha-20261003-aut1.zip.002`
   - `Join.Test.ZIP.cmd`
   - `Join-Test-ZIP.ps1`
   - `TEST_PARTS.json`
2. `Join.Test.ZIP.cmd` ni oching. U qismlarning SHA-256 qiymatlarini tekshiradi va ZIP faylini yig‘adi.
3. Hosil bo‘lgan ZIP ichidagi barcha fayllarni chiqaring.
4. `Play Tashkent City.cmd` ni oching. Unreal Editor kerak emas.
5. `VCRUNTIME` yoki `MSVCP` yetishmasa, paketdagi `Install Runtime.cmd` ni ishga tushiring.
6. Til va grafikani tanlang: **O‘ynash → Erkin yurish → mashina tanlash → boshlash**.

Windows x64 kerak. Yuklash, ZIP yig‘ish va chiqarish uchun kamida **11 GB bo‘sh joy** ajrating. GitHub’ning avtomatik `Source code (zip/tar.gz)` fayllari o‘yin paketi emas.

## Tester uchun

Avval **Muvozanatli / Balanced** grafikada sinang. 20–30 daqiqa davomida kunduz va tunda shahar, mashinaga kirish/chiqish, tormoz, faralar, svetoforlar, piyodalar, poyga va saqlab qayta ochishni tekshiring.

Muammo topsangiz [Issues](https://github.com/Shahzod1602/Tashkentcity_-gtastyle/issues) bo‘limida PC tarkibi, grafik sozlamalari, FPS, takrorlash qadamlari va rasm yoki qisqa videoni yuboring. `FEEDBACK_TEMPLATE.txt` paket ichida bor. Hech qanday fikr yoki log avtomatik yuborilmaydi.

Boshqaruv: **WASD** harakat/haydash; **E** interaksiya/mashinaga kirish; **Space** sakrash/qo‘l tormozi; **C** kamera; **M** xarita; **G** garaj; **B** radio; **N** keyingi trek; **L** faralar; **Esc** pauza. Tugmalarni Sozlamalar → Boshqaruv’dan o‘zgartirish mumkin.

Progress, sozlamalar va loglar `%LOCALAPPDATA%\TashkentCityTest` ostida saqlanadi.

## Joriy cheklovlar

- Bu tugallanmagan **Development alpha**; shahar hali to‘liq 1:1 rekonstruksiya emas.
- RTX 3050 Laptop 4 GB, Ryzen 5 6600H, 16 GB RAM qurilmasida 1280×720 Balanced sinovi taxminan **49 FPS**, p95 **28,5–28,8 ms** bo‘lgan. Bu boshqa PC uchun kafolat yoki minimal talab emas; RTX 5080 hali sinovdan o‘tmagan.
- Avtomatik poyga tekshiruvi to‘liq fizik aylanani qamramaydi. Toza PC’da runtime o‘rnatilishi ham tester tekshiruvi talab qiladi.
- Asset manbalari va mavjud litsenziya qaydlari paketdagi `SourceNotices` papkasida. Bu repository uchinchi tomon assetlariga yangi litsenziya bermaydi.

## English quick start

Download both numbered ZIP parts, `Join.Test.ZIP.cmd`, `Join-Test-ZIP.ps1` and `TEST_PARTS.json` from the Release into one folder. Run the joiner, extract the verified ZIP, then launch `Play Tashkent City.cmd`. Windows x64 and 11 GB free space are needed; Unreal Editor is not required.

Start with Balanced graphics. Please report PC specifications, settings, FPS and reproduction steps in Issues. The package includes English instructions and a feedback template. This is an unfinished alpha, with no RTX 5080 benchmark or guaranteed performance on other PCs.
