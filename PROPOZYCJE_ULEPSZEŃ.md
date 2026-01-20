# Propozycje ulepszeń dokumentacji

## 1. Pliki wymagające standaryzacji

### NPCs do poprawienia
Następujące pliki NPC nie zostały jeszcze dostosowane do standardu:
- `NPCs/CohorsObscura.md` - wymaga struktury jak w OliverSchreiber.md
- `NPCs/HandlarzeGildiiGórniczej.md` - wymaga struktury jak w OliverSchreiber.md
- `NPCs/WolniHandlarze.md` - wymaga struktury jak w OliverSchreiber.md

### Brakujące NPCs
Warto utworzyć pliki dla postaci wspomnianych w dokumentacji:
- `NPCs/LordEjdolon.md` - Lord Komandor, kluczowa postać w Akcie 1
- `NPCs/LiraThornheart.md` - dowódca Zakonu Białej Róży w Tylnym Wejściu
- `NPCs/KapitanSolokrusz.md` - kapitan korsarzy wspomniany w Korsarze.md
- `NPCs/KapitanHelios.md` - dowódca Cohors Helios (informacja tylko dla MG)

## 2. Brakujące pliki pomocnicze

### Quick Reference dla MG
Stwórz `AKT_1/QuickReference.md`:
- Lista kluczowych NPCs w Wielkiej Bibliotece
- Mapa połączeń między lokacjami
- Timeline wydarzeń (dzień po dniu)
- Ważne dowody i ślady w każdej lokacji

### Encounter Tables
Stwórz `AKT_1/TabelePotworów.md`:
- Tabele losowych spotkań dla każdej lokacji
- Poziomy trudności
- Typowe łupy

### Session Prep
Stwórz `AKT_1/PrzygotowanieDoSesji.md`:
- Checklist przed sesją
- Kluczowe punkty fabularne do przekazania
- Możliwe rozgałęzienia
- Backup plans jeśli gracze pójdą w nieoczekiwanym kierunku

## 3. Pliki indeksujące (Hub Files)

### Index NPCs
Stwórz `NPCs/INDEX.md`:
```markdown
# Index Postaci

## Wielka Biblioteka
- [[OliverSchreiber]] - Handlarz i kartograf
- [[Hera|Siostra Hera]] - Zakon Czerwonej Róży (charytatywna fasada)
- [[Dornan|Brat Dornan]] - Zakon Czerwonej Róży (strażnik)
- [[Niru|Pucybut Niru]] - Pracownik Gildii Górniczej
- [[Skial]] - Agent Cohors Liber (TAJNE)
- [[Ishara]] - Gildia Eksploracyjna
- [[Korsarze|Grupa korsarzy]] - Kapitan Solokrusz

## Frakcje
- [[CohorsObscura]] - Nefilim (TAJNE)

## Do utworzenia
- Lord Komandor Ejdolon
- Lira Thornheart
- Kapitan Solokrusz
- Kapitan Helios
```

### Index Lokacji
Stwórz `Lokacje/INDEX.md`:
```markdown
# Index Lokacji

## Powierzchnia
- [[WielkaBiblioteka]] - Główny hub handlowy
- [[MiasteczkoNadBiblioteką]] - Osada na powierzchni
- [[TylneWejście]] - Tajne wejście (Zakon Białej Róży)

## Poziom 1 - Płytkie Jaskinie
- [[Korytarze]] - Główne arterie
- [[Katakumby]] - Nekropolis/mieszkania
- [[ZalaneJaskinie]] - Labirynt krasowy
- [[Rotunda]] - Węzeł śledczy (ślady Nefilim)
- [[Katedra]] - Scena bitwy (AKT 1)
```

## 4. Metadata i Properties

Dodaj YAML frontmatter do wszystkich plików dla lepszej organizacji w Obsidian:

### Przykład dla NPC:
```yaml
---
typ: NPC
frakcja: "Zakon Czerwonej Róży"
lokacja: "Wielka Biblioteka"
poziom: 10
alignment: Neutral
status: alive
---
```

### Przykład dla Lokacji:
```yaml
---
typ: Lokacja
poziom: 1
niebezpieczeństwo: średnie
przeszukana: częściowo
powiązania: ["Katedra", "Katakumby", "Korytarze"]
---
```

### Przykład dla Frakcji:
```yaml
---
typ: Frakcja
wpływy: wysoki
zasoby: bardzo_wysokie
alignment: lawful_evil
---
```

## 5. Timeline i Chronologia

Stwórz `AKT_1/Timeline.md`:
```markdown
# Timeline Aktu 1

## Dzień -5 (5 dni przed początkiem kampanii)
- Cohors Helios przybywa przez Tylne Wejście (teleporter)
- Rozpoczynają rekonesans kompleksu

## Dzień -3
- Cohors Helios mapuje trasę do Katedry
- Przygotowują zasadzkę

## Dzień -1
- Ekspedycja Zakonu Czerwonej Róży wchodzi do kompleksu
- Walka z potworami i eksploatacja tuneli

## Dzień 0 - RANO (incydent)
- Bitwa w Katedrze między Cohors Helios a ekspedycją Czeru
- Cohors Helios wycofuje się przez Rotundę i Tylne Wejście
- "Golemy ucieczkowe" (Nefilim w pancerzach) pojawiają się w Wielkiej Bibliotece
- Panika w Miasteczku

## Dzień 0 - POPOŁUDNIE
- Przemówienie Lorda Komandora Ejdolona
- Ogłoszenie nagrody
- Pierwsi poszukiwacze ruszają do tuneli

## Dzień 1 - KAMPANIA ZACZYNA SIĘ
- Gracze otrzymują informacje o nagrodzie
- Rozpoczynają śledztwo
```

