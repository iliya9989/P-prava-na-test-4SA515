# P-prava-na-test-4SA515
Níže najdeš detailní shrnutí klíčových konceptů užitečných pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů** na VŠE. Veškeré informace organizačního charakteru byly vynechány a rozpracovány byly pouze obsahově důležité části výuky.

---
# 1
## Klíčové koncepty předmětu 4SA515 - Řízení bezpečnosti informačních systémů:

### Systém řízení bezpečnosti informací (ISMS – Information Security Management System)
ISMS je strukturovaný rámec pravidel, postupů a procesů pro řízení informační bezpečnosti v organizaci. Cílem ISMS je chránit důvěrnost, integritu a dostupnost informací (CIA triáda).

- **Confidentiality (důvěrnost)** – přístup k informacím pouze pro autorizované osoby.
- **Integrity (integrita)** – informace jsou přesné, kompletní a neporušené.
- **Availability (dostupnost)** – informace jsou dostupné oprávněným uživatelům, kdykoliv je potřeba.

### Analýza a řízení rizik (Risk Management)
Analýza rizik představuje systematický proces identifikace, vyhodnocování a řízení rizik souvisejících s informační bezpečností.

Základní vzorec pro výpočet rizik:
\[
R = f(a, t, v)
\]

- **Asset (aktivum)** – jakákoli součást organizace, která má hodnotu a je třeba ji chránit (např. informace, software, hardware, zaměstnanci).
- **Threat (hrozba)** – potenciální příčina nežádoucího incidentu, která může poškodit aktivum.
- **Vulnerability (zranitelnost)** – slabina aktiva nebo opatření, která může být zneužita hrozbou.

Cílem je riziko efektivně identifikovat, kvantifikovat a následně minimalizovat implementací vhodných bezpečnostních opatření.

---

## Zdroje informací o řízení bezpečnosti (relevantní instituce):
- **ANSI** – American National Standards Institute
- **BSI** – British Standards Institute
- **ENISA** – European Network and Information Security Agency
- **ISO** – International Standards Organization (zejména standard ISO/IEC 27001 pro ISMS)
- **NIST** – National Institute of Standards and Technology (např. NIST Cybersecurity Framework)
- **ITU** – International Telecommunication Union
- **NÚKIB** – Národní úřad pro kybernetickou a informační bezpečnost (ČR)
- **CERT** – Computer Emergency Response Team (globálně Carnegie Mellon University a lokálně CERT CZ)

---

## Modelování aktiv
Model aktiv je souhrn všech zdrojů a komponent, které se podílejí na realizaci určité služby koncovému uživateli (SKU). Cílem modelu aktiv je jasně definovat závislosti mezi jednotlivými aktivy a technologickými komponentami v rámci ICT infrastruktury.

**Příklad struktury modelu aktiv:**

- Popis účelu aktiva (k čemu aktivum slouží).
- Výčet konkrétních technologií, aplikací a dat, která aktivum využívá.
- Grafická reprezentace závislostí mezi aktivy.

Příklad (z prezentace) – SKU „Řidiči – Operativa“:
- Slouží pro zadávání práce řidičům, operativní komunikaci, sledování zásilek a evidenci práce řidičů.
- Využívá aplikace Personalistika, Vozový park, Sklad, Obchod.
- SKU reprezentováno mobilní aplikací (tablet) s bezpečným připojením na aplikační server.

---

## Popis vzorové organizace 123-LOG, a.s. (pro potřeby cvičení):
Jedná se o fiktivní logistickou společnost poskytující skladovací a přepravní služby.

Struktura ICT zahrnuje:
- **Budova A (Serverovna):** Databázové servery (DS1, DS2), Mail server (MS1), Aplikační server (AS1), Web server (WS1), Firewall (FW1), File server (FS1), Switch/router (SW1).
- **Budova B:** Připojení přes VPN na FW1, používají se aplikace SKLAD, AUTA, ŘIDIČI.
- **Externí prostředí:** Přístup přes internet (HTTPS) k webovému serveru (WS1), data propagována přes AS1 z DS1 a DS2.

SKU (služby koncovému uživateli):
- Management (MGMNT)
- Účetnictví (ÚČTO)
- Personalistika (PERSON)
- Obchod (OBCHOD)
- Controlling (CONTROL)
- Sklad (SKLAD)
- Auta (AUTA)
- Řidiči (ŘIDIČI)
- Externí přepravci (EXT_PŘEP)
- Klienti (KLIENT)
- Řidiči v terénu (R_TER)
- Obchodník v terénu (O_TER)

### Příklad detailního popisu SKU „AUTA“ (zadaný v dokumentu):
- Slouží k evidenci a správě vozidel (evidence jízd, servisu, údržby apod.).
- Využívá tlustého klienta s přístupem na databázi DS2.

---

## Klíčové dovednosti pro zpracování modelu aktiv (zadání na cvičení):
1. Slovní popis účelu dané SKU.
2. Detailní popis aktiv podílejících se na realizaci SKU.
3. Grafická reprezentace modelu aktiv (diagram vztahů a závislostí mezi komponentami ICT infrastruktury).

