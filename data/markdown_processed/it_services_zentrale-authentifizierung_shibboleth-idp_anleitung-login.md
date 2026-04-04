---
title: Shibboleth Single Sign-On (SSO) Login und Logout Anleitung
source_url_de: https://www.uni-mannheim.de/it/services/zentrale-authentifizierung/shibboleth-idp/anleitung-login/
source_url_en: https://www.uni-mannheim.de/en/it/services/central-authentication/shibboleth-idp/login-instructions/
category: Services
tags: ['Shibboleth', 'SSO', 'Login', 'Authentifizierung', 'Uni Mannheim', 'Logout', 'Zugang', 'Zentraler Dienst']
language: de
---

# Shibboleth Identity Provider – Login & Logout Anleitung

## Shibboleth Single Sign-On (SSO) Login-Ablauf

Der Anmeldeprozess bei einem Dienst ist in mehrere Schritte unterteilt und beginnt immer auf der Webseite des jeweiligen Dienstes.

**Schritt 1: Dienstauswahl**
Wählen Sie auf der Startseite des Dienstes die gewünschte Login-Möglichkeit, beispielsweise „Shibboleth“ oder „bwIDM“.

**Schritt 2: Institution identifizieren**
Wählen Sie anschließend die zugehörige Hochschule („Universität Mannheim“). Bei nicht-deutschen Diensten muss zuvor die Föderation „DFN-AAI“ oder „German Higher Education and Research“ ausgewählt werden. Der Dienst fragt nach dem Herkunftsort (WAYF – „Where Are You From“).
*Hinweis:* Bei manchen Diensten (z.B. bwidm.scc.kit.edu) ist der WAYF-Dienst bereits auf der Startseite integriert.

**Schritt 3: Authentifizierung**
Nach der Auswahl werden Sie zum IdP der Universität Mannheim weitergeleitet, wo Sie sich mit Kennung und Passwort authentifizieren müssen.
*Hinweis:* Um beispielsweise für Support-Zwecke einen bestimmten Schritt zu erzwingen, setzen Sie den Haken bei: „Lösche die frühere Einwilligung zur Weitergabe Ihrer Informationen an diesen Dienst.“

**Schritt 4: Datenübermittlung**
Nach erfolgreicher Authentifizierung werden alle Daten, die an den Dienst gesendet werden sollen, zur Kenntnisnahme angezeigt. Anschließend werden die Daten an den Dienst übermittelt.

**Zusätzliche Hinweise:**

- **Unbekannte Dienste:** Benötigen Sie Zugang zu einem Dienst, der bisher nicht unterstützt wird, melden Sie sich bitte bei uns. Wir werden unser Bestes tun, um den Zugang zeitnah zu ermöglichen.
- **Selten genutzte Dienste:** Speziell für Dienste, die Sie nicht regelmäßig verwenden, empfiehlt sich die Option „Bei nächster Anmeldung erneut anzeigen“ auszuwählen.

## Logout-Verfahren

Ein Single-Logout (Ausloggen bei allen angemeldeten Diensten auf Knopfdruck) ist aktuell nicht möglich.

**Empfohlene Vorgehensweise:**

1. **Browser schließen:** Schließen Sie den Browser.
1. **Cookies löschen:** Löschen Sie die Cookies, um die Sitzung zu beenden.
1. **Sitzenauslaufen:** Alternativ läuft die Sitzung des Dienstes nach einer gewissen Zeit automatisch ab.

**Anleitung zum Löschen von Cookies (Beispiel Mozilla Firefox):**
Das Löschen der aktuellsten Chronik/des aktuellen Verlaufs ist der einfachste Weg.

1. Wählen Sie unter „Chronik“ den Punkt „Neueste Chronik löschen...“ aus. (In älteren Browsern: Extras, Shortcut: `Strg + Umschalt + Entf`)
1. Wählen Sie den gewünschten Zeitrahmen (z.B. „Alles“).
1. Aktivieren Sie nur die Optionen „Cookies“, „Cache“ und „Aktive Logins“ und klicken Sie auf „Jetzt löschen“.
