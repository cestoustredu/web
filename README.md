# Cestou středu

Webové stránky pro celostní poradenství s využitím tradiční čínské medicíny, biorezonance a přírodních prostředků.

## 🌿 O webu

Tento web je postaven pomocí **Jekyll** a je určen pro hosting na **GitHub Pages** s vlastní doménou **www.cestoustredu.cz**.

## 📋 Obsah webu

- **Domů** - Úvodní stránka s představením
- **Certifikace** - Vzdělání a kvalifikace
- **Co nabízím** - Služby a průběh návštěvy
- **Biorezonance** - Diagnostické metody (Oberon, Plazma FQ, HRV, kvantová analýza)
- **Metody** - Mycoterapie, Joalis, Schüslerovy soli, Bachovy esence, byliny
- **Ceník** - Přehled služeb a storno podmínky
- **Kontakt** - Kontaktní údaje a ordinační hodiny
- **GDPR** - Ochrana osobních údajů

## 🚀 Rychlé spuštění

### Instalace

1. Nainstalujte Ruby a Jekyll (viz [DEPLOYMENT.md](DEPLOYMENT.md))
2. Nainstalujte závislosti:
   ```powershell
   bundle install
   ```

### Lokální spuštění

```powershell
bundle exec jekyll serve
```

Web bude dostupný na: http://localhost:4000

### Build pro produkci

```powershell
bundle exec jekyll build
```

Výstup bude v složce `_site/`

## 📝 Úpravy před spuštěním

### 1. Kontaktní údaje

Upravte v souboru `_config.yml`:

```yaml
email: "info@cestoustredu.cz"
phone: "+420 XXX XXX XXX"
address: "Vaše adresa"
city: "Praha"
```

### 2. Fotografie certifikátů

1. Vytvořte složku `assets/images/certificates/`
2. Nahrajte obrázky certifikátů
3. Upravte `certifikace.md` a nahraďte placeholders

### 3. Mapa

V `kontakt.md` vložte Google Maps iframe s vaší adresou.

### 4. Ordinační hodiny

Upravte v `kontakt.md` podle vašich reálných hodin.

### 5. Ceny

Aktualizujte ceny v `cenik.md` podle vašeho ceníku.

## 🎨 Design

Web má moderní, čistý design inspirovaný soulad.info:

- **Barvy:** Zelená (zdraví, příroda) + zlatohnědá (teplo, důvěra)
- **Typografie:** Segoe UI (text) + Georgia (nadpisy)
- **Responzivní:** Mobilní menu, flexibilní layout
- **Kontakty nahoře:** Telefon a email v horním pruhu

## 📁 Struktura projektu

```
c:\web\aja\
├── _layouts/           # Šablony stránek
│   ├── default.html    # Základní layout
│   ├── page.html       # Layout pro běžné stránky
│   └── service.html    # Layout pro služby
├── _includes/          # Znovupoužitelné komponenty
│   ├── header.html     # Hlavička s navigací
│   └── footer.html     # Patička
├── assets/             # Statické soubory
│   ├── css/
│   │   └── main.css    # Hlavní styly
│   └── js/
│       └── main.js     # JavaScript
├── _config.yml         # Konfigurace Jekyll
├── Gemfile             # Ruby dependencies
├── CNAME               # Doména pro GitHub Pages
├── index.md            # Úvodní stránka
├── certifikace.md      # Certifikace
├── sluzby.md           # Co nabízím
├── biorezonance.md     # Biorezonance
├── metody.md           # Metody
├── cenik.md            # Ceník
├── kontakt.md          # Kontakt
├── gdpr.md             # Ochrana osobních údajů
├── DEPLOYMENT.md       # Návod na nasazení
└── README.md           # Tento soubor
```

## 🌐 Deployment na GitHub Pages

Podrobný návod najdete v [DEPLOYMENT.md](DEPLOYMENT.md).

Stručně:

1. Vytvořte GitHub repozitář
2. Nahrajte soubory pomocí Git nebo GitHub Desktop
3. Zapněte GitHub Pages v nastavení
4. Nastavte DNS záznamy pro www.cestoustredu.cz
5. Přidejte custom domain v GitHub Pages

## 🔧 Technologie

- **Jekyll 4.3** - Generátor statických stránek
- **Minima theme** - Základní Jekyll téma (přizpůsobeno)
- **GitHub Pages** - Hosting
- **Markdown** - Psaní obsahu
- **Liquid** - Šablonovací jazyk
- **CSS3** - Moderní styly s CSS proměnnými
- **Vanilla JavaScript** - Bez závislostí na knihovnách

## 📱 Responzivní design

Web je plně responzivní s breakpointy:

- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: < 768px

## ✅ TODO před spuštěním

- [ ] Upravit kontaktní údaje
- [ ] Přidat fotografie certifikátů
- [ ] Vložit mapu
- [ ] Upravit ordinační hodiny
- [ ] Zkontrolovat ceny
- [ ] Otestovat lokálně
- [ ] Nahrát na GitHub
- [ ] Nastavit DNS
- [ ] Zapnout HTTPS

## 📄 Licence

Tento web je vytvořen na zakázku pro Cestou středu.

## 🆘 Podpora

Pro otázky a pomoc:

- Jekyll dokumentace: https://jekyllrb.com/docs/
- GitHub Pages: https://docs.github.com/pages
- Markdown guide: https://www.markdownguide.org/

---

Vytvořeno s ❤️ pro Cestou středu
