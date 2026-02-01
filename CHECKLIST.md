# RYCHLÁ KONTROLA PŘED SPUŠTĚNÍM

## 1. POVINNÉ ÚPRAVY

### Soubor: _config.yml
```yaml
email: "info@cestoustredu.cz"        # ← ZMĚŇTE na váš email
phone: "+420 XXX XXX XXX"            # ← ZMĚŇTE na váš telefon
address: "Vaše adresa"               # ← ZMĚŇTE na vaši adresu
city: "Praha"                        # ← ZMĚŇTE na vaše město
```

## 2. DOPORUČENÉ ÚPRAVY

### Přidat fotografie certifikátů
- Vytvořte složku: `assets/images/certificates/`
- Nahrajte obrázky: cert1.jpg, cert2.jpg, atd.
- Upravte soubor: `certifikace.md`

### Přidat mapu
- Otevřete: `kontakt.md`
- Najděte sekci "Mapa"
- Vložte Google Maps iframe

### Zkontrolovat ceny
- Otevřete: `cenik.md`
- Upravte ceny podle vašeho ceníku

### Upravit ordinační hodiny
- Otevřete: `kontakt.md`
- Upravte tabulku s ordinačními hodinami

## 3. TESTOVÁNÍ LOKÁLNĚ

```powershell
# V PowerShell:
cd c:\web\aja
bundle install
bundle exec jekyll serve
```

Pak otevřete: http://localhost:4000

## 4. NAHRÁNÍ NA GITHUB

### Varianta A: Git (rychlejší)
```powershell
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin main
```

### Varianta B: GitHub Desktop (jednodušší)
1. Stáhněte GitHub Desktop
2. File → Add Local Repository → vyberte c:\web\aja
3. Vytvořte commit
4. Publikujte

## 5. NASTAVENÍ GITHUB PAGES

1. Jděte do repozitáře na GitHubu
2. Settings → Pages
3. Source: main branch, / (root)
4. Custom domain: www.cestoustredu.cz
5. Zapnout: Enforce HTTPS

## 6. DNS NASTAVENÍ

U registrátora domény přidejte:

**CNAME záznam:**
- Název: www
- Hodnota: USERNAME.github.io
- TTL: 3600

**A záznamy:**
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

## 7. BARVY WEBU

- Primární (zelená): #2c7873
- Sekundární (zlatohnědá): #a67c52
- Tmavý text: #2d2d2d
- Světlé pozadí: #f8f9fa

Můžete změnit v: `assets/css/main.css` (sekce :root)

## 8. ČASTÉ DOTAZY

**Q: Kde změním text na úvodní stránce?**
A: V souboru `index.md`

**Q: Jak přidat novou stránku?**
A: Vytvořte nový .md soubor s front matter:
```yaml
---
layout: page
title: Název stránky
---
Obsah...
```

**Q: Jak aktualizovat web?**
A: Udělejte změny v souborech a pushněte na GitHub (git push)

**Q: Web nefunguje po nahrání**
A: Počkejte 3-5 minut na build, zkontrolujte Actions tab v GitHubu

**Q: DNS nefunguje**
A: DNS propagace trvá až 24h (obvykle 1h), zkontrolujte na dnschecker.org

## 9. KONTAKTY PRO POMOC

- Jekyll dokumentace: https://jekyllrb.com
- GitHub Pages: https://pages.github.com
- Markdown: https://www.markdownguide.org

## 10. STRUKTURA SOUBORŮ

```
c:\web\aja\
│
├── index.md              ← Domovská stránka
├── certifikace.md        ← Certifikace
├── sluzby.md            ← Co nabízím
├── biorezonance.md      ← Biorezonance
├── metody.md            ← Metody
├── cenik.md             ← Ceník
├── kontakt.md           ← Kontakt
├── gdpr.md              ← GDPR
│
├── _config.yml          ← ⚠️ HLAVNÍ KONFIGURACE
├── _layouts/            ← Šablony
├── _includes/           ← Komponenty (header, footer)
├── assets/
│   ├── css/main.css     ← Styly
│   └── js/main.js       ← JavaScript
│
├── CNAME                ← Doména
├── Gemfile              ← Ruby závislosti
├── README.md            ← Dokumentace
└── DEPLOYMENT.md        ← Podrobný návod
```

---

✅ Po dokončení všech úprav můžete web nahrát na GitHub!