---

## Otázky pro vlastní ověření znalostí:
1. Co znamená zkratka ISMS a jaký je její hlavní účel?
2. Vysvětli vzorec pro analýzu rizik R=f(a,t,v). Co jednotlivé parametry znamenají?
3. Jaké hlavní instituce jsou zdrojem informací pro řízení bezpečnosti informací?
4. Proč je důležité modelování aktiv v organizaci? Co by měl takový model zahrnovat?
5. Jak vypadá model aktiv v praxi (uveď příklad ze zadání cvičení)?

---

## Odpovědi na otázky pro vlastní ověření znalostí:
1. **ISMS** znamená Information Security Management System, hlavním účelem je řízení bezpečnosti informací v organizaci (zajištění důvěrnosti, integrity a dostupnosti informací).
2. **R=f(a,t,v)** znamená, že riziko (Risk – R) je funkcí aktiva (Asset – a), hrozby (Threat – t) a zranitelnosti (Vulnerability – v).
3. **Hlavní instituce:** ISO, NIST, ENISA, ANSI, BSI, ITU, NÚKIB, CERT.
4. **Modelování aktiv** je důležité k identifikaci všech zdrojů podílejících se na poskytování služeb ICT, včetně vzájemných závislostí, pro lepší řízení rizik a efektivnější ochranu informací. Model by měl obsahovat slovní popis, seznam technologií, aplikací a grafické znázornění vztahů.
5. **Příklad:** Aplikace AUTA – správa vozidel, tlustý klient s databází DS2.

Tento přehled pokrývá klíčová témata a koncepty, které jsou nezbytné k dobré přípravě na test z předmětu **4SA515 - Řízení bezpečnosti informačních systémů**.

# 2
Níže najdeš podrobný souhrn užitečný pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**, konkrétně ke kapitole **Hodnocení aktiv** (z dokumentu **C02-Hodnocení aktiv.pdf**) a doplňujícím informacím z dokumentu **RAMSES**.

---

## Hodnocení aktiv v ISMS (Information Security Management System)

Aktivem v ISMS může být cokoliv, co má hodnotu v rámci zpracování informací v organizaci. Aktivy mohou být fyzická zařízení, software, data, zaměstnanci, dokumentace, služby apod. Správné ohodnocení aktiv je klíčové pro určení závažnosti případných bezpečnostních incidentů a následně efektivní řízení rizik.

---

## Způsob hodnocení aktiv

Při hodnocení aktiv se zaměřujeme zejména na tři klíčové atributy informační bezpečnosti:

- **Dostupnost (Availability)**
- **Důvěrnost (Confidentiality)**
- **Integrita (Integrity)**

### 1. Hodnocení dostupnosti aktiv
Zaměřuje se na dopady nedostupnosti určitého aktiva. Je klíčové určit, jaké dopady by mělo, pokud aktivum nebude k dispozici po různé časové intervaly (např. 6 hodin, 1 den, 3 dny, týden apod.).

Postup při hodnocení dostupnosti aktiv:
- Identifikace scénářů nedostupnosti aktiva
- Posouzení dopadů na uživatele, organizaci a třetí strany
- Ověření dopadů uživatelem, nadřízeným a managementem

Výsledkem je tzv. **Business Impact Analysis (BIA)**, která definuje závažnost dopadů podle délky nedostupnosti.

Časové intervaly hodnocení dostupnosti (z příkladu cvičení):
- 6 hodin, 1 den, 3 dny, 1 týden, 2 týdny, 1 měsíc a déle.

### 2. Hodnocení důvěrnosti aktiv
Zkoumá dopady ztráty důvěrnosti, tedy situace, kdy jsou informace vyzrazeny neoprávněným osobám, konkurenci, nebo veřejnosti.

Postup hodnocení důvěrnosti:
- Identifikace scénářů ztráty důvěrnosti informací
- Určení dopadů pro uživatele, organizaci, konkurenci, třetí strany
- Ověření scénářů uživatelem, nadřízeným a managementem organizace

### 3. Hodnocení integrity aktiv
Zabývá se dopady v případě, kdy data nejsou korektní (jsou pozměněna, neúplná nebo chybně zaznamenaná).

Postup hodnocení integrity:
- Identifikace scénářů narušení integrity dat
- Posouzení dopadů na uživatele, organizaci a třetí strany
- Ověření scénářů uživatelem, nadřízeným a managementem organizace

---

## Metodika hodnocení dopadů podle RAMSES

RAMSES poskytuje jasná kritéria (vodítka), jak kvalitativní scénáře dopadů převést do číselné škály (1–10). Každá úroveň definuje míru dopadu podle několika dimenzí:

