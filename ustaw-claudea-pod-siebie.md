# Ustaw Claude'a pod siebie
**Poradnik · 8 kroków · zero kodowania**
Autor: Heredero (github.com/heredero7)

---

## Czego potrzebujesz

Bezpłatne konto na claude.ai. Plan darmowy daje Memory i Instructions for Claude. Projects, wyszukiwanie historii czatów i wyższe limity — w Claude Pro (~20 USD/mies.).

**Ważne:** Zacznij od kroku 01 (Memory). Bez niej żadne inne ustawienie się nie utrwali.

---

## Krok 01 — Włącz Memory

**Gdzie:** Settings → Capabilities → sekcja Memory → włącz „Generate memory from chat history". Na płatnym planie włącz też „Search and reference chats".

**Po co:** Memory jest bezpłatna. Claude pamięta kontekst między rozmowami zamiast zaczynać od zera przy każdym czacie.

**Wskazówki:**
- Daj mu do 24 godzin na zbudowanie pamięci z dotychczasowej historii.
- Kliknij „View and manage memory", żeby zobaczyć i edytować każdy zapisany fakt. Zaglądaj tam co jakiś czas.
- Jeśli wcześniej używałeś ChatGPT lub Gemini: w tej samej sekcji znajdziesz „Import memory from other AI providers" — możesz przenieść kontekst.

---

## Krok 02 — Powiedz mu, kim jesteś

**Gdzie:** Settings → General → pole „Instructions for Claude".

**Po co:** To Twoje stałe przedstawienie się. Ładuje się automatycznie do każdego nowego czatu na każdym planie. Napisz raz — Claude przestaje zgadywać, kim jesteś.

**Szablon do skopiowania:**

```
O MNIE
Nazywam się [Imię]. Prowadzę [nazwa firmy], czyli [czym się zajmujesz]
dla [kogo obsługujesz] — albo: pracuję jako [stanowisko] w firmie
[nazwa firmy], gdzie odpowiadam za [główne obowiązki].

Moja główna oferta to [oferta] w cenach [ceny] — albo: moje główne
zadania to [lista zadań].

Teraz najbardziej zależy mi na [Twój cel na ten okres], a moim
klientom/odbiorcom na [rezultat, którego chcą].

Na co dzień pracuję w [narzędzia], a w [Twój obszar] jestem na
poziomie [początkujący / średnio zaawansowany / zaawansowany] —
nie tłumacz mi podstaw z tego obszaru.

Mów do mnie jak do doświadczonego praktyka: konkretnie,
bezpośrednio i szczerze, bez wstępów i wypełniaczy.
```

---

## Krok 03 — Ustaw swój głos i zasady

**Gdzie:** To samo pole „Instructions for Claude" — dopisz poniżej akapitu o sobie.

**Po co:** Pozbywasz się generycznego tonu AI. Mówisz Claude'owi, czego ma unikać i jak ma brzmieć.

**Szablon do skopiowania:**

```
GŁOS I ZASADY
Pisz prostym, pewnym językiem. Bez korpomowy, napompowanych
słów i typowych wzorców AI. Najpierw sedno, potem uzasadnienie.
Jeśli masz dla mnie niewygodną odpowiedź, podaj ją w pierwszym zdaniu.
Zanim doradzisz w sprawie cen, produktów, narzędzi albo aktualnych
faktów — najpierw sprawdź w sieci. Twoja wiedza się dezaktualizuje.
Kwestionuj moje rozumowanie, nie potakuj. Jeśli widzisz błąd, ryzyko
albo lepsze podejście — powiedz to z własnej inicjatywy.
Gdy doradzasz, daj jedną konkretną rekomendację, a nie listę opcji.
Czegoś nie wiesz — powiedz wprost, nie zmyślaj. Bądź zwięzły.
```

---

## Krok 04 — Podziel pracę na Projects

**Gdzie:** Lewy pasek boczny → Projects → „+ New Project". Po wejściu w projekt: „Set project instructions".

**Po co:** Każdy projekt ma osobne instrukcje i osobne pliki. Praca z klientami nie miesza się z marketingiem. Dostępne w płatnych planach.

**Zasada nazewnictwa:** Nazywaj projekty po zadaniach, nie po klientach. „Treści" i „Operacje" będziesz używał latami. „Klient X" porzucisz.

Przykładowe projekty: Treści, Klienci, Operacje.

---

## Krok 05 — Załaduj swoje pliki

**Gdzie:** Otwórz projekt → przeciągnij pliki do bazy wiedzy projektu.

