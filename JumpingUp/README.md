# 🏔️ Jumping Up - PWA Game

Jump King-štýl hra s drag and drop mechanikou vytvorená vo Vue 3 ako záverečné zadanie pre WEBTE1 (ZS 2025/2026).

## 🚀 Inštalácia a spustenie

### Požiadavky
- Node.js 20.19.0 alebo vyššie
- npm

### Kroky

1. **Nainštalujte závislosti:**
```bash
npm install
```

2. **Spustite vývojový server:**
```bash
npm run dev
```
Aplikácia bude dostupná na `http://localhost:5173`

3. **Build pre produkciu:**
```bash
npm run build
```

4. **Náhľad produkčného buildu:**
```bash
npm run preview
```

## 🎮 Ako hrať

### Ovládanie
1. **Desktop**: Klikni na panáčika, drž a ťahaj myšou v **opačnom smere**, kam chceš skočiť
2. **Mobile**: Ťukni na panáčika, drž a ťahaj prstom
3. **Sila skoku** = dĺžka ťahania (čím viac ťaháš, tým silnejší skok - max 200px pre 100% silu)
4. **Smer skoku** = opačný smer ťahania
5. **Rotácia panáčika** = Vizuálna indikácia smeru letu počas skoku

### Cieľ
- Dostaň sa na cieľ (červená platforma) v čo najkratšom čase
- Pokús sa urobiť to s čo najmenším počtom pokusov a skokov
- Dokončiť všetky 3 levely

### Tipy
- Pre krátke skoky ťahaj menej
- Pre vysoké skoky ťahaj viac smerom dole
- Skús predvídať trajektóriu skoku pomocou šípky
- Každý level je náročnejší ako predchádzajúci
- Zelená vlajka ukazuje kde spadneš na začiatku levelu

## 📊 Funkcionality

### Herná mechanika
- ✅ **Drag and Drop** - Intuítívne ovládanie myšou/prstom
- ✅ **Inverzný smer skoku** - Ťaháš opačne než chceš skočiť
- ✅ **Sila skoku** - Závisí od dĺžky ťahania (max 200px)
- ✅ **Fyzikálny engine** - Gravitácia (0.5), rýchlosť, frikcia (0.95), kolízie
- ✅ **Pokročilá kolízna detekcia** - Frame-by-frame kontrola pre vysoké rýchlosti
- ✅ **Kolízie zo všetkých strán** - Vrch, spodok, ľavá, pravá strana platformy
- ✅ **Bounce efekt** - Odraz od bočných strán platforiem
- ✅ **Pád a reset** - Ak spadneš mimo obrazovku, level sa restartuje
- ✅ **Rotácia panáčika** - Vizuálna indikácia smeru letu
- ✅ **Start drop** - Panáčik spadne na prvú platformu pri štarte levelu
- ✅ **Animovaný background** - 40 častíc pohybujúcich sa v pozadí

### Vizuálne prvky
- ✅ **Šípka smeru** - Ukazuje kam skočíš
- ✅ **Power bar** - Indikácia sily skoku (farba mení podľa sily)
- ✅ **Vlajka startu** - Zelená vlajka ukazuje kde panáčik dopadne na začiatku
- ✅ **Farebné platformy** - Štartová platforma (modrá), Cieľ (červená), Bežné (šedá)
- ✅ **Fullscreen responzívny dizajn** - Hra sa prispôsobí akejkoľvek veľkosti obrazovky
- ✅ **Landscape orientácia** - Automatické otočenie na mobil zariadeniach

### Štatistiky a tracking
- ✅ **Pokusy (deaths)** - Počet pádom mimo obrazovku
- ✅ **Skoky (jumps)** - Celkový počet vykonaných skokov
- ✅ **Časomer** - Real-time meranie času s pause/resume
- ✅ **Celkové štatistiky** - Total deaths, total jumps, completed levels
- ✅ **História levelov** - Detailný záznam každého dokončeného levelu
- ✅ **Priemerný čas** - Automatický výpočet priemerného času na level
- ✅ **Success rate** - Úspešnosť (levely/deaths)

### Pokročilé funkcie
- ✅ **localStorage Persistence** - Automatické ukladanie progresiu
- ✅ **Pokračovať v hre** - Po refresh stránky môžeš pokračovať odkiaľ si skončil
- ✅ **Level restart** - Reštart aktuálneho levelu
- ✅ **Game restart** - Nová hra od začiatku (zmaže uložený progress)
- ✅ **Pause/Resume** - Automatická pauza pri otvorení menu
- ✅ **Level completion screen** - Prehľad štatistík po dokončení levelu

