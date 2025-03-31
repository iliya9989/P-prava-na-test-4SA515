# P-prava-na-test-4SA515
Níže najdeš detailní shrnutí klíčových konceptů užitečných pro přípravu na test z předmětu **4SA515 – Řízení bezpečnosti informačních systémů** na VŠE. Veškeré informace organizačního charakteru byly vynechány a rozpracovány byly pouze obsahově důležité části výuky.

---

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
