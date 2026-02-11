---
layout: page
title: Kontakt
subtitle: Těším se na setkání s vámi
permalink: /kontakt/
---

<div class="cards-grid" style="margin: 2rem 0;">
    <div class="card">
        <h3>📞 Telefon</h3>
        <p style="font-size: 1.25rem; margin: 1rem 0;">
            <a href="tel:{{ site.phone | replace: ' ', '' }}">{{ site.phone }}</a>
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            Pro objednání, prosím, pište sms, email či využijte whatsapp, případně volejte. Ozvu se vám, jakmile to bude možné. <br>
            Po–Pá: 9:00–18:00 
        </p>
    </div>
    
    <div class="card">
        <h3>✉️ Email</h3>
        <p style="font-size: 1.25rem; margin: 1rem 0;">
            <a href="mailto:{{ site.email }}">{{ site.email }}</a>
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            
        </p>
    </div>
    
    <div class="card">
        <h3>📍 Kde mě najdete</h3>
        <p style="margin: 1rem 0;">
            <strong>{{ site.address }}</strong><br>
            {{ site.city }}
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            Parkování u domu. Bezbarierový přístup.
        </p>
    </div>
</div>

<div style="background: var(--bg-light); padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0; max-width: 800px; margin-left: auto; margin-right: auto;">
    <h3 class="text-center">Objednání návštěvy</h3>
    <p class="text-center" style="margin-bottom: 2rem;">
        Pro objednání konzultace mě,prosím, kontaktujte sms, whatsapp  nebo emailem. Případně telefonicky, ozvu se vám, jakmile to bude možné.
        Společně najdeme vhodný termín.   </p>
    
    <div style="text-align: center;">
        <a href="tel:{{ site.phone | replace: ' ', '' }}" class="btn btn-primary">
            Zavolat {{ site.phone }}
        </a>
        <a href="mailto:{{ site.email }}" class="btn btn-secondary">
            Napsat email
        </a>
    </div>
</div>

<div style="margin: 3rem 0;">
    <h3 class="text-center" style="margin-bottom: 2rem;">Mapa</h3>
    <div style="background: var(--bg-light); padding: 3rem; border-radius: var(--radius-md); text-align: center; color: var(--text-light);">
        <p>
            <em>Zde bude umístěna mapa s polohou ordinace</em>
        </p>
        <p style="margin-top: 1rem; font-size: 0.9rem;">
            Vložte Google Maps iframe nebo jinou mapovou službu s vaší adresou
        </p>
    </div>
</div>
    <p style="margin-top: 1.5rem; font-size: 0.9rem; color: var(--text-light);">
        <em>*  Konzultace probíhají dle objednání či domluvy.</em>
    </p>
</div>

<div style="background: var(--primary-light); color: white; padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0; text-align: center;">
    <h3 style="color: white;">Máte dotazy?</h3>
    <p style="margin: 1rem 0;">
        Neváhejte mě kontaktovat s jakýmkoliv dotazem ohledně služeb, 
        metod nebo objednání. Ráda vám poradím a pomohu najít tu správnou cestu.
    </p>
</div>