1. **Osobní bezpečnost**
2. **Ochrana osobních údajů**
3. **Povinnosti ze zákona**
4. **Trestní jednání**
5. **Veřejný pořádek**
6. **Ztráta důvěryhodnosti**
7. **Řízení a provoz organizace**
8. **Obchodní a ekonomické zájmy**
9. **Finanční ztráty / narušení činností**
10. **Mezinárodní vztahy**
11. **Obrana**
12. **Bezpečnostní a zpravodajské zájmy**

Každý scénář hodnocení dopadů je vyhodnocen na stupnici od 1 (malé narušení) do 10 (extrémní dopady, kritické pro organizaci nebo stát).

**Příklady stupnice RAMSES:**
- **Úroveň 1:** Drobné narušení emocí, žádné porušení zákona, finanční ztráta do 100 000 Kč.
- **Úroveň 5:** Závažné narušení činnosti organizace, finanční ztráta od 3 do 10 mil. Kč.
- **Úroveň 10:** Kritické poškození národního hospodářství, finanční ztráta nad 1 mld. Kč, ohrožení stability státu.

---

## Výstupy hodnocení aktiv dle zadání

Pro konkrétní SKU (služby koncovým uživatelům) je nutné vytvořit:

- **Dotazníky pro hodnocení dopadů:** 
  - Nedostupnosti
  - Ztráty důvěrnosti
  - Narušení integrity

- Dotazníky obsahují:
  - Reálné scénáře možných dopadů
  - Vyhodnocení scénářů podle vodítek RAMSES
  - Převod kvalitativního popisu dopadů na číselné hodnoty (relativní škála)

---

## Klíčové body shrnutí:
- Hodnota aktiva je určována závažností dopadu při narušení bezpečnosti (dostupnost, důvěrnost, integrita).
- Business Impact Analysis (BIA) určuje důležitost aktiva v čase jeho nedostupnosti.
- Metoda RAMSES poskytuje standardizovaná vodítka pro číselné vyjádření scénářů dopadů.
- Pro každé aktivum je nutné posoudit dopady individuálně a zapojit do hodnocení různé úrovně managementu.

---

## Otázky pro ověření znalostí:

1. Jaké jsou tři hlavní oblasti hodnocení aktiv?
2. Proč se provádí hodnocení dostupnosti aktiv a co je výsledkem tohoto hodnocení?
3. Jaká kritéria zahrnuje metoda RAMSES?
4. Jaký je rozdíl mezi kvalitativním a kvantitativním hodnocením dopadů?

---

## Odpovědi na otázky pro ověření znalostí:

1. Tři hlavní oblasti hodnocení aktiv jsou **dostupnost, důvěrnost a integrita**.
2. Hodnocení dostupnosti se provádí, aby bylo možné posoudit závažnost dopadů, pokud aktivum není k dispozici určitou dobu. Výsledkem je analýza dopadů (Business Impact Analysis – BIA).
3. Metoda RAMSES zahrnuje kritéria jako osobní bezpečnost, ochrana údajů, právní důsledky, ekonomické dopady, vliv na veřejný pořádek a další oblasti závažnosti dopadů.
4. **Kvalitativní hodnocení** využívá slovní popisy scénářů dopadů, zatímco **kvantitativní hodnocení** používá číselné hodnoty podle standardizované škály, např. RAMSES (1–10).

Tento detailní souhrn pokrývá základní koncepty potřebné pro pochopení hodnocení aktiv a jejich dopadů v ISMS, což je klíčové pro úspěšné zvládnutí testu z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

# 3
Níže najdeš detailní shrnutí konceptů důležitých pro test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**, konkrétně kapitoly **Rizika a jejich řízení** (z dokumentu **03-Rizika.pdf** a zadání **C03_Zadani.pdf**). Vše je doplněno o vysvětlení pojmů, postupů a metodických kroků potřebných ke správnému zvládnutí testu.

---

## Rizika a jejich řízení

Řízení rizik představuje proces, jehož cílem je identifikace, analýza, hodnocení a zvládání rizik souvisejících s provozem informačních systémů a bezpečností aktiv v organizaci.

### Základní rovnice rizika
Riziko se obecně vypočítává podle dvou základních rovnic:

**1. Rovnice s hrozbou a zranitelností:**
\[
R = f(a, t, v)
\]

- **a (asset)** – Hodnota aktiva
- **t (threat)** – Míra hrozby (pravděpodobnost realizace hrozby)
- **v (vulnerability)** – Míra zranitelnosti aktiva

**2. Rovnice s pravděpodobností:**
\[
R = f(a, p)
\]

- **p** – Pravděpodobnost úspěšnosti hrozby

Obě rovnice jsou zjednodušené modely, které umožňují kvantifikovat riziko pro konkrétní aktivum a situaci.

---

## Metodika CRAMM (CTTIA Risk Analysis and Management Method)
Pro účely cvičení předmětu je využívána metodika CRAMM, která umožňuje systematickou analýzu a řízení rizik v informačních systémech.

Metodika zahrnuje:
- **Identifikaci aktiv**
- **Hodnocení aktiv**
- **Identifikaci hrozeb a zranitelností**
- **Výpočet míry rizika**
- **Výběr a implementaci bezpečnostních opatření**

