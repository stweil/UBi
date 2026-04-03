---
title: "Anleitung: Wie man den tatsächlichen Absender einer E-Mail mittels Header-Analyse in Outlook ermittelt"
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/it/instructions/microsoft-exchange/outlook-analyze-mail-header/
category: Benutzung
tags: ['Outlook', 'E-Mail', 'Header', 'Absender', 'Analyse', 'Anleitung', 'Microsoft Exchange']
language: de
---

# Den tatsächlichen Absender einer E-Mail bestimmen: Header-Analyse in Outlook

Diese Anleitung zeigt Ihnen, wie Sie den Header einer E-Mail in Outlook auslesen können, um festzustellen, wer der tatsächliche Absender der Nachricht ist.

### Schritt-für-Schritt-Anleitung

Folgen Sie diesen Schritten, um die notwendigen Informationen zu sammeln:

1. **E-Mail öffnen und Eigenschaften aufrufen:**

   - Öffnen Sie die betreffende E-Mail mit einem Doppelklick.
   - Klicken Sie links oben auf **„Datei“**.
   - Wählen Sie im sich öffnenden Menü **„Eigenschaften“**.

1. **Internetkopfzeilen kopieren:**

   - Markieren Sie den gesamten Text unter **„Internetkopfzeilen“** (Strg + A).
   - Kopieren Sie diesen Text (Strg + C).
   - Schließen Sie das Eigenschaften-Fenster.

1. **Header analysieren:**

   - Rufen Sie einen Webbrowser auf und navigieren Sie zu einer „Mail Header Analyse“- Webseite, wie zum Beispiel von Microsoft: [https://mha.azurewebsites.net/](https://mha.azurewebsites.net/).
   - Fügen Sie den kopierten Text in das Analysefeld ein.

1. **Ursprung des Senders prüfen:**

   - Suchen Sie in den Ergebnissen nach dem Eintrag **„Hop“** in der Spalte **„Submitting Host“**.
   - Dieser Eintrag zeigt den Ursprung der E-Mail und den absendenden Server.
   - **Ergebnisinterpretation:** Wenn die angezeigte Adresse auf `[…].uni-mannheim.de` endet, wurde die E-Mail von den Servern der Universität Mannheim versendet.
