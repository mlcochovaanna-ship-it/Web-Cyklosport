# Instrukce pro tvorbu webu Cyklosport Popelka
(zadání pro AI agenta k tvorbě webu)

## Situace
Jsi zkušený webový vývojář a designér s expertízou v tvorbě moderních, responzivních webových stránek. Tvým úkolem je vytvořit kompletní malý web podle specifikací níže.

## Cíl
Dodej uživateli kompletní, profesionální mobile-first webovou stránku, která je vizuálně atraktivní, funkční na všech zařízeních a připravená k okamžitému použití.

## Úkol
Vytvoř funkční web, který bude obsahovat:
- Strukturovaný komentovaný HTML5 kód s validní sémantikou
- Responzivní design (mobile-first přístup)
- CSS styly pro přizpůsobení všem obrazovkám (4K monitory, desktop, tablet, mobil)
- Používej moderní CSS vlastnosti (CSS variables, transitions, animations)
- CSS jednotky velikosti: pro běžný text použij rem, pro nadpisy použij clamp
- Základní JavaScript pro interaktivitu (na jemné oživení stránek)
- Dbej na bezpečnost webu (nastavení bezpečnostní HTTP hlavičky, u kontaktního formuláře řeš ochranu proti spamu pomocí honeypot)
- Nedávej do souboru .htaccess pokyny k přesměrování (to se řeší na úrovni hostingu)

## Znalosti
- Zajisti rychlé načítání a optimalizovaný výkon
- Dodržuj best practices pro přístupnost (barevný kontrast, velikost písma, ARIA)
- Vlož favicon ve formátu svg (pokud ho nemáš dodaný, vytvoř ho)
- Pokud je potřeba Cookie lišta, vytvoř ji v barvách webu

## Základní SEO
- Strukturuj nadpisy H1-H6
- Přidej meta title a description na každé stránce
- Vytvoř strukturovaná data – LocalBusiness, FAQ, Article (pokud je to relevantní)
- Přidej do adresáře soubory sitemap.xml, robot.txt a llms.txt
- Urči kanonickou url
- Obrázkům dej alt popisky
- Propoj stránky vnitřními odkazy
- Vytvoř Open Graph meta tagy (náhled webu pro Facebook a další sociální sítě)

## Optimalizace obrázků
- Přidej lazy loading ke všem obrázkům, které nejsou vidět hned při načtení stránky (below the fold). Tj. u hero sekce lazy loading nedělej.
- Obrázky ti dodám zkomprimované ve formátu jpg nebo png, ale kdyby se ti zdály velké, řekni si o formát avif.

## Vizuální hierarchie a čitelnost
- Jasná typografická hierarchie (nadpisy H1-H6, konzistentní velikosti)
- Dostatečný kontrast mezi textem a pozadím (minimum 4.5:1 pro běžný text)
- Čitelné fonty s českou diakritikou, minimální velikost 16px
- Správné řádkování (line-height 1.5-1.8 pro odstavce)
- Nikdy nezarovnávej text do bloku

## Layout
- Šířku celého webu dej na 85% obrazovky
- Jasné oddělení sekcí a obsahových celků
- Pokud mám v sekci 4 karty/boxy – dej je po dvou na řádek (ne 3+1)
- Vyvážené použití bílého prostoru (white space)
- Intuitivní navigace - logo vlevo, hamburger menu na mobilu pravo
- Funční hamburger menu pro šířku obrazovky takovou, kdy se už zalamují nebo těsnají položky menu
- Dej si záležet na patičce webu, ideálně tmavší akcent
- U prvku accordion (př. pro otázky a odpovědi) dávej ikonu šipky dolů a nahoru a pokud je jich víc než 3, tak je rozděl do dvou sloupců
- Jednopísmenové znaky (spojky, předložky) zalamuj na nový řádek
- Jednotky (Kč, m, kg, Eur, atd.) spoj s číslem nedělitelnou mezerou
- Datum piš ve formátu 1. 1. 2026 a mezery dej nedělitelné

