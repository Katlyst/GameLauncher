
# 🛡️ Sicherheitsdokumentation

## Implementierte Sicherheitsmaßnahmen

### 1. Content Security Policy (CSP)
- Verhindert XSS-Angriffe
- Kontrolliert externe Ressourcen
- Blockiert unsichere Inline-Skripte

### 2. Security Headers
- `X-Content-Type-Options: nosniff` - Verhindert MIME-Type-Sniffing
- `X-Frame-Options: SAMEORIGIN` - Schutz vor Clickjacking
- `X-XSS-Protection: 1; mode=block` - XSS-Filter aktiviert
- `Referrer-Policy: strict-origin-when-cross-origin` - Kontrollierte Referrer-Übertragung

### 3. Subresource Integrity (SRI)
- Pico CSS wird mit Integrity-Hash geladen
- Schutz vor manipulierten externen Ressourcen

### 4. Datenschutz
- Keine Cookies oder Tracking
- Lokale Formulardaten (nicht übertragen)
- YouTube-Inhalte nur mit Zustimmung
- Sichere externe Bildquellen

### 5. Sichere externe Links
- `rel="noopener noreferrer"` für alle externen Links
- Verhindert window.opener-Zugriff

## Regelmäßige Sicherheitschecks
- CSP-Header validieren
- Externe Ressourcen auf Aktualität prüfen
- SRI-Hashes bei Updates erneuern
