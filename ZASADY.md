# ZASADY projektu

Czytam ten plik na początku każdego kroku.

## Projekt
Sklep dropshippingowy ze sprzedażą z ruchu organicznego: krótkie klipy na TikToka,
Instagram Reels i Facebook Reels. Bez płatnych reklam. Sklep: Shopify (Rzepiaki, www.rzepiaki.pl).

## Zasady
1. Używam wyłącznie konektorów (Higgsfield, Shopify, Winning Hunter, Facebook / biblioteka reklam)
   i darmowych narzędzi lokalnych (ffmpeg, yt-dlp, openai-whisper, Python + Pillow, jq).
   Żadnych płatnych API ani zewnętrznych scraperów. Jeśli czegoś nie da się zrobić bez nich,
   mówię to wprost, zamiast kombinować.
2. Przed każdą generacją obrazu, wideo albo głosu w Higgsfield sprawdzam koszt w kredytach
   i podaję sumę, zanim ruszę. Po każdym kroku podaję saldo.
3. Kopiujemy koncept, nigdy cudzy materiał. W naszych klipach i na stronie nie ma cudzego wideo,
   cudzych zdjęć, logo ani nazw marek.
4. Wszystko po polsku, dla polskiego odbiorcy. Zdania krótkie, mówione. Zero kalk z angielskiego
   i słów z reklam („rewolucyjny”, „innowacyjny”).
5. Nie wymyślam liczb ani opinii klientów. Jeśli czegoś nie widzę, piszę „brak danych”.
6. Każdy wygenerowany obraz i każde wideo oglądam sam, zanim je pokażę. Nieudane próby
   zapisuję w `nieudane/` z jednym zdaniem, co nie wyszło.
7. Jedna rekomendacja z uzasadnieniem, nie pięć opcji do wyboru.
8. Po każdym kroku raport w trzech zdaniach: co zrobiłem, co wyszło, czego potrzebuję od Ciebie.

## Pliki (płasko w tym folderze)
- `produkt.md`: wynik szukania produktu
- `referencja.mp4`: klip, którego koncept odtwarzamy
- `produkt_1.jpg`: zdjęcie produktu
- `persona.md`: dla kogo i jakim językiem
- `skrypt.md`: skrypt klipu
- `gotowe/`: klipy do publikacji
- `nieudane/`: odrzucone próby

## Uwagi o środowisku (stan na 2026-10-06)
- Winning Hunter: nawet `check_credits` zużywa 1 kredyt. Saldo sprawdzam tylko wtedy, gdy jest potrzebne.
- Font do napisów: `/usr/share/fonts/truetype/liberation/LiberationSans-Bold.ttf`
  (odpowiednik Arial Bold, polskie znaki sprawdzone). Montserrat niedostępny, bo sieć blokuje Google Fonts.
- Sieć kontenera blokuje: tiktok.com, instagram.com, facebook.com, youtube.com (yt-dlp nie pobierze
  klipów), openaipublic.azureedge.net (Whisper nie pobierze modelu), fonts.google.com.
  Dopóki to się nie zmieni, `referencja.mp4` wrzucasz ręcznie do folderu.