**Obsługiwane formaty:** PDF, DOCX, CSV, TXT, HTML i inne.

**Co wrzucać:** Przewodnik po marce, najlepsze oferty, skuteczne strony sprzedażowe, materiały produktowe.

**Po co:** Claude odpowiada na podstawie Twoich materiałów, a nie internetowej przeciętności. Pliki są dostępne w każdym czacie wewnątrz projektu — bez ponownego wklejania.

**Ważne:** Nie wrzucaj dziesiątek niepowiązanych dokumentów do jednego projektu. Im więcej przypadkowego materiału, tym gorsza jakość odpowiedzi.

---

## Krok 06 — Połącz swoje aplikacje

**Gdzie:** Lewy pasek boczny → Customize → sekcja konektorów.

**Co podłączyć:** Google Drive, Gmail, Google Calendar.

**Po co:** Claude wyciągnie dokument z Drive'a, napisze szkic na podstawie prawdziwego wątku mailowego, sprawdzi Twój tydzień w kalendarzu — bez ręcznego wklejania. Każda akcja wymaga Twojej zgody. Anthropic nie trenuje modeli na danych z konektorów.

---

## Krok 07 — Ustaw swój styl pisania

**Gdzie:** Customize → Skills → kliknij „+" → „Browse skills".

**Po co:** Styl pisania to oddzielny mechanizm od Instructions. Instructions mówią Claude'owi, kim jesteś. Skill mówi mu, jak pisać w danej rozmowie — przydatne gdy raz piszesz posty na LinkedIn, a raz maile do klientów.

**Jak używać:** Skille są domyślnie wyłączone. Włącz wybrany w Customize → Skills, a wywołaj go w rozmowie komendą `/nazwa-skilla`.

Możesz też zbudować własny skill.

---

## Krok 08 — Web Search i tryb Incognito

### Web Search

Przy polu tekstowym jest ikona globusa. Po włączeniu Claude sięga po aktualne dane z internetu, a nie tylko po wiedzę treningową. Przydaje się przy cenach, nowościach, przepisach i wszystkim, co mogło się zmienić. Włączasz osobno dla każdego czatu.

### Tryb Incognito

W prawym górnym rogu każdego nowego czatu jest ikona ducha. Otwiera rozmowę, która:
- nie zapisuje się do historii
- nie trafia do Memory
- nie służy do trenowania modeli

**Kiedy używać:** Wrażliwe dane firmowe, dane osobowe klientów, cokolwiek czego nie chcesz w historii.

---

## Jak rozmawiać z Claude

### Daj kontekst, nie samo polecenie

„Napisz maila" da generyczny tekst. „Napisz maila do klienta, że projekt opóźni się o dwa tygodnie — szczerze, ale tak, żeby nie stracić jego zaufania, do 150 słów" da coś, co naprawdę wyślesz.

### Iteruj, nie licz na strzał

Pierwsza odpowiedź to punkt startu. Poprawiaj w rozmowie: „za formalne", „skróć o połowę", „dodaj konkretny przykład". Claude pamięta całą rozmowę — nie zaczynasz od zera.

### Zacznij nowy czat, gdy rozmowa dryfuje

Po wielu wiadomościach na różne wątki jakość spada — Claude miesza tematy. Gdy odpowiedzi schodzą z tematu, otwórz świeży czat. Dzięki Memory i projektom nic nie tracisz.

---

## Który model wybrać

Pod polem tekstowym widać, z którym modelem rozmawiasz. Na darmowym planie nie zmienisz go ręcznie; na płatnym przełączasz z listy.

| Model | Do czego | Zużycie limitu |
|-------|----------|----------------|
| Haiku | Proste rzeczy: podsumowania, tłumaczenia, formatowanie | najmniejsze |
| Sonnet | Codzienna praca (domyślny): pisanie, analiza, research | umiarkowane |
| Opus | Trudne rozumowanie: złożone analizy i decyzje | duże |
| Fable | Najbardziej wymagające zadania | największe |

| Plan | Dostępne modele |
|------|-----------------|
| Free | Haiku, Sonnet |
| Pro / Max | + Opus, Fable oraz większy limit |

**Zasada:** Dopasuj model do zadania. Używanie Opusa lub Fable do wszystkiego to najszybszy sposób na komunikat o limicie. Sonnet obsłuży większość codziennej pracy.

**O limitach:** Liczą się w tokenach (ilość przetworzonego tekstu), nie w liczbie wiadomości. Odnawiają się co kilka godzin. Cięższy model zużywa limit szybciej.

