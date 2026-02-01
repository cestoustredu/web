---
layout: page
title: Ceník
subtitle: Přehled služeb a cen
permalink: /cenik/
---

<div class="pricing-table">
    <div class="price-item">
        <div>
            <h3>Úvodní konzultace</h3>
            <p>Rozhovor + diagnostika + doporučení (90-120 min)</p>
        </div>
        <div class="price">1 500 Kč</div>
    </div>
    
    <div class="price-item">
        <div>
            <h3>Kontrolní konzultace</h3>
            <p>Kontrola stavu + úprava doporučení (60 min)</p>
        </div>
        <div class="price">1 000 Kč</div>
    </div>
    
    <div class="price-item">
        <div>
            <h3>Biorezonanční vyšetření Oberon</h3>
            <p>Komplexní diagnostika organismu</p>
        </div>
        <div class="price">800 Kč</div>
    </div>
    
    <div class="price-item">
        <div>
            <h3>Kvantová analýza</h3>
            <p>Rychlá analýza funkčního stavu organismu</p>
        </div>
        <div class="price">500 Kč</div>
    </div>
    
    <div class="price-item">
        <div>
            <h3>HRV měření</h3>
            <p>Variabilita srdeční frekvence + vyhodnocení</p>
        </div>
        <div class="price">400 Kč</div>
    </div>
    
    <div class="price-item">
        <div>
            <h3>Plazma FQ Qmtrin aplikace</h3>
            <p>Harmonizace a revitalizace (30 min)</p>
        </div>
        <div class="price">600 Kč</div>
    </div>
</div>

<div style="background: var(--bg-light); padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0;">
    <h3>Důležité informace</h3>
    <ul class="service-list">
        <li>Ceny jsou orientační a mohou se lišit podle individuálních potřeb</li>
        <li>První konzultace doporučuji delší (90-120 min) pro komplexní zhodnocení</li>
        <li>Následné konzultace jsou kratší (60 min) a zaměřují se na kontrolu a úpravu terapie</li>
        <li>Jednotlivá vyšetření lze kombinovat podle potřeby</li>
        <li>Při opakovaných návštěvách možnost balíčků konzultací za zvýhodněnou cenu</li>
    </ul>
</div>

## Storno podmínky

<div style="background: white; padding: 2rem; border-radius: var(--radius-md); box-shadow: var(--shadow-md); margin: 2rem 0;">
    <h3>Zrušení objednané návštěvy</h3>
    
    <div style="margin: 1.5rem 0;">
        <h4>Včasné zrušení (více než 24 hodin před termínem)</h4>
        <p>
            Pokud zrušíte objednanou návštěvu více než 24 hodin před plánovaným termínem, 
            nevzniká žádný poplatek. Termín můžete zdarma přeobjednat na jiný vhodný čas.
        </p>
    </div>
    
    <div style="margin: 1.5rem 0;">
        <h4>Pozdní zrušení (méně než 24 hodin před termínem)</h4>
        <p>
            Při zrušení návštěvy méně než 24 hodin před plánovaným termínem účtuji 
            storno poplatek ve výši <strong>50% z ceny objednané služby</strong>.
        </p>
    </div>
    
    <div style="margin: 1.5rem 0;">
        <h4>Nedostavení se bez omluvy</h4>
        <p>
            V případě nedostavení se na objednanou návštěvu bez předchozí omluvy 
            účtuji storno poplatek ve výši <strong>100% z ceny objednané služby</strong>.
        </p>
    </div>
    
    <div style="margin-top: 2rem; padding: 1rem; background: var(--bg-light); border-radius: var(--radius-sm);">
        <p><strong>Jak zrušit návštěvu:</strong></p>
        <p>
            Zrušení nebo přeobjednání termínu prosím oznamte telefonicky na 
            <a href="tel:{{ site.phone | replace: ' ', '' }}">{{ site.phone }}</a> 
            nebo emailem na <a href="mailto:{{ site.email }}">{{ site.email }}</a>.
        </p>
    </div>
</div>

<div style="background: var(--primary-light); color: white; padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0; text-align: center;">
    <h3 style="color: white;">Dárkové poukazy</h3>
    <p style="margin: 1rem 0;">
        Hledáte originální dárek pro své blízké? Nabízím dárkové poukazy na konzultace 
        a vyšetření v libovolné hodnotě.
    </p>
    <a href="{{ '/kontakt/' | relative_url }}" class="btn" style="background: white; color: var(--primary-color);">
        Informace o dárkových poukazech
    </a>
</div>

<div style="text-align: center; margin-top: 3rem;">
    <a href="{{ '/kontakt/' | relative_url }}" class="btn btn-primary">Objednat se</a>
    <a href="{{ '/sluzby/' | relative_url }}" class="btn btn-outline">Co nabízím</a>
</div>