---

## Postup analýzy rizik dle zadání cvičení

### Krok 1 – Identifikace aktiv (z předchozího cvičení)
- Přenos již určených hodnot aktiv do tabulky (XLSX šablona).

### Krok 2 – Kvalifikovaný odhad hrozeb a zranitelností
- Odhad se provádí kvalitativně na stupnici 1 až 3:
  - **1 (Malá)**
  - **2 (Střední)**
  - **3 (Velká)**

- Hrozba a zranitelnost se stanovují na základě realistických scénářů a odhadu pravděpodobnosti jejich realizace.

### Krok 3 – Výpočet míry rizika
- Riziko se vypočítá kombinací hodnoty aktiva, hrozby a zranitelnosti podle rovnice uvedené výše.
- Výsledná míra rizika se použije ta nejvyšší a ta se následně propaguje na všechny komponenty modelu aktiv SKU.

---

## Návrh bezpečnostních opatření (ISO/IEC 27001)
Po určení míry rizika je nutné navrhnout vhodná bezpečnostní opatření, která budou eliminovat nebo snížit zjištěné riziko.

Opatření se dělí do kategorií:
- **O (organizační)**
- **T (technické)**
- **P (personální)**
- **F (fyzické)**

### Postup výběru opatření:
1. Výběr minimálně **2–3 opatření** pro každý prvek aktiv z normy ISO/IEC 27001 (nebo ISO 27002).
2. Opatření vybraná pro každé aktivum se uvedou v tabulce XLSX.
3. Označí se podle příslušného čísla z normy ISO 27001 (z „Příloha1.pdf“) a podle typu opatření (O, T, P, F).

---

## Kategorie bezpečnostních opatření dle ISO/IEC 27001 (z přílohy1)
Norma ISO/IEC 27001 poskytuje rámec bezpečnostních opatření členěných do skupin. Každá skupina obsahuje sadu specifických opatření, která organizace může implementovat k řízení informační bezpečnosti.

Příklad kategorií opatření (přehledově dle ISO 27001):
- **Řízení přístupu**
- **Fyzická bezpečnost a bezpečnost prostředí**
- **Bezpečnost lidských zdrojů**
- **Bezpečnost komunikace a provozu**
- **Správa aktiv**
- **Kryptografická opatření**
- **Bezpečnostní politika**
- **Řízení incidentů**
- **Soulad s legislativou a normami**

---

## Výstup cvičení – Riziková analýza v XLSX tabulce:
- Korektně vyplněná tabulka odpovídající SKU.
- Sloupce obsahují:
  - Hodnoty aktiv
  - Odhad hrozeb a zranitelností
  - Vypočtenou míru rizika
  - Navržená bezpečnostní opatření (označená číslem dle normy ISO a typem opatření).

---

## Kontrolní otázky pro ověření znalostí:
1. Jak zní základní rovnice rizika a co znamenají její jednotlivé složky?
2. Co je CRAMM a jaké kroky tato metodika zahrnuje?
3. Jaký je rozdíl mezi hrozbou a zranitelností?
4. Jaké jsou typy bezpečnostních opatření a jak jsou označovány?
5. Jak postupovat při výběru bezpečnostních opatření dle ISO/IEC 27001?

---

## Odpovědi na kontrolní otázky:
1. **Základní rovnice rizika:** R = f(a, t, v), kde aktivum (a), hrozba (t), zranitelnost (v). Alternativně R = f(a, p), kde p je pravděpodobnost úspěšnosti hrozby.
2. **CRAMM (CTTIA Risk Analysis and Management Method)** je metodika, která systematicky pokrývá identifikaci aktiv, hrozeb, zranitelností, výpočet rizik a řízení rizik skrze opatření.
3. **Hrozba** je potenciální příčina nežádoucího incidentu, zatímco **zranitelnost** je slabina aktiva, která může být zneužita touto hrozbou.
4. Typy opatření: **Organizační (O)**, **Technické (T)**, **Personální (P)**, **Fyzické (F)**.
5. Opatření se vybírají podle relevance k aktivům a určenému riziku, minimálně dvě až tři opatření pro každý prvek, označená číslem normy ISO a typem opatření (O, T, P, F).

Tento detailní přehled poskytuje jasnou orientaci v oblasti řízení rizik, což je klíčová součást znalostí pro zvládnutí předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

# 4
Níže nalezneš podrobný souhrn ke kapitole **„Priorita opatření“** z předmětu **4SA515 – Řízení bezpečnosti informačních systémů** podle nahraného dokumentu **„C04_Priorita opatření.pdf“** a doplňujících dokumentů z normy ISO/IEC 27002.

---

# Priorita bezpečnostních opatření

Proces prioritizace bezpečnostních opatření následuje po analýze rizik a je zaměřen na efektivní výběr opatření a jejich realizaci. Prioritizace opatření vychází z výše rizik, nákladů a časové náročnosti implementace, spolu s očekávanou účinností.

