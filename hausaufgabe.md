# Hausaufgabe: Dashboard für Schrauben24.de

## Aufgabenstellung

Erstelle ein professionelles Dashboard für das Unternehmen **Schrauben24.de** mit Chart.js und Bootstrap. Du sollst die Geschäftsdaten des Online-Schraubenhändlers visualisieren.

## Anforderungen

### Technische Anforderungen:
- **HTML-Datei** mit Bootstrap CSS Framework
- **Chart.js** für alle Diagramme 
- **Mindestens 4 verschiedene Charts** (siehe unten)
- **Responsive Design** - funktioniert auf Desktop und Handy

### Pflicht-Charts:
1. **Liniendiagramm:** Monatlicher Umsatz 2024
2. **Balkendiagramm:** Top 5 Produktkategorien
3. **Tortendiagramm:** Versandarten-Verteilung
4. **Horizontal Bar:** Lagerbestände nach Standorten

### Optional (Bonuspunkte):
- Mixed Chart (Balken + Linie)
- Animationen
- Weitere Charts deiner Wahl
- Eigenes Styling/Farben

## Über Schrauben24.de

**Schrauben24.de** ist ein Online-Händler für Befestigungsmaterial mit:
- Hauptsitz in München
- 3 Lagerhallen (München, Hamburg, Köln)
- Über 10.000 verschiedene Schrauben, Muttern und Bolzen
- 50.000+ zufriedene Kunden deutschlandweit

## Deine Daten (JSON Format)

Kopiere diese JSON-Daten und verwende sie für deine Charts:

### Monatliche Umsätze 2024
```json
{
  "monate": ["Jan", "Feb", "Mär", "Apr", "Mai", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dez"],
  "umsatz": [125000, 142000, 168000, 195000, 210000, 235000, 258000, 242000, 220000, 205000, 180000, 310000]
}
```

### Top 5 Produktkategorien (Stückzahl verkauft)
```json
{
  "kategorien": ["Holzschrauben", "Metallschrauben", "Muttern", "Bolzen", "Unterlegscheiben"],
  "stueckzahl": [45200, 38500, 32100, 28700, 24800]
}
```

### Versandarten (Prozent der Bestellungen)
```json
{
  "versandarten": ["Standard (2-3 Tage)", "Express (1 Tag)", "Selbstabholung", "Spedition"],
  "prozent": [65, 20, 10, 5]
}
```

### Lagerbestände nach Standorten (in Tonnen)
```json
{
  "standorte": ["München (Zentrale)", "Hamburg (Nord)", "Köln (West)"],
  "lagerbestand": [850, 420, 380]
}
```

### Bonus: Umsatz vs. Bestellungen (für Mixed Chart)
```json
{
  "monate": ["Jan", "Feb", "Mär", "Apr", "Mai", "Jun"],
  "umsatz": [125000, 142000, 168000, 195000, 210000, 235000],
  "bestellungen": [2100, 2400, 2800, 3200, 3500, 3900]
}
```

## Technische Hilfen

### CDN Links (für dein HTML):
```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Chart.js -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<!-- Bootstrap JS (optional für Responsive) -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

### Beispiel Bootstrap Layout:
```html
<div class="container-fluid">
    <div class="row">
        <div class="col-md-6">
            <!-- Chart 1 hier -->
        </div>
        <div class="col-md-6">
            <!-- Chart 2 hier -->
        </div>
    </div>
    <div class="row">
        <div class="col-md-6">
            <!-- Chart 3 hier -->
        </div>
        <div class="col-md-6">
            <!-- Chart 4 hier -->
        </div>
    </div>
</div>
```

## Arbeiten mit ChatGPT

### Erlaubte Hilfe:
- ChatGPT fragen wie Bootstrap Grid funktioniert
- Fragen zu Chart.js Syntax und Optionen
- Hilfe beim CSS Styling
- Debugging von JavaScript Fehlern
- Fragen zu responsive Design

### Wichtig:
- **Verstehe den Code** den ChatGPT vorschlägt
- **Ändere die Beispiele ab** und mache sie zu deinen eigenen
- **Teste verschiedene Optionen** aus der Chart.js Dokumentation
- **Sei kreativ** mit Farben und Design

## Tipps für den Erfolg

### Design-Tipps:
- Verwende **einheitliche Farben** für dein Unternehmen
- **Blau/Grau** passt gut zu einem B2B-Geschäft wie Schrauben24.de
- Achte auf **gute Kontraste** für Lesbarkeit
- **Titel und Beschriftungen** nicht vergessen!

### Häufige Fehler vermeiden:
- Canvas-IDs müssen **einzigartig** sein
- **JavaScript-Fehler** in der Browser-Konsole checken (F12)
- **Bootstrap Klassen** richtig verwenden (`col-md-6` nicht `col-6-md`)
- Charts brauchen **Höhe** - setze CSS height oder verwende maintainAspectRatio

### Responsive checken:
- Browser-Entwicklertools verwenden (F12 → Device Toolbar)
- Testen mit verschiedenen Bildschirmgrößen
- Charts sollten sich anpassen, nicht überlaufen

---

## Viel Erfolg!