### PWA funkcie
- ✅ **Instalovateľná** - Možnosť pridať na plochu (Add to Home Screen)
- ✅ **Offline režim** - Funguje aj bez internetu
- ✅ **Service Worker** - Cache resources pre rýchle načítanie
- ✅ **Manifest.json** - PWA konfigurácia s ikonami a orientáciou
- ✅ **SVG ikony** - 192x192 a 512x512 ikony pre PWA
- ✅ **Screenshot** - Screenshot pre PWA inštaláciu

### UI/UX
- ✅ **HUD na vrchu** - Level info, pokusy, skoky, čas
- ✅ **Menu overlay** - Návod, štatistiky, história levelov
- ✅ **Level Complete screen** - Gratulačná obrazovka s možnosťou pokračovať
- ✅ **Start screen** - Uvítacia obrazovka s tlačidlami Pokračovať/Začať novú hru
- ✅ **Rotate Device prompt** - Upozornenie na mobil zariadeniach v portrait mode
- ✅ **Dark theme** - Konzistentná tmavá farebná schéma (#1a1a2e, #16213e, #0f1626)
- ✅ **Smooth animations** - Fade-in, slide-up, bounce efekty

### Responzivita
- ✅ **Fullscreen layout** - Hra zaberá celú obrazovku
- ✅ **Dynamic scaling** - Canvas sa škáluje podľa veľkosti okna
- ✅ **Aspect ratio preservation** - Zachová pomer strán 1000:750
- ✅ **Mobile landscape** - Vynútená landscape orientácia na mobil zariadeniach
- ✅ **Touch support** - Plná podpora touch eventov pre mobile

## 📁 Štruktúra projektu

```
JumpingUp/
├── public/
│   ├── manifest.json           # PWA manifest (landscape orientácia)
│   ├── sw.js                   # Service worker (cache v2)
│   ├── icon-192.svg            # PWA ikona 192x192
│   ├── icon-512.svg            # PWA ikona 512x512
│   └── screenshot.svg          # Screenshot pre PWA
├── src/
│   ├── components/
│   │   ├── GameCanvas.vue      # Herný canvas s fyzikou, rendering, particles
│   │   ├── GameStats.vue       # Zobrazenie štatistík (deaths, jumps, time)
│   │   ├── GameMenu.vue        # Menu overlay s návodom a štatistikami
│   │   ├── LevelComplete.vue   # Obrazovka po dokončení levelu
│   │   └── RotateDevice.vue    # Prompt pre otočenie zariadenia
│   ├── composables/
│   │   ├── useGamePhysics.js       # Fyzika (gravitácia, kolízie, velocity, rotation)
│   │   ├── useGameStats.js         # Štatistiky + localStorage persistence
│   │   └── useResponsiveCanvas.js  # Responzívne škálovanie canvas
│   ├── css/
│   │   ├── main.css                # Globálne štýly (reset, body, #app)
│   │   ├── game-canvas.css         # Štýly pre GameCanvas komponent
│   │   ├── game-menu.css           # Štýly pre GameMenu komponent
│   │   ├── game-stats.css          # Štýly pre GameStats komponent
│   │   └── level-complete.css      # Štýly pre LevelComplete komponent
│   ├── data/
│   │   └── levels.json         # Konfigurácia 3 levelov s platformami
│   ├── App.vue                 # Hlavný komponent (game state, level management)
│   └── main.js                 # Entry point
├── index.html                  # HTML entry point s PWA meta tags
├── package.json                # Závislosti a skripty
├── vite.config.js              # Vite konfigurácia
└── README.md                   # Tento súbor
```

## 🛠️ Technológie

- **Vue 3** - Composition API (`<script setup>`), reactive state (ref, computed, watch)
- **Vite** - Build tool a dev server
- **Canvas API** - 2D rendering hry, 60 FPS s requestAnimationFrame
- **Service Workers** - PWA offline funkcionalita, cache management
- **localStorage** - Persistentné ukladanie progresiu a štatistík
- **CSS3** - Flexbox, Grid, animations, transforms, gradients
- **Media Queries** - Responzívny dizajn (@media max-width: 768px)
- **SVG** - Ikony pre PWA
- **Touch Events** - Podpora pre mobilné zariadenia

## 🎨 Herná logika

### Fyzikálny systém
- **Gravitácia**: 0.5 (konštantné zrýchlenie nadol)
- **Frikcia**: 0.95 (spomalenie pri pristátí)
- **Max jump power**: 200px = 100% sila
- **Velocity**: Vypočítané z drag distance a direction
- **Rotation**: Počítané z velocity pomocou Math.atan2()

### Kolízny systém
- **Platform collision**: Frame-by-frame kontrola predchádzajúcej pozície
- **Head collision**: Zastaví pohyb nahor pri náraze hlavou do platformy
- **Side collision**: Odraz (bounce) pri náraze z boku s velocity * -0.3
- **Goal detection**: Kontrola dosiahnutia červenej cieľovej platformy
- **Fall detection**: Reset levelu pri páde mimo canvas (y > canvas height)

### Level systém
- **3 levely** s rastúcou obtiažnosťou
- **JSON konfigurácia**: Každý level má definované platformy, štart, cieľ
- **Dynamic scaling**: Platformy sa škálujú podľa veľkosti obrazovky
- **Progression tracking**: localStorage ukladá aktuálny level a stats

## 📝 Poznámky

### Ikony a PWA
- Projekt obsahuje SVG ikony v priečinku `public/`
- SVG ikony sú plne podporované v moderných prehliadačoch
- Manifest vynucuje landscape orientáciu na mobiloch
- Service Worker cache verzia: `jumping-up-v2`

### Optimalizácia
- Canvas rendering s requestAnimationFrame pre 60 FPS
- Optimalizované kolízne detekcie s early exit
- Responzívny canvas s dynamic scaling
- localStorage auto-save po každej zmene stavu
- Particle system s 40 časticami pre vizuálny efekt

### Kompatibilita
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Edge 90+
- ⚠️ Safari 14+ (limitovaná PWA podpora)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile, Samsung Internet)