## Základní vzorec výpočtu rizika (zjednodušeno pro výuku):

Pro potřeby cvičení je riziko vypočteno podle vzorce:

\[
RISK = \frac{(\text{Aktivum} \times \text{Hrozba} \times \text{Zranitelnost})}{10} + 1
\]

V praxi však výpočet rizika většinou není lineární a často se používají expertní odhady (matice rizik).

---

## Hodnocení a prioritizace opatření

Pro efektivní snížení rizik je doporučeno použít kombinaci opatření různého charakteru (organizační, technická, personální a fyzická). Prioritizace implementace opatření se určuje podle následujících kritérií:

- **Míra rizika** (primární kritérium)
- **Cena implementace**
- **Čas implementace**
- **Interní/externí náklady** (vyjádřeno v člověkodnech)
- **Účinnost opatření** (odhadnutá na škále 1-malá, 2-střední, 3-vysoká)

### Vzorec pro stanovení priority opatření (použitý ve cvičení):

\[
P = \frac{1}{r \times \frac{c}{10\,000\,000} \times t \times \frac{d}{100}} \times u
\]

Kde:  
- **P** – priorita  
- **r** – riziko  
- **c** – cena implementace (Kč)  
- **t** – čas implementace (měsíce)  
- **d** – náklady implementace (člověkodny)  
- **u** – účinnost opatření  

Tento vzorec je jednoduchou konstrukcí pro výukové účely. Studenti mají za úkol jej analyzovat a případně navrhnout vylepšení.

---

## Obsah dokumentu „Plán zvládání rizik“

Dokument „Plán zvládání rizik“ je výsledkem procesu prioritizace opatření a obsahuje:

- Přehled konkrétních navržených opatření k eliminaci nejzávažnějších rizik.
- Parametry opatření (cena, čas a náklady implementace, účinnost).
- Výpočet priorit jednotlivých opatření.
- Management summary – shrnutí výsledků analýzy a doporučení pro vedení organizace.
- Časový harmonogram a grafický přehled nákladů plánovaných investic.

---

## Výběr bezpečnostních opatření podle ISO/IEC 27002

Opatření pro snížení rizik se vybírají z normy ISO/IEC 27002, která je obsáhlým standardem, popisujícím osvědčené postupy pro bezpečnost informací. Norma pokrývá oblasti jako:

- Politiky bezpečnosti informací  
- Organizace bezpečnosti  
- Bezpečnost lidských zdrojů  
- Řízení aktiv  
- Řízení přístupu  
- Kryptografie  
- Fyzická bezpečnost  
- Bezpečnost provozu  
- Bezpečnost komunikací  
- Akvizice, vývoj a údržba systémů  
- Řízení incidentů bezpečnosti informací  
- Soulad s požadavky a normami  

Konkrétní opatření musí odpovídat typu aktiva a charakteru rizika.

---

## Doporučené aspekty implementace opatření dle ISO 27002 (příklad opatření z normy):

- **Řízení přístupu** (kapitola 9 ISO/IEC 27002):
  - Řízení privilegovaných přístupových práv (např. omezení administrátorských účtů).
  - Přezkoumání a úprava přístupových práv zaměstnanců při změně pozice nebo ukončení pracovního poměru.
  - Správa hesel – požadavky na bezpečnou volbu a správu hesel.

- **Bezpečnost komunikací** (kapitola 13 ISO/IEC 27002):
  - Ochrana elektronické komunikace (šifrování citlivých informací).
  - Dohody o přenosu informací mezi organizací a externími stranami.
  - Dohody o mlčenlivosti a zachování důvěrnosti informací.

- **Vývoj a údržba systémů** (kapitola 14 ISO/IEC 27002):
  - Bezpečnostní požadavky ve všech fázích životního cyklu vývoje systému.
  - Bezpečné postupy vývoje softwaru a aplikací.
  - Řízení změn systémů (kontrola integrity a bezpečnosti při změnách).

---

## Kontrolní otázky pro ověření znalostí:

1. Jaká kritéria jsou využívána pro prioritizaci bezpečnostních opatření?
2. Co zahrnuje plán zvládání rizik?
3. Jaké hlavní oblasti pokrývá norma ISO/IEC 27002?
4. Vysvětli účel vzorce používaného ve cvičení pro výpočet priorit opatření.
5. Jaké typy opatření ISO/IEC 27002 doporučuje pro oblast řízení přístupu?

---

## Odpovědi na kontrolní otázky:

1. Kritéria pro prioritizaci opatření zahrnují míru rizika, cenu, čas implementace, náklady v člověkodnech a účinnost opatření.
2. Plán zvládání rizik zahrnuje výběr opatření, jejich parametry, výpočet priorit, management summary, harmonogram a plán investic.
3. Norma ISO/IEC 27002 pokrývá oblasti politik, organizace bezpečnosti, řízení přístupu, fyzické bezpečnosti, kryptografie, provozu a dalších klíčových aspektů informační bezpečnosti.
4. Vzorec výpočtu priorit opatření umožňuje určit relativní důležitost opatření podle jejich nákladů, účinnosti, času implementace a míry rizika.
5. Typy opatření doporučené pro řízení přístupu zahrnují omezení a řízení privilegovaných přístupů, přezkoumání práv uživatelů, bezpečnou správu hesel a řízení autentizace.