---

## Artifacts

Gdy poprosisz o coś większego niż zwykła odpowiedź — dokument, stronę, tabelę, wykres, kalkulator, prostą aplikację — Claude otworzy to w osobnym oknie obok czatu. To Artifact: samodzielna rzecz, którą widzisz, edytujesz i pobierasz. Działa na każdym planie.

**Do czego się nadaje:** landing page, opis oferty gotowy do wklejenia, prosty kalkulator, tabela porównawcza, wykres z danych, materiały szkoleniowe.

**Jak używać:**
- Proś o zmiany punktowo: „zmień nagłówek", „dodaj czwartą kolumnę" — Claude poprawia tylko to.
- Pod oknem masz historię wersji, kopiowanie i pobieranie pliku.
- Gotowy Artifact możesz opublikować i udostępnić linkiem — nawet komuś bez konta Claude.
- Jeśli coś się wysypie: kliknij „Try fixing with Claude".

---

## Pliki Markdown (.md)

Markdown to zwykły tekst z kilkoma prostymi znakami nadającymi strukturę. Claude go preferuje — modele uczyły się na ogromnych ilościach Markdownu, więc to dla nich język ojczysty. Format jest lekki, więc w okno kontekstu mieści się więcej treści.

**Podstawowa składnia:**

```
# Nagłówek główny
## Mniejszy nagłówek
**pogrubienie**
*kursywa*
- punkt listy
- kolejny punkt
1. lista numerowana
[tekst linku](https://adres.pl)
> cytat albo ważna uwaga
```

**Jak zrobić plik .md:**
- Napisz tekst w Notatniku i zapisz z rozszerzeniem `.md`
- Poproś Claude'a „zapisz to jako plik .md"
- Pisz w aplikacji obsługującej Markdown: Obsidian, Notion

---

## Gotowe prompty na co dzień

### Pre-mortem (przed ważną decyzją)

```
Zanim wydam na to czas/pieniądze, wciel się w bezlitosnego
sceptyka. Wypisz wszystkie powody, dla których to się nie uda — osobno
od strony popytu, wykonania i moich założeń. Uszereguj je od
najbardziej do najmniej prawdopodobnego, a na końcu powiedz, co
musiałoby być prawdą, żeby to jednak zadziałało.
```

### Ostry redaktor (skracanie tekstu)

```
Skróć ten tekst o połowę, nie tracąc sensu. Wytnij
wodolejstwo, stronę bierną i typowe wzorce AI. Zachowaj mój głos.
Pokaż samą poprawioną wersję, a pod nią krótko wypunktuj, co
skróciłeś i dlaczego.

[wklej tekst]
```

### Nauczyciel od podstaw (nauka nowego tematu)

```
Wytłumacz mi [temat] od pierwszych zasad, prostym
językiem, bez żargonu — tak, jakbyś tłumaczył komuś bystremu, kto nie
zna tej dziedziny. Użyj jednego przykładu albo analogii. Na końcu
zadaj mi 2–3 pytania sprawdzające, czy naprawdę to zrozumiałem.
```

---

## Lista kontrolna

- [ ] Memory włączona (Settings → Capabilities)
- [ ] Instructions for Claude zapisane (Settings → Profile)
- [ ] Trzy Projects utworzone (np. Treści, Klienci, Operacje)
- [ ] Pliki wgrane do jednego Project
- [ ] Konektory podłączone (Customize)
- [ ] Styl pisania skonfigurowany jako Skill (Customize → Skills)
- [ ] Web Search przetestowany
- [ ] Tryb Incognito poznany
- [ ] Wiesz, który model wybrać (Opus i Fable palą limit najszybciej)
- [ ] Wiesz, czym są Artifacts i jak je poprawiać
- [ ] Wiesz, czym są pliki .md i że Claude je preferuje

---

## Wskazówki końcowe

**Kolejność ma znaczenie.** Najpierw Memory — inaczej nic, co ustawisz, się nie utrwali.

**Memory nie jest idealna.** Czasem Claude zapamięta coś źle lub nieaktualnie. Co jakiś czas zaglądaj do „View and manage memory" i rób porządki.

**Sprawdź prywatność.** Settings → Privacy → opcja „Help improve our AI models". Jeśli nie chcesz, żeby Twoje rozmowy służyły do trenowania, upewnij się, że jest wyłączona.

**Wrażliwe dane — zawsze Incognito.** Dane klientów, umowy, informacje poufne wklejaj tylko w trybie Incognito, nigdy w zwykłych czatach.