## 6. Mapa połączeń

Stwórz `AKT_1/MapaPołączeń.md`:
```markdown
# Mapa połączeń - Akt 1

## Wielka Biblioteka
↓ główne wejście
**Korytarze**
├→ Katakumby
├→ Zalane Jaskinie
└→ Rotunda
    ├→ Katakumby (tylne wejście)
    ├→ Katedra
    └→ Tylne Wejście (do powierzchni)

## Tylne Wejście
↑ grota na powierzchni
↓ tunel
Rotunda
```

## 7. Sekrety i Informacje MG

Stwórz `AKT_1/SekretnyMG.md`:
```markdown
# Sekrety MG - Akt 1

## Prawda o "golemach ucieczkowych"
- To byli Nefilim w ciężkich pancerzach bojowych
- Teleportowali się, stąd grom i błyskawica
- Ślady w Rotundzie prowadzą DO kompleksu, nie NA ZEWNĄTRZ

## Cohors Helios
- Dowódca: Kapitan Helios
- 6-8 żołnierzy w pancerzach
- Jeden ciężko ranny (mag najemny)
- Wycofali się z łupami z bitwy

## Przetrwali z ekspedycji Czeru
- Dwójka rycerzy + czarodziejka
- Uciekli w tunelach
- Możliwe lokacje: Zalane Jaskinie lub głębiej w kompleksie

## Frakcje śledcze
- **Cohors Obscura** - ma mapę od Cohors Helios, szybko dotrą do Katedry
- **Skial (Cohors Liber)** - obserwuje w Wielkiej Bibliotece
- **Zakon Białej Róży** - bada Tylne Wejście, szczerze szuka prawdy
- **Lord Ejdolon** - zna prawdę? Ukrywa? Motywacje niejasne
```

## 8. Checklista przygotowania sesji

Stwórz `AKT_1/ChecklistaSesji.md`:
```markdown
# Checklist przygotowania sesji - Akt 1

## Przed pierwszą sesją
- [ ] Przeczytaj AKT_1/Wprowadzenie.md
- [ ] Przeczytaj NPCs w Wielkiej Bibliotece
- [ ] Przeczytaj Lokacje/Katedra.md i Lokacje/Rotunda.md
- [ ] Przygotuj mapę Wielkiej Biblioteki
- [ ] Przygotuj tabele potworów dla Katakumb i Korytarzy
- [ ] Zdecyduj timeline - ile dni po incydencie gracze zaczynają?

## Przed każdą sesją
- [ ] Review notatek z poprzedniej sesji
- [ ] Update timeline (który dzień?)
- [ ] Przeczytaj lokacje, gdzie gracze mogą dotrzeć
- [ ] Przygotuj 2-3 losowe spotkania
- [ ] Sprawdź status konkurencyjnych grup (Oliver, Ishara, Cohors Obscura)

## Po każdej sesji
- [ ] Zapisz gdzie gracze skończyli
- [ ] Zanotuj co odkryli (ślady, dowody, NPCs)
- [ ] Update timeline
- [ ] Zaplanuj reakcje innych frakcji na działania graczy
```

## 9. Kluczowe poprawki w istniejących plikach

### CLAUDE.md - dodaj sekcję
```markdown
## Session Preparation Files
- `AKT_X/QuickReference.md` - szybki przegląd kluczowych informacji
- `AKT_X/Timeline.md` - chronologia wydarzeń
- `AKT_X/SekretnyMG.md` - informacje tylko dla MG
- `AKT_X/ChecklistaSesji.md` - przygotowanie do sesji
```

### Dodaj tags do wszystkich plików
W każdym pliku dodaj na końcu:
```markdown
---
Tags: #akt1 #lokacja #npc #frakcja (odpowiednio)
```

## 10. Przyszłe akty

Stwórz strukturę dla kolejnych aktów:
```
AKT_2/
├── Wprowadzenie.md
├── QuickReference.md
├── Timeline.md
├── SekretnyMG.md
└── ChecklistaSesji.md

AKT_3/
└── ...
```

## 11. Grafika i mapy

Rozważ dodanie:
- `Mapy/WielkaBiblioteka.png` - mapa dla graczy
- `Mapy/PoziomPierwszy.png` - ogólna mapa poziomu 1
- `Mapy/Katedra_MG.png` - mapa dla MG z zaznaczonymi śladami
- `Portrety/` - folder na portrety NPCs

## 12. Glossary

Stwórz `GLOSSARIUM.md`:
```markdown
# Glossarium

## Technologia pyłowa
Technologia oparta na magicznym pyle...

## Cohors (łac.)
Oddział, formacja wojskowa. Używana przez Nefilim...

## Czeru
Potoczna nazwa rycerzy Zakonu Czerwonej Róży...

## Perły magiczne
Źródła zasilania dla mechanicznych istot...
```

---

## Priorytet implementacji

### Wysoki priorytet (przed następną sesją)
1. Popraw NPCs: CohorsObscura, HandlarzeGildiiGórniczej, WolniHandlarze
2. Stwórz AKT_1/QuickReference.md
3. Stwórz AKT_1/Timeline.md
4. Stwórz AKT_1/SekretnyMG.md

### Średni priorytet
5. Stwórz Index pliki (NPCs/INDEX.md, Lokacje/INDEX.md)
6. Stwórz AKT_1/ChecklistaSesji.md
7. Dodaj NPCs: LordEjdolon, LiraThornheart, KapitanHelios

### Niski priorytet (długoterminowo)
8. Dodaj YAML frontmatter do wszystkich plików
9. Stwórz GLOSSARIUM.md
10. Przygotuj strukturę AKT_2
11. Dodaj grafiki i mapy