Tento souhrn detailně pokrývá veškeré koncepty nezbytné pro zvládnutí tématu prioritizace bezpečnostních opatření, což je důležitá součást přípravy na test předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

# 5
Níže najdeš podrobný souhrn užitečný pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**, konkrétně ke kapitole **„Zvládání rizik“** na základě dokumentu **„C05_Zvladani_rizik.pdf“**:

---

## Zvládání rizik (Risk Treatment)

Zvládání rizik je proces, který následuje po analýze a prioritizaci rizik. Je klíčovou fází ISMS (Information Security Management System) a zahrnuje rozhodnutí a implementaci opatření k omezení, přenosu, přijetí nebo vyhnutí se riziku.

### Základní strategie zvládání rizik

Existují čtyři základní přístupy ke zvládání rizik:

1. **Redukce rizika**
2. **Přenos rizika**
3. **Podstoupení (akceptace) rizika**
4. **Vyhnutí se riziku**

---

### 1. Redukce rizika
Redukce je nejčastější a často nejžádanější strategie. Cílem je snížit pravděpodobnost vzniku nebo dopad bezpečnostního incidentu.

**Redukce rizika zahrnuje např.:**
- Zdokonalování technických a organizačních opatření
- Zavedení účinných metod monitorování, obnovy a reakce
- Zvyšování povědomí zaměstnanců a informovanosti veřejnosti

**Typy ochrany při redukci rizik:**
- Náprava
- Vyloučení
- Prevence
- Minimalizace dopadu
- Odstrašování
- Odhalení
- Obnovení
- Monitorování
- Zvyšování povědomí

**Omezení při redukci rizik:**
- Časová, finanční, technická, provozní, kulturní, etická, ekologická, právní a osobní omezení.

---

### 2. Přenos rizika
Tento přístup neodstraňuje příčinu rizika, ale tlumí dopady. Typicky se jedná o pojištění, outsourcing či delegování odpovědnosti za určitá aktiva či procesy.

**Důležité body při přenosu rizik:**
- Vhodné pro případy, kdy opatření ke snížení rizik jsou ekonomicky nebo organizačně náročnější než náklady na přenos rizika.
- Přenos rizika je vhodný především pro situace, kde potenciální dopady nejsou pro organizaci fatální.

---

### 3. Podstoupení (akceptace) rizika
Organizace se rozhodne riziko akceptovat, ať už vědomě či nevědomě.

**Formy podstoupení rizika:**
- **Vědomá** – Organizace si riziko uvědomuje a rozhodne se ho akceptovat (např. nízká pravděpodobnost incidentu, nízké potenciální dopady).
- **Nevědomá** – Organizace o riziku neví nebo ho podceňuje.
- **Dobrovolná** / **Nedobrovolná** – Rozhodnutí vedení či přijetí situace bez jasného rozhodnutí.

---

### 4. Vyhnutí se riziku
Organizace se riziku zcela vyhne eliminací aktivit, které ho generují. Např. zrušení určitého projektu či neimplementace potenciálně rizikových technologií.

- Nevýhodou je ztráta potenciálních příležitostí („Kdo nehraje, nevyhraje“).

---

## Plán zvládání rizik (Risk Treatment Plan – RTP)

Jedná se o závěrečný dokument shrnující všechna opatření navržená na základě analýzy rizik.

**Struktura plánu zvládání rizik obsahuje:**
- Výčet navržených opatření (ISO 27002) včetně nákladů, časových rámců a detailního popisu zaměření na konkrétní rizika.
- Stanovení odpovědnosti za realizaci opatření.
- KPI (Key Performance Indicators) pro měření účinnosti po implementaci opatření.

---

## Postup při tvorbě RTP (dle zadání cvičení):

### Krok 1: Zjištění rizika aktiv
- Sloučení analýz rizik aktiv z předchozích kroků do jednotné tabulky pro celou organizaci (souhrn SKU).

### Krok 2: Zjištění priority opatření
- Výpočet priorit bezpečnostních opatření (včetně přehodnocení ceny, doby, člověkodnů a účinnosti opatření).
- Výpočet nových priorit opatření podle aktualizovaného vzorce.

### Krok 3: Finální zpráva o zvládání rizik (Risk Treatment Plan)
- Komplexní zpráva pro vedení organizace, shrnující celý průběh analýzy rizik a navržená bezpečnostní opatření.
- Jasně zdůvodňuje výběr opatření, priority, časový plán a náklady implementace.

---

## Shrnutí obsahu RTP:
- Přehled aktiv a jejich rizik
- Prioritizace bezpečnostních opatření (rozdělení opatření na vysokou, střední a nízkou prioritu)
- Časový harmonogram implementace
- Náklady implementace
- Odpovědnost za realizaci jednotlivých opatření
- Kritéria KPI pro vyhodnocování účinnosti