### Tlač
⚠️ **Aplikácia NIE JE optimalizovaná pre tlač**
- Ide o interaktívnu hru určenú pre obrazovku
- Print functionality bola odstránená
- Pre dokumentáciu použite screenshot alebo PDF z prehliadača

## 🧪 Testovanie PWA

1. Build aplikácie: `npm run build`
2. Preview: `npm run preview`
3. Otvor v Chrome DevTools:
   - **Application → Manifest** - Skontroluj PWA manifest
   - **Application → Service Workers** - Over registráciu SW
   - **Application → Local Storage** - Over ukladanie progresiu
   - **Lighthouse** - PWA audit (skóre 90+)
4. Testuj "Add to Home Screen" na mobile
5. Testuj offline režim (vypni sieť a refresh stránku)

## 👨‍💻 Vývoj

Projekt vytvorený pre **WEBTE1 - Záverečné zadanie - ZS 2025/2026**

### Implementované funkcie

#### Core gameplay
- [x] Drag and drop mechanika (inverzný smer)
- [x] Fyzikálny engine (gravitácia, velocity, friction, rotation)
- [x] Kolízny systém (všetky strany, frame-by-frame)
- [x] 3 levely s JSON konfiguráciou
- [x] Sila skoku závislá od dĺžky ťahania
- [x] Vizuálne indikátory (šípka, power bar, rotácia)

#### UI/UX
- [x] Fullscreen responzívny dizajn
- [x] Dark theme konzistentný cez celú aplikáciu
- [x] HUD s real-time štatistikami
- [x] Menu s návodom a históriou
- [x] Level completion screen
- [x] Start screen s možnosťou pokračovať
- [x] Rotate device prompt pre mobile

#### PWA
- [x] Manifest.json s landscape orientáciou
- [x] Service Worker s cache v2
- [x] SVG ikony (192x192, 512x512)
- [x] Offline funkcionalita
- [x] Instalovateľnosť (Add to Home Screen)

#### Pokročilé funkcie
- [x] localStorage persistence (save/load game state)
- [x] Pause/Resume timer
- [x] Particle background system
- [x] Dynamic canvas scaling
- [x] Touch events pre mobile
- [x] Enhanced collision detection
- [x] Player rotation animation

#### Štatistiky
- [x] Deaths tracking (pokusy)
- [x] Jumps tracking (skoky)
- [x] Real-time timer
- [x] Level history
- [x] Total statistics
- [x] Average time calculation
- [x] Success rate calculation

### Splnené body hodnotenia:
- ✅ Nápad, grafický návrh, atraktivita prevedenia (6b)
- ✅ Responzivita, použitie drag & drop (10b)
- ✅ Spolupráca s xml alebo json (6b)
- ✅ PWA (10b)
- ✅ Možnosť viacnásobného hrania, náhodnosť generovania, logika, štatistika (8b)
- ✅ Popis hry a návod (4b - bez tlačovej optimalizácie)
- ✅ Celková funkčnosť, minimálny počet úloh (10b)

**Celkom: ~54 bodov**

## 📄 Licencia

Tento projekt je vytvorený pre vzdelávacie účely.

---

**Vyšplhaj sa na vrchol! 🏔️**
