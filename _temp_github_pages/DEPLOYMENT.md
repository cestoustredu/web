# Cestou Středu - Deployment na GitHub Pages

## Příprava GitHub repozitáře

1. **Vytvořte GitHub účet** (pokud ještě nemáte): https://github.com

2. **Vytvořte nový repozitář:**
   - Klikněte na "New repository"
   - Název: `cestoustredu` (nebo jiný název)
   - Nastavte jako Public
   - Neklikejte na "Initialize this repository with a README"

## Nahrání souborů

### Pomocí Git (doporučeno)

Otevřete PowerShell v této složce (`c:\web\aja`) a spusťte:

```powershell
# Inicializace Git repozitáře
git init

# Přidání všech souborů
git add .

# První commit
git commit -m "Initial commit - Cestou Středu website"

# Propojení s GitHub (nahraďte USERNAME a REPOSITORY)
git remote add origin https://github.com/USERNAME/REPOSITORY.git

# Nahrání na GitHub
git branch -M main
git push -u origin main
```

### Pomocí GitHub Desktop (jednodušší varianta)

1. Stáhněte a nainstalujte GitHub Desktop: https://desktop.github.com
2. Přihlaste se svým GitHub účtem
3. File → Add Local Repository → vyberte složku `c:\web\aja`
4. Vytvořte commit s popisem
5. Publikujte repozitář

## Nastavení GitHub Pages

1. **Jděte do nastavení repozitáře:**
   - Settings → Pages (v levém menu)

2. **Vyberte zdroj:**
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/ (root)`
   - Klikněte Save

3. **Počkejte na build:**
   - GitHub automaticky sestaví web (trvá 1-3 minuty)
   - Po dokončení se zobrazí zelená zpráva s URL

## Nastavení vlastní domény (www.cestoustredu.cz)

### 1. Nastavení DNS u vašeho registrátora domény

Přidejte následující DNS záznamy:

**Pro www.cestoustredu.cz (doporučeno):**
```
Typ: CNAME
Název: www
Hodnota: USERNAME.github.io
TTL: 3600
```

**Pro cestoustredu.cz (root doména):**
```
Typ: A
Název: @
Hodnota: 185.199.108.153
TTL: 3600

Typ: A
Název: @
Hodnota: 185.199.109.153
TTL: 3600

Typ: A
Název: @
Hodnota: 185.199.110.153
TTL: 3600

Typ: A
Název: @
Hodnota: 185.199.111.153
TTL: 3600
```

### 2. Nastavení v GitHub Pages

1. V Settings → Pages najděte sekci "Custom domain"
2. Zadejte: `www.cestoustredu.cz`
3. Klikněte Save
4. Po chvíli zaškrtněte "Enforce HTTPS" (pro zabezpečené spojení)

### 3. Počkejte na propagaci DNS

- DNS změny se propagují 1-24 hodin (obvykle do 1 hodiny)
- Můžete kontrolovat na: https://dnschecker.org

## Aktualizace webu

### Pomocí Git

```powershell
# Přidání změn
git add .

# Commit
git commit -m "Popis změn"

# Nahrání na GitHub
git push
```

GitHub Pages automaticky znovu sestaví web do několika minut.

### Pomocí GitHub Desktop

1. Udělejte změny v souborech
2. V GitHub Desktop uvidíte změněné soubory
3. Napište popis změn a klikněte "Commit to main"
4. Klikněte "Push origin"

## Testování lokálně

Před nahráním na GitHub můžete web otestovat lokálně:

### 1. Instalace Ruby a Jekyll

**Windows:**
- Stáhněte RubyInstaller: https://rubyinstaller.org/downloads/
- Nainstalujte Ruby+Devkit (doporučeno verze 3.1)
- Při instalaci zaškrtněte "Add Ruby to PATH"

### 2. Instalace závislostí

```powershell
cd c:\web\aja
gem install bundler
bundle install
```

### 3. Spuštění lokálního serveru

```powershell
bundle exec jekyll serve
```

Web bude dostupný na: http://localhost:4000

Pro zastavení serveru stiskněte `Ctrl+C`

## Důležité úpravy před spuštěním

V souboru `_config.yml` upravte:

```yaml
email: "vase@email.cz"              # Váš email
phone: "+420 XXX XXX XXX"           # Váš telefon
address: "Vaše adresa"              # Vaše adresa
city: "Město"                       # Město
```

## Přidání fotografií certifikátů

1. Vytvořte složku: `assets/images/certificates/`
2. Uložte obrázky certifikátů (např. `cert1.jpg`, `cert2.jpg`)
3. Upravte soubor `certifikace.md` - nahraďte placeholders odkazy na vaše obrázky:

```html
<img src="{{ '/assets/images/certificates/cert1.jpg' | relative_url }}" alt="Certifikát">
```

## Přidání mapy

V souboru `kontakt.md` najděte sekci s mapou a vložte iframe z Google Maps:

1. Otevřete Google Maps
2. Najděte vaši adresu
3. Klikněte "Sdílet" → "Vložit mapu"
4. Zkopírujte iframe kód
5. Vložte místo placeholderu

## Podpora a pomoc

- **Jekyll dokumentace:** https://jekyllrb.com/docs/
- **GitHub Pages:** https://docs.github.com/pages
- **Problém s buildem:** Zkontrolujte Actions tab v repozitáři

## Kontrolní seznam před spuštěním

- [ ] Upraveny kontaktní údaje v `_config.yml`
- [ ] Přidány fotografie certifikátů
- [ ] Přidána mapa v kontaktech
- [ ] Upraveny ordinační hodiny
- [ ] Zkontrolovány a upraveny ceny
- [ ] Otestováno lokálně
- [ ] Nahráno na GitHub
- [ ] Nastaveny DNS záznamy
- [ ] Zapnut HTTPS v GitHub Pages

## Tipy pro optimalizaci

1. **Optimalizujte obrázky:** Používejte formáty WebP nebo optimalizované JPG (max 200 KB)
2. **Přidejte favicon:** Vytvořte `favicon.ico` a umístěte do root složky
3. **Google Analytics:** Pro sledování návštěvnosti přidejte tracking kód
4. **SEO:** Upravte meta popisky v jednotlivých stránkách

Vaše webové stránky jsou připraveny k nasazení! 🚀
