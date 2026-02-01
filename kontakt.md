---
layout: page
title: Kontakt
subtitle: Těším se na setkání s vámi
---

<div class="cards-grid" style="margin: 2rem 0;">
    <div class="card">
        <h3>📞 Telefon</h3>
        <p style="font-size: 1.25rem; margin: 1rem 0;">
            <a href="tel:{{ site.phone | replace: ' ', '' }}">{{ site.phone }}</a>
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            Volejte pro objednání nebo dotazy<br>
            Po–Pá: 9:00–18:00
        </p>
    </div>
    
    <div class="card">
        <h3>✉️ Email</h3>
        <p style="font-size: 1.25rem; margin: 1rem 0;">
            <a href="mailto:{{ site.email }}">{{ site.email }}</a>
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            Odpovídám obvykle do 24 hodin
        </p>
    </div>
    
    <div class="card">
        <h3>📍 Kde mě najdete</h3>
        <p style="margin: 1rem 0;">
            <strong>{{ site.address }}</strong><br>
            {{ site.city }}
        </p>
        <p style="font-size: 0.9rem; color: var(--text-light);">
            Parkování v blízkosti ordinace
        </p>
    </div>
</div>

<div style="background: var(--bg-light); padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0; max-width: 800px; margin-left: auto; margin-right: auto;">
    <h3 class="text-center">Objednání návštěvy</h3>
    <p class="text-center" style="margin-bottom: 2rem;">
        Pro objednání konzultace mě prosím kontaktujte telefonicky nebo emailem. 
        Společně najdeme vhodný termín a probereme vaše potřeby.
    </p>
    
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

<div style="background: white; padding: 2rem; border-radius: var(--radius-md); box-shadow: var(--shadow-md); margin: 3rem 0; max-width: 800px; margin-left: auto; margin-right: auto;">
    <h3>Ordinační hodiny</h3>
    <table style="width: 100%; margin-top: 1rem;">
        <tbody>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Pondělí</td>
                <td style="padding: 0.75rem; text-align: right;">9:00 – 18:00</td>
            </tr>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Úterý</td>
                <td style="padding: 0.75rem; text-align: right;">9:00 – 18:00</td>
            </tr>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Středa</td>
                <td style="padding: 0.75rem; text-align: right;">9:00 – 18:00</td>
            </tr>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Čtvrtek</td>
                <td style="padding: 0.75rem; text-align: right;">9:00 – 18:00</td>
            </tr>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Pátek</td>
                <td style="padding: 0.75rem; text-align: right;">9:00 – 16:00</td>
            </tr>
            <tr style="border-bottom: 1px solid var(--border-color);">
                <td style="padding: 0.75rem;">Sobota</td>
                <td style="padding: 0.75rem; text-align: right;">Po domluvě</td>
            </tr>
            <tr>
                <td style="padding: 0.75rem;">Neděle</td>
                <td style="padding: 0.75rem; text-align: right;">Zavřeno</td>
            </tr>
        </tbody>
    </table>
    <p style="margin-top: 1.5rem; font-size: 0.9rem; color: var(--text-light);">
        <em>* Ordinační hodiny jsou orientační. Konzultace probíhají na objednání.</em>
    </p>
</div>

<div style="background: var(--primary-light); color: white; padding: 2rem; border-radius: var(--radius-md); margin: 3rem 0; text-align: center;">
    <h3 style="color: white;">Máte dotazy?</h3>
    <p style="margin: 1rem 0;">
        Neváhejte mě kontaktovat s jakýmkoliv dotazem ohledně služeb, 
        metod nebo objednání. Ráda vám poradím a pomohu najít tu správnou cestu.
    </p>
</div>