## Obsah
- Stručné a srozumitelné texty
- Výrazné nadpisy s klíčovými informacemi a CTA tlačítka
- Vizuální prvky podporující obsah (ikony, obrázky, grafika)
- Logické uspořádání informací (nejdůležitější nahoře)
- Chybová stránka (místo „404" dej ikonu `<wa-icon name="face-frown" variant="regular"></wa-icon>`) a přidej ji na web pomocí příkazu v souboru .htaccess: `ErrorDocument 404 /404.html`
- Kontrola povinných údajů na webu: jméno, sídlo, IČ, zápis v rejstříku

## Konzistence
- Jednotný styl tlačítek, karet a komponent
- Stejný padding/margin napříč podobnými elementy
- Stejné zaoblení prvků
- Konzistentní ikonografie (používej font awesome, nebo uvedené ikony, ne emotikony)
- Stíny karet pouze velmi jemné
- Jednotný projev značky (brand voice)
- Konzistentní použití barev napříč celým webem
- Jednotný spacing a odsazení (používej jednotný systém, např. 8px grid)

## Barevná paleta
- Omezený počet barev (2-3 hlavní + neutrální)
- Primární barva pro CTA (call-to-action) tlačítka
- Neutrální jemné barvy pro pozadí
- Pro text #333333
- Brand barvy (HEX):
  - primární: `#FF7D23`
  - sekundární: `#7E8088`
  - tlačítka: jemný `linear-gradient(140deg, #FF7D23, #B34800)`
  - pozadí: `#F5F4F2`
  - text: `#333333`

## Fonty
- Font textu: Montserrat
- Font nadpisů: Bebas Neue / verzálky

## Struktura
Jednostránkový web

Položky menu:
- Služby
- Prodej
- Servis
- O nás
- Kontakt
- tlačítko: ikona telefonu a vytáčecí telefonní číslo: +420724860002

Do hlavičky vlevo nahoře přidej logo `Obrazky/logo-cyklosport.png`

## Další prvky na webu
Vlož Google mapu do sekce kontakt – adresu najdeš níže v instrukcích

## Design
Design hero sekce (celého webu) vytvoř podle vzoru, který ti dám před začátkem tvorby ve formátu jpg. Design laď do velmi jemných barev, které se hodí k tématu. Na zbytku webu používej moderní trendy webdesignu: jemný barevný gradient, glass efekt a jemné interaktivní prvky.

## Moderní design
- Layout: používej souměrný Bento grid
- Barvy: Jemné barevné gradienty, plynulé přechody
- Prvky: Zaoblené rohy (border-radius 16-24px), jemné stíny, 3D prvky
- Grafické prvky: Zařaď jemné grafické prvky
- Glass efekt: Skleněný efekt v pozadí karet (glassmorphism)
- Animace: Mikro interakce na hover, jemné scroll animace

## Obrázky
Na webu použij fotky (přílohy), které najdeš ve složce:
- `Obrazky/` – pro celý web (hero sekce atd.)

Odkazy na konkrétní obrázky najdeš v textu níže.

---

## Texty pro jednotlivé sekce
Na webu použij tyto texty pro jednotlivé sekce. Drž se jich doslova a nic neměň ani nepřidávej.

---

### POLOŽKY MENU (KOTVY)
- Služby
- Prodej
- Servis
- O nás
- Kontakt
- tlačítko: ikona telefonu a vytáčecí telefonní číslo: +420724860002

---

### HERO SEKCE
Obrázek: `Obrazky/hero-1.jpg`

**Cyklosport Popelka | Lutín u Olomouce**

Prodej a servis jízdních kol a elektrokol

Staráme se o vaše kola už 25 let. Přijďte si vybrat své nové kolo nebo se objednejte na servis.

Tlačítko: ikona telefonu a vytáčecí telefonní číslo: +420724860002

---

### SEKCE – SLUŽBY

**Ikona:** `Obrazky/ikona-kolo.svg`

**Jízdní kola a elektrokola**

Poradíme vám s výběrem vhodného kola pro vás i vaše děti, na výlet i do terénu. Nabízíme kola značek Author, Superior, CTM, Rock Machine, Pells a elektrokola Crussis.

---

**Ikona:** `Obrazky/ikona-servis.svg`

**Servis a přestavby jízdních kol**

Seřídíme, opravíme a připravíme vaše kolo na sezónu. Provádíme také montáž elektrosad a přestavby klasických kol na elektrokola. Na servis se vždy předem telefonicky objednejte.

---

**Ikona:** `Obrazky/ikona-helma.svg`

**Příslušenství a doplňky**

U nás nakoupíte přilby, zámky, brašny, cyklistické oblečení i mnoho dalšího včetně náhradních dílů. Zastupujeme značky Shimano, Mavic, Cratoni, SKS a další. Doplňky vám rádi na kolo i namontujeme.

---

### SEKCE – PRODEJ

**Kola pro každého**

Obrázek: `Obrazky/prodej-1.jpg`

Ať hledáte kolo do města, na výlety, do terénu nebo elektrokolo, pomůžeme vám najít to pravé. S výběrem vám poradíme osobně v naší prodejně v Lutíně u Olomouce.

Máme kola skladem, která si můžete ihned vyzkoušet a odvézt. A pokud nenajdete přesně to, co hledáte, kolo vám rádi objednáme přímo u výrobce.

Prodáváme značky, kterým důvěřujeme a za jejichž kvalitou si stojíme. Jsme oficiální Author Bike Centrum a Mavic Tech Dealer.

- Jízdní kola: Author, Pells, Superior, CTM, Rock Machine
- Elektrokola: Crussis

Loga značek a certifikací.

---

### SEKCE – FOTOGALERIE

Bez textu, jen galerie.

Použij obrázky:
- `Obrazky/prodej-2.jpg`
- `Obrazky/prodej-3.jpg`
- `Obrazky/prodej-4.jpg`
- `Obrazky/prodej-5.jpg`

---

### SEKCE – SERVIS

**Servis jízdních kol**

Postaráme se o vaše kolo od defektu až po kompletní přípravu na sezónu. Provádíme servis všech typů kol včetně elektrokol a umíme i přestavby klasických kol na elektropohon.

- Kompletní servis a seřízení kola
- Garanční prohlídky
- Výplet a napletení kol, centrování
- Repase odpružených vidlic
- Přestavby kol na elektrokola
- Montáž náhradních dílů a doplňků
- Nástřiky rámů
- Montáž elektrosad — středový motor 250 W a 750 W

Na servis se předem objednejte telefonicky.

Tlačítko: ikona telefonu a vytáčecí telefonní číslo: +420724860002

Obrázek: `Obrazky/servis.jpg`

---

### SEKCE – O NÁS

**O nás**

Obrázek: `Obrazky/o-nas.jpg`

Jsme rodinná prodejna s tradicí od roku 1999. Cyklosport Popelka jsme založili jako rodinný podnik a tradici poctivého přístupu ke kolům i zákazníkům v něm udržujeme dodnes. Za 25 let jsme se stali oblíbeným místem pro cyklisty z Lutína i širokého okolí Olomouce.

> „Baví mě, když zákazník přijde s konkrétní představou a my mu pomůžeme ji naplnit, nebo ji trošku poupravíme, protože víme, co mu bude opravdu sedět. Jsme malý obchod a to je naše výhoda. Každého zákazníka tady známe a na každé kolo si najdeme čas."
>
> Magda Popelková, provozovatelka Cyklosportu Popelka

Jsme držiteli certifikátu Férový přístup k zákazníkovi.

---

### SEKCE – KONTAKT

**Kontakt**

Přijďte si vybrat kolo nebo se objednejte na servis. Jsme tu pro vás.

Tlačítko: ikona telefonu a vytáčecí telefonní číslo: +420724860002

**Cyklosport Popelka**
U Parku 79
783 49 Lutín u Olomouce

**Otevírací doba:**
Pondělí, pátek: 9:00–12:00 a 13:00–16:00
Sobota, neděle: zavřeno

Parkování najdete na parkovišti u Billy, vzdáleném jen pár kroků.

[ mapa google maps ] adresa U Parku 79, 783 49 Lutín

---

### PATIČKA

Obrázek: `Obrazky/paticka.jpg` nebo `Obrazky/favicon-popelka-oranzova.png`, uvidíš, co bude vypadat líp.

**Cyklosport Popelka**
+420 724 860 002
popelka.sport@seznam.cz
FB: facebook.com/CyklosportPopelka

**Provozovna**
U Parku 79, 783 49 Lutín
Pondělí, pátek: 9.00–12.00 a 13.00–16.00
Sobota, neděle: zavřeno

**Provozovatel**
Jaroslav Popelka
IČO: 692 31 320 | DIČ: CZ6603231767
Fyzická osoba zapsaná v Živnostenském rejstříku

Copyright © 2026 Cyklosport Popelka. Všechna práva vyhrazena. Webdesign harmonickyweb.cz (funkční odkaz s proklikem na novou stránku, zvýraznění odkazu dle barev webu)
