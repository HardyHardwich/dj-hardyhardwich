# Projekt: DJ Hardy Hardwich - Single Page Application (SPA)

## Projektübersicht

Diese **Single Page Application (SPA)** stellt eine professionelle DJ-Website dar, die vollständig dynamisch mit **PHP, HTML, CSS & JavaScript** arbeitet. Durch PHP werden **dynamische Inhalte** (Referenzen, Testimonials, Locations) nachgeladen. Zudem sorgt eine **SEO-Optimierung** für **Landingpages mit lokalen Städtenamen** für ein besseres Ranking in Suchmaschinen.

---

## 📁 Projektstruktur / Architektur

```
📂 root
├── 📂 api                         # Dynamische Inhalte per PHP
│   ├── cocompanys.php              # Kundenreferenzen (Firmen)
│   ├── testimonials.php           # Kundenmeinungen (Testimonials)
│   ├── referencelocations.php    
│   ├── generate_location_pages.php # Automatische SEO Landingpages für Städte
├── 📂 assets                      # Bilder, Logos & Medien
│   ├── 📂 css                     # Stile & Animationen
│   │   ├── style.css              # Haupt-CSS-Datei inkl. DarkMode & Animationen
│   │   ├── translations.json       # Sprachdatei für Mehrsprachigkeit
│   ├── 📂 images                  # Logos, Thumbnails, Backgrounds
│   ├── 📂 fonts                   # Benutzerdefinierte Schriftarten
│   ├── 📂 js                      # JavaScript für UI & Funktionen
│   │   ├── script.js              # Haupt-JS Datei inkl. Animationen, Formhandling
│   │   ├── darkmode.js            # Tag/Nacht Umschaltung
│   │   ├── translation.js         # Mehrsprachige Auto-Übersetzung
│   │   ├── testimonials.js        # Automatisches Rotieren der Testimonials
│   │   ├── gallery.js             # Lightbox & Hover Effekte
├── 📂 legal                       # Rechtliche Seiten
│   ├── impressum.html             # Impressum
│   ├── datenschutz.html           # Datenschutz
│   ├── agb.html                   # AGB
├── 📂 pages                       # Landingpages für regionale SEO
│   ├── hochzeits-dj-berlin.php    # Beispiel für eine lokale SEO Landingpage
│   ├── party-dj-potsdam.php       # Beispiel für eine weitere lokale Landingpage
├── index.html                     # Hauptseite (Single Page Application)
├── .htaccess                      # URL Rewrites für SEO & Routing
├── robots.txt                     # Suchmaschinen-Richtlinien
├── sitemap.xml                    # XML Sitemap für SEO
└── readme.md                      # Dokumentation
```

---

## 🌟 Features & Technologien

✅ **Single Page Application (SPA)** – Kein Page Reload, alle Inhalte werden dynamisch geladen  
✅ **Dynamische Inhalte mit PHP** – Testimonials, Referenzen & Locations per PHP nachgeladen  
✅ **SEO-Optimierung mit Local Landing Pages** – Automatisch generierte Städte-Landingpages  
✅ **Dark Mode Toggle** – Nutzerfreundliche Umschaltung zwischen Tag & Nachtmodus  
✅ **Automatische Sprachübersetzung** – Mehrsprachig durch Auto-Detection & Benutzerwahl  
✅ **Lightbox Galerie & Hover-Effekte** – Responsive & modern für Bildergalerien  
✅ **Testimonials & Referenzen mit Animationen** – Dynamisches Karussell mit Überblendungen  
✅ **Schüttel-Interaktion für zufällige Event-Ideen** – Interaktives Feature für Nutzer  
✅ **Preisrechner für DJ-Buchung** – Benutzer erhält eine transparente Preisberechnung  
✅ **Playlist-Generator mit KI** – Nutzer erstellt & sendet Wunsch-Playlist für Event  
✅ **Google Maps Integration & Routenplaner** – Einfache Navigation zur Event-Location  
✅ **WhatsApp, Facebook Messenger & Direktanruf-Buttons** – Einfache Kontaktmöglichkeiten  
✅ **Animierte Call-to-Action Buttons** – Animierte Buttons für höhere Conversion  
✅ **Mutige Blocklayouts & Retro-Neonfarben** – Modernes Design für Club-Feeling  
✅ **Mobile-First-Design** – Optimierung für alle Bildschirmgrößen mit Touch-Interaktion  

---

## 🛠 Installation & Nutzung

1. **Server Anforderungen**

   - PHP 7.4 oder höher
   - Apache Server mit mod\_rewrite
   - MySQL (optional für erweiterte Funktionen)
   - SSL-Zertifikat für HTTPS (empfohlen)

2. **Projekt Klonen & Einrichten**

   ```sh
   git clone https://github.com/deinrepo/dj-hardyhardwich.git
   cd dj-hardyhardwich
   ```

3. **Webserver Konfiguration** (Optional für Local SEO)

   - `.htaccess` aktivieren & mod\_rewrite einschalten:
     ```apache
     RewriteEngine On
     RewriteRule ^(.*)/$ /index.html [L,QSA]
     ```

4. **Übersetzungen aktivieren**

   - Sprache basierend auf Nutzer-Standort:
     ```js
     fetch('/api/detect_city.php').then(response => response.json()).then(data => {
         loadTranslation(data.language || 'de');
     });
     ```

5. **Automatische SEO Landingpages generieren**

   ```sh
   php api/generate_location_pages.php
   ```

---

## 🔗 Wichtige Links & Weiterentwicklung

- **Website Live-Demo:** [www.hardyhardwich.de](https://www.hardyhardwich.de)
- **Bug Reporting:** [GitHub Issues](https://github.com/deinrepo/dj-hardyhardwich/issues)
- **Feature Requests:** [GitHub Discussions](https://github.com/deinrepo/dj-hardyhardwich/discussions)
- **API Doku:** `/api/docs`

---

## 🚀 Nächste geplante Features

- **KI-gestützte Event-Playlist Empfehlung** 🎵
- **Dynamische Preiskalkulation basierend auf Standort & Event-Dauer** 💰
- **Live Chat mit AI für Kundenanfragen** 🧠
- **SEO A/B-Testing mit verschiedenen Landingpage-Titeln** 📊

---

📌 **Lizenz:** Open Source MIT License  
📌 **Entwickelt von:** DJ Hardy Hardwich alias Nicky Hartwig
