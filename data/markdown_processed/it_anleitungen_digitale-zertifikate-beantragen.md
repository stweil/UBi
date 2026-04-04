---
title: Anleitung zur Beantragung, Verwaltung und Sperrung digitaler Zertifikate
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/en/
category: Services
tags: ['digitales Zertifikat', 'Beantragung', 'Sperrung', 'Outlook', 'HARICA', 'Server', 'Persönlich']
language: de
---

# Digitale Zertifikate: Beantragung und Verwaltung

In dieser Anleitung finden Sie Schritt-für-Schritt-Anleitungen zur Beantragung, Verwaltung und Sperrung verschiedener Arten digitaler Zertifikate. Bitte wählen Sie den entsprechenden Zertifikat-Typ aus.

Für allgemeine Informationen zu den einzelnen Zertifikaten besuchen Sie bitte [Services/ TCS Zertifikate](https://www.uni-mannheim.de/it/services/tsc-zertifikate).

## 🔑 Persönliches Zertifikat

### 1. Beantragung eines persönlichen Zertifikats

Folgen Sie diesen Schritten, um Ihr persönliches digitales Zertifikat zu beantragen:

**Vorbereitung:**

1. Klicken Sie auf diesen [Link](https://cm.harica.gr), um zur Beantragung bei unserem Zertifikatsanbieter HARICA zu gelangen.
1. Wählen Sie „Academic Login“ zur Anmeldung bei HARICA.
1. Wählen Sie zunächst die Institution. Geben Sie „Mannheim“ in die Suchleiste ein, um „University of Mannheim“ auszuwählen und auf die Anmeldeseite weitergeleitet zu werden. Melden Sie sich dort mit Ihrer Uni-ID und Ihrem Passwort an.

**Zertifikatstyp wählen:**
4\. Wählen Sie auf der linken Seite den Menüpunkt „Email“.
5\. Wählen Sie als Zertifikatstyp „**E@only**“.
6\. Scrollen Sie nach unten und wählen Sie **Next**.
7\. Belassen Sie die vorausgewählte Verifizierungsmethode und wählen Sie **Next**.
8\. Überprüfen Sie die Angaben und stimmen Sie den „Terms of Use“ von HARICA zu, indem Sie einen Haken setzen und mit **Next** bestätigen.
9\. Sie erhalten eine E-Mail von HARICA mit einem Bestätigungslink. Klicken Sie auf die „Confirm“ Schaltfläche, um fortzufahren.
10\. Klicken Sie erneut auf die Schaltfläche „Confirm“.
11\. Sie werden zum Dashboard des HARICA Zertifikatsmanagers weitergeleitet. Klicken Sie im Bereich „Pending Certificates“ auf „Enroll your Certificate“.
12\. Wählen Sie als Keysize den Wert „4096“ und legen Sie ein sicheres Passwort für Ihre Zertifikatsdatei fest. Bestätigen Sie, dass Sie das alleinige Wissen über dieses Passwort besitzen. Klicken Sie auf „Enroll Certificate“.
13\. Klicken Sie auf „Download“ und laden Sie Ihr Zertifikat im **.p12 Format** herunter. **Achtung:** Geben Sie diese Datei niemals an andere Personen weiter!

### 2. Einbinden des Zertifikats in Outlook

Standardmäßig verwendet Outlook das Verfahren SHA1, was zu Fehlermeldungen führen kann. Die Universitäts-IT empfiehlt daher die Verwendung eines neueren Verfahrens wie SHA256.

**Zertifikat importieren:**

1. Klicken Sie in Outlook unter „Datei“ auf „Optionen“ und anschließend auf „Trust Center“. Wählen Sie „Einstellungen für das Trust Center...“.
1. Klicken Sie unter „E-Mail-Sicherheit“ auf „Importieren/ Exportieren...“.
1. Wählen Sie die exportierte Zertifikatsdatei aus, geben Sie das Kennwort ein und klicken Sie auf „OK“.
1. Setzen Sie den Haken bei „Ausgehende Nachrichten digitale Signatur hinzufügen“.

**Zertifikat anzeigen:**

1. Klicken Sie in Outlook unter „Datei“ auf „Optionen“ und anschließend auf „Trust Center“. Wählen Sie „Einstellungen für das Trust Center...“.
1. Klicken Sie unter dem Reiter „E-Mail-Sicherheit“ bei „Verschlüsselte E-Mail-Nachrichten“ auf „Einstellungen“.
1. Wählen Sie die entsprechende Sicherheitsregel aus und klicken Sie auf „Auswählen...“.
1. Das Zertifikat kann anschließend unter „Zertifikateigenschaften anzeigen“ eingesehen werden.

### 3. Sperrung des persönlichen Zertifikats

Sollte das Zertifikat nicht mehr benötigt, kompromittiert oder der private Schlüssel nicht mehr sicher verwahrt sein, veranlassen Sie bitte eine Sperrung.

- **Per E-Mail:** Schreiben Sie eine E-Mail an **ca-admin@uni-mannheim.de** mit der Bitte um Sperrung und der Nennung des betroffenen Zertifikats.
- **Selbstveranlassung:** Alternativ können Sie die Sperrung selbst über den [HARICA Zertifikatsmanager](https://cm.harica.gr) veranlassen:
  1. Melden Sie sich mit Ihrer Uni-ID und Ihrem Passwort an.
  1. Wählen Sie im Bereich „Valid Certificates“ das Zertifikat aus, das gesperrt werden soll, und klicken Sie auf die drei Punkte, gefolgt von „Revoke“.
  1. Geben Sie einen Grund für die Sperrung an und bestätigen Sie.

## 👥 Gruppenzertifikat

### 1. Beantragung eines Gruppenzertifikats

Bitte senden Sie eine E-Mail an **ca-admin@uni-mannheim.de**, um die Möglichkeiten für ein Gruppenzertifikat zu besprechen.

### 2. Sperrung des Gruppenzertifikats

Sollte das Zertifikat nicht mehr benötigt, kompromittiert oder der private Schlüssel nicht mehr sicher verwahrt sein, veranlassen Sie bitte eine Sperrung.

- **Per E-Mail:** Schreiben Sie eine E-Mail an **ca-admin@uni-mannheim.de** mit der Bitte um Sperrung und der Nennung des betroffenen Zertifikats.
- **Selbstveranlassung:** Alternativ können Sie die Sperrung selbst über den [HARICA Zertifikatsmanager](https://cm.harica.gr) veranlassen (siehe Anleitung für die Sperrung des persönlichen Zertifikats).

## 🌐 Serverzertifikat

### 1. Beantragung eines Serverzertifikats

**Option A: Generierung des Certificate Request (CSR) lokal (Empfohlen für technische Nutzer)**
Führen Sie folgenden Befehl auf einem Windows- oder Linux-System mit installiertem „openssl“ aus. Bitte ersetzen Sie die fett markierten Attribute durch Ihre korrekten Werte:

```bash
openssl req -new -newkey rsa:4096 -sha512 -nodes -subj '/C=DE/ST=Baden-Wuerttemberg/O=Universitet Mannheim/CN=******FQDN******/emailAddress=**ihre-emailadresseuni-mannheim.de**' -keyout******FQDN******.key -out******FQDN******.csr
```

*Hinweis: Alternative Domainnamen können später im Antragsprozess ergänzt werden.*

**Option B: Online-Antrag über HARICA**

1. Klicken Sie auf diesen [Link](https://cm.harica.gr), um zur Beantragung bei HARICA zu gelangen.
1. Wählen Sie „Academic Login“ zur Anmeldung.
1. Klicken Sie auf „Your Institution“, suchen Sie „Mannheim“ und wählen Sie „University of Mannheim“. Melden Sie sich mit Ihrer Uni-ID und Ihrem Passwort an.
1. Wählen Sie auf der linken Seite den Menüpunkt „Server“.
1. Geben Sie den gewünschten Servernamen an und klicken Sie auf **Next**.
1. Wählen Sie als Zertifikatstyp „**For enterprises or organizations (OV)**“.
1. Bestätigen Sie Ihre Auswahl und anschließend die angezeigten Organisationsinformationen mit **Next**.
1. Überprüfen Sie die Angaben und stimmen Sie den „Terms of Use“ von HARICA zu, indem Sie einen Haken setzen und mit **Next** bestätigen.
1. **CSR-Generierung:** Wählen Sie, ob Sie den „Certificate Request“ automatisch durch den Browser erzeugen lassen oder einen zuvor generierten Request verwenden. Wählen Sie „Automatisch“:
   - Wählen Sie als Keysize „4096“ und legen Sie ein sicheres Passwort fest.
   - Bestätigen Sie das alleinige Wissen über dieses Passwort und klicken Sie auf „Generate Private Key, CSR, and submit order“.
1. Laden Sie den privaten Schlüssel für Ihr Zertifikat herunter und speichern Sie diesen auf Ihrem Computer.
1. Ihr Antrag wird von HARICA geprüft. Sie erhalten eine automatische E-Mail. Nach Erhalt können Sie das Zertifikat über das Dashboard des Zertifikatsmanagers herunterladen.

### 2. Sperrung des Serverzertifikats

Sollte das Zertifikat nicht mehr benötigt, kompromittiert oder der private Schlüssel nicht mehr sicher verwahrt sein, veranlassen Sie bitte eine Sperrung.

- **Per E-Mail:** Schreiben Sie eine E-Mail an **ca-admin@uni-mannheim.de** mit der Bitte um Sperrung und der Nennung des betroffenen Zertifikats.
- **Selbstveranlassung:** Alternativ können Sie die Sperrung selbst über den [HARICA Zertifikatsmanager](https://cm.harica.gr) veranlassen (siehe Anleitung für die Sperrung des persönlichen Zertifikats).

______________________________________________________________________

**Tipp zur Passwortsicherheit:** Speichern und verwalten Sie Ihre Passwörter sicher mit dem kostenfreien Passwort Manager [KeePass](https://www.uni-mannheim.de/informationssicherheit/infomaterial/anleitung-keepass/).