---

## Kontrolní otázky pro ověření znalostí:

1. Jaké existují hlavní strategie zvládání rizik?
2. Co znamená strategie přenosu rizika a kdy ji využíváme?
3. Jaké typy ochrany zahrnuje strategie redukce rizika?
4. Co by měl obsahovat kvalitní Risk Treatment Plan?
5. Vysvětlete, co znamená strategie vyhnutí se riziku a jaké jsou její výhody a nevýhody.

---

## Odpovědi na kontrolní otázky:

1. Hlavní strategie zvládání rizik jsou **Redukce, Přenos, Podstoupení (akceptace) a Vyhnutí se riziku**.
2. Přenos rizika znamená delegovat důsledky rizika na třetí stranu (např. pojištění, outsourcing). Využívá se, když je přenos levnější než opatření.
3. Redukce rizika zahrnuje ochranu typu nápravy, prevence, minimalizace dopadu, odhalení, obnovení, monitorování a další.
4. RTP obsahuje výčet opatření, náklady, lhůty, odpovědnosti za realizaci a KPI pro vyhodnocení účinnosti opatření.
5. Vyhnutí se riziku znamená úplnou eliminaci rizikové aktivity či technologie. Výhodou je nulové riziko, nevýhodou pak ztráta příležitostí.

Tento detailní přehled pokrývá základní koncepty potřebné pro pochopení a správnou aplikaci zvládání rizik v rámci ISMS, což je důležitá část přípravy na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

# 6
Níže nalezneš detailní shrnutí prezentace **„Cybersecurity Fundamentals I – Cíle, role a domény“** (z dokumentu CSX-1.pdf), které je užitečné pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

---

# Cybersecurity Fundamentals I – Cíle, role a domény

## 1. Úvod do Cybersecurity

Cybersecurity představuje ochranu informačních aktiv, jejichž cílem je zabránit působení hrozeb na informace, které jsou **zpracovávané, přenášené nebo ukládané** v prostředí informačních systémů.

### Základní atributy informační bezpečnosti (CIA triáda):

- **Důvěrnost (Confidentiality)** – přístup pouze autorizovaným osobám.
- **Integrita (Integrity)** – správnost a neporušenost informací.
- **Dostupnost (Availability)** – dostupnost informací v okamžiku, kdy je potřeba.

Další důležitý cíl:

- **Nepopiratelnost (Non-repudiation)** – důkaz, že zpráva byla skutečně odeslána deklarovaným odesílatelem (zejména v transakčních systémech).

---

## 2. Situační povědomí (Situational Awareness)

Profesionalita bezpečnostního manažera vyžaduje komplexní znalost širších souvislostí:

- Obchodních plánů, záměrů a prostředí organizace.
- Dostupných technologií.
- Bezpečnostních procesů a systémů.

---

## 3. Základní funkce Cybersecurity (NIST Cybersecurity Framework)

Dle NIST Framework existuje pět klíčových funkcí (doplněno o jednu další v prezentaci):

- **Identifikace** – Stav aktiv, identifikace hrozeb a rizik.
- **Ochrana** – Implementace opatření ke zmírnění rizik.
- **Detekce (Odhalení)** – Odhalení selhání či incidentů.
- **Reakce** – Akce a postupy v reakci na incident.
- **Obnovení** – Včasná oprava a obnovení provozu.
- **Poučení** – Zlepšení na základě zkušeností z incidentu.

---

## 4. Role v rámci Cybersecurity

### Governance

Klíčová role v oblasti strategického řízení bezpečnosti:

- Určení strategických směrů.
- Zajištění dosažení stanovených cílů.
- Zajištění odpovídajícího řízení rizik.
- Efektivní využití zdrojů organizace.

### Risk Management

- Identifikace, hodnocení a řízení rizik.

### Compliance

- Zajištění souladu s regulatorními požadavky, zákonnými normami a smluvními závazky.

### Typická hierarchie rolí v organizaci:

- **Top management (správní rada)** – strategická rozhodnutí.
- **Výkonný management (CEO)** – vytváří podmínky pro realizaci strategií.
- **Bezpečnostní manažer** – koordinace a dohled nad bezpečností.
- **Bezpečnostní administrátoři** – implementace bezpečnostních opatření v praxi.

---

## 5. Domény Cybersecurity

Pět hlavních domén kybernetické bezpečnosti zahrnuje komplexní oblasti, ve kterých je nutné aplikovat specifické znalosti a přístupy:

### Doména 1: Základní koncepty

- Risk management (řízení rizik).
- Typické vektory útoků a hrozby.
- Identifikace a klasifikace útoků.
- Bezpečnostní politiky a procesy.
- Bezpečnostní opatření.

### Doména 2: Bezpečnostní architektury

- Principy bezpečné architektury.
- Bezpečnostní rámce a standardy.
- Topologie sítí a bezpečnostní perimetry.
- Firewally, šifrování, izolace, segmentace.
- Monitoring, detekce a logování bezpečnostních událostí.

