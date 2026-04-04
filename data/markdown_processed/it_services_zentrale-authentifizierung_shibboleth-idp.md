---
title: Shibboleth Identity Provider (IdP) und Single Sign-On (SSO) an der Universität Mannheim
source_url_de: https://www.uni-mannheim.de/it/services/zentrale-authentifizierung/shibboleth-idp/
source_url_en: https://www.uni-mannheim.de/en/it/services/central-authentication/shibboleth-idp/
category: Services
tags: ['Shibboleth', 'SSO', 'Single Sign-On', 'Authentifizierung', 'IdP', 'bwIDM', 'Uni Mannheim']
language: de
---

# Shibboleth Identity Provider (IdP) und Single Sign-On (SSO)

Der Shibboleth Identity Provider (IdP) bietet Authentifizierung und Autorisierung mittels Single Sign-On (SSO) für teilnehmende Service Provider. Er ist ein integraler Bestandteil der [bwIDM](https://www.bwidm.de/)-Infrastruktur.

## Was ist Single Sign-On (SSO)?

Single Sign-On (SSO) ist ein Login-Dienst, der es Nutzern ermöglicht, sich für mehrere Webseiten nur einmal einzuloggen.

- **CAS:** Bietet beispielsweise Zugang zum Portal der Uni Mannheim.
- **Shibboleth Identity Provider (IdP):** Bietet Zugang zu lokalen Diensten, die meist von anderen Hochschulen und Einrichtungen stammen.

## Wofür benötige ich den Shibboleth Identity Provider (IdP)?

Viele wissenschaftliche Dienste weltweit sind für eine große Anzahl von Personen erreichbar. Anstatt für jede Person ein eigenes Konto anzulegen, nutzen diese Dienste die SAML-Technologie. Dadurch kann das Konto der Heimatuniversität verwendet werden, wodurch die Einrichtung eines zusätzlichen Kontos entfällt. Der IdP kann bei Bedarf die notwendigen Informationen an den jeweiligen Dienst übermitteln.

## Der IdP-Login-Ablauf

Der Anmeldeprozess ist mehrstufig:

1. **Start:** Der Vorgang beginnt auf der Webseite des Ziel-Dienstes, wo Sie eine Login-Möglichkeit wie „Shibboleth“ oder „bwIDM“ auswählen.
1. **Hochschule wählen:** Anschließend wählen Sie Ihre zugehörige Hochschule aus. Bei nicht-deutschen Diensten muss zuvor die Föderation „DFN-AAI“ oder „German Higher Education and Research“ ausgewählt werden.
1. **Authentifizierung:** Sie werden zum IdP der Universität Mannheim weitergeleitet, wo Sie sich mit Ihrer Uni-ID und dem zugehörigen Passwort authentifizieren.
1. **Datenübermittlung:** Nach erfolgreicher Authentifizierung werden alle Daten, die an den Dienst gesendet werden sollen, zur Kenntnisnahme angezeigt und anschließend übermittelt. Der Dienst nimmt die Daten entgegen und gewährt in der Regel den Zugriff.

Ein detailliertes Beispiel finden Sie in unserer [Anleitung zum Login](https://www.uni-mannheim.de/it/services/zentrale-authentifizierung/shibboleth-idp/anleitung-login/).

**Probleme auftreten?**

- Beachten Sie bitte die [Hinweise zu den Diensten](https://www.uni-mannheim.de/it/services/zentrale-authentifizierung/shibboleth-idp-dienste/).
- Wenden Sie sich an den [IT-Support](https://www.uni-mannheim.de/it/support/).

## Verfügbare Dienste

Eine [Liste der eingerichteten Dienste](https://www.uni-mannheim.de/it/services/zentrale-authentifizierung/shibboleth-idp-dienste/) mit zugehörigen Hinweisen ist auf einer separaten Seite verfügbar. Diese Liste ist nicht abschließend.

- **Baden-Württemberg:** Alle Dienste aus Baden-Württemberg sind auf der [Dienste-Seite von bwIDM](https://www.bwidm.de/dienste/) zu finden und sind auch Dienste der Föderation [DFN-AAI](https://www.aai.dfn.de/der-dienst/).
- **DFN-AAI:** Eine vollständige Liste aller Dienste der DFN-AAI-Föderation ist auf den [Seiten des DFN](https://www.aai.dfn.de/verzeichnis/sp-dfn-aai/) zu finden.

**Wichtig:** Nicht alle DFN-Dienste sind über den IdP der Universität Mannheim nutzbar, da ein Datenabgleich mit jedem Dienst geklärt werden muss. Benötigen Sie Zugang zu einem bisher nicht unterstützten Dienst, melden Sie sich bitte beim [IT-Support](https://www.uni-mannheim.de/it/support/).

## Häufig gestellte Fragen (FAQ)

**Wie kann ich mich wieder ausloggen?**
Ein Single-Logout (Ausloggen bei allen angemeldeten Diensten auf Knopfdruck) ist aktuell nicht möglich. Zum Ausloggen können Sie den Browser schließen oder Cookies löschen. Alternativ läuft die Sitzung des Dienstes nach einiger Zeit automatisch ab.

**Wann muss ich mein Passwort erneut eingeben? / Wie lange ist meine Sitzung gültig?**
Mit dem Login beginnt eine zeitlich begrenzte Sitzung, deren Dauer vom jeweiligen Dienst festgelegt wird. Ist die Sitzung beim Dienst abgelaufen, ist ein erneuter Besuch beim IdP notwendig.

**Ich habe das Passwort meiner Uni-ID vergessen. Was nun?**
Folgen Sie bitte unserer Anleitung [„Passwort vergessen“](https://www.uni-mannheim.de/it/anleitungen/passwort/).

**Die IdP-Seiten werden mir auf Englisch angezeigt. Wie ändere ich die Sprache?**
Die Sprache im IdP wird automatisch durch die Browsersprache festgelegt.

## Technische Metainformationen (IdP)

**EntityID:** `https://idp.uni-mannheim.de/idp/shibboleth`
**Scope:** `uni-mannheim.de` (ausschließlich)
**Federationen:** German Higher Education and Research (DFN-AAI), eduGAIN