### Doména 3: Bezpečnost sítí, systémů, aplikací a dat

- Procesní opatření pro zajištění bezpečnosti.
- Hodnocení rizik, řízení zranitelností, penetrační testy.
- Best practices a efektivní řízení zranitelností.

### Doména 4: Incident Management (řízení incidentů)

- Kategorizace incidentů.
- Plány obnovy (DRP – Disaster Recovery Plan) a kontinuity podnikání (BCP – Business Continuity Plan).
- Incident Response (reakce na incidenty).
- Digitální forenzní analýza a připravenost na forenzní vyšetřování.

### Doména 5: Dopady vývoje technologií

- Mobilní zařízení (mobilní bezpečnost).
- Cloud Computing a cloudová úložiště.
- Efektivní spolupráce a komunikace mezi týmy.

---

## Otázky pro ověření znalostí:

1. Jaké jsou klíčové atributy informační bezpečnosti?
2. Jaké funkce definuje NIST Cybersecurity Framework?
3. Co znamená pojem „nepopiratelnost“ v kybernetické bezpečnosti?
4. Jaké hlavní oblasti pokrývá doména bezpečnostních architektur?
5. Co je hlavním cílem Governance v oblasti cybersecurity?

---

## Odpovědi na otázky pro ověření znalostí:

1. Klíčové atributy jsou **důvěrnost, integrita a dostupnost** (CIA triáda).
2. Funkce dle NIST framework: **Identifikace, Ochrana, Detekce, Reakce a Obnovení**.
3. Nepopiratelnost znamená, že **odesílatel nemůže popřít odeslání zprávy** – důležité v právních či transakčních systémech.
4. Doména bezpečnostních architektur pokrývá principy bezpečné architektury, bezpečnostní rámce, síťové topologie, firewally, izolace, segmentace, monitoring, detekci a logování.
5. Governance v cybersecurity má za cíl **určovat strategický směr, zajišťovat dosažení cílů, efektivně řídit rizika a efektivně využívat zdroje organizace**.

---

Toto shrnutí pokrývá klíčové body prezentace a je vhodným podkladem pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů**.

# 7
Zde jsou správné odpovědi na otázky uvedené v obrázcích a vysvětlení každé z nich:

---

### Question 1
**Three common controls used to protect the availability of information are:**  
✅ **a. Redundancy, backups, and access controls.**

**Vysvětlení:**  
- **Redundancy** (redundance): Snižuje dopady poruchy systému, zajistí dostupnost.
- **Backups** (zálohy): Umožňují obnovení informací při incidentu.
- **Access controls** (řízení přístupu): Brání neoprávněnému narušení, které by mohlo ovlivnit dostupnost.

---

### Question 2
**Governance has several goals, including (select all that apply):**  
✅ **a. Providing strategic direction.**  
✅ **b. Ensuring that objectives are achieved.**  
✅ **c. Verifying that organizational resources are being used appropriately.**  
✅ **d. Directing and monitoring security activities.**  
✅ **e. Ascertaining whether risk is being managed properly.**

**Vysvětlení:**  
Všechny uvedené body jsou správné a součástí cílů governance. Governance definuje strategii, zajistí dosažení cílů, správné využívání zdrojů, monitoruje bezpečnost a dohlíží na řízení rizik.

---

### Question 3
**According to the NIST framework, key functions necessary for the protection of digital assets are (choose three):**  
✅ **b. Protect**  
✅ **d. Recover**  
✅ **e. Identify**

**Vysvětlení:**  
Klíčové funkce NIST Cybersecurity Framework jsou:  
- **Identify** – identifikace aktiv a rizik  
- **Protect** – ochrana aktiv  
- **Detect** – detekce incidentů  
- **Respond** – reakce na incidenty  
- **Recover** – obnova po incidentu

Možnosti „Encrypt“ a „Investigate“ nejsou součástí klíčových funkcí dle NIST frameworku.

---

### Question 4
**Which of the following is the best definition for cybersecurity?**  
✅ **d. Protecting information assets by addressing threats to information that is processed, stored or transported by internetworked information systems.**

**Vysvětlení:**  
Cybersecurity se zaměřuje specificky na ochranu digitálních aktiv a systémů, které zpracovávají, ukládají nebo přenášejí informace prostřednictvím sítí.

---

### Question 5
**Which of the following cybersecurity roles is charged with the duty of managing incidents and remediation?**  
✅ **c. Security management**

**Vysvětlení:**  
Bezpečnostní management má zodpovědnost za správu incidentů, reakce na ně a nápravná opatření. Tento úkol je na provozní úrovni a spadá přímo pod roli bezpečnostního managementu.

---

Toto shrnutí odpovědí pokrývá důležité koncepty a souvislosti nezbytné pro správné pochopení a přípravu na test z oblasti cybersecurity dle předmětu 4SA515 – Řízení bezpečnosti informačních systémů.
