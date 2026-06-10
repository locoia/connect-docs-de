# Wodis Yuneo

## Initiale Einrichtung

### Lizenzen Einlesen

Lesen Sie wie [hier beschrieben](../../../erps/wodis-yuneo.md#aareon-connect-in-wodis-yuneo-aktivieren-lizenzen-einlesen) die aktuellen Lizenzen ein.

### Verknüpfung zwischen WODIS Yuneo und Aareon Connect herstellen

Voraussetzung ist, dass die Setup Einstellungen in folgenden Bereichen erfolgt sind:\
Verbindung zu Scrive wurde über Aareon Connect hergestellt

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXe8i9MXPOt6KMA48XlLmzYJVdrY-em46UkzI9gJAR00Ys5r98OL-Z8pjaUBnaNb0Q15oOX4HXW0uOY8xmaVfKV0QXTWJ6ahFhnH_l_Suva8WsSOCzFs21J8H44Ue9ktAPXyJCjkrJzkpwsCyvwa3WY?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXfmXq7dRuKzrTd9nx1ATHlcgFUuq7HQpmUlzQIbUQtmxtdUNJjvNoPfttFbTnkU8fO8Keyff0BYyQKSy-zaf0M2mDr9yuImeTrT8gS9jEdNQZ6Zj4EE4Calnku8IjgFOER954JRaqFcTBaM1-dfjw?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>

Nachdem Sie die Digitale Unterschrift wie in [#aktivierung-in-aareon-connect](../technologie-partner/scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") beschrieben aktiviert haben muss zuletzt die Verknüpfung zwischen WODIS Yuneo und Aareon Connect eingerichtet werden.

1.  Gehen Sie auf **Systemeinrichtung** > **Optionen** > **Optionen Allgemein** > **Digitale Unterschrift**<br>

    <figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXc5HodqMSsSWfA_eB5XH05FTGrtun6LYv-JG0s6BNPrqOtyJV8xM96TgPDN5QTwA-Ko03pIah_AxP7t1Y1Cqx5r8gFOcKjLT3JT7frYVB4abT_P-TgIHHBEBZLl9ppch1GIHuBuLQI1NGizkCY9_gE?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>
2. Setzen Sie **Digitale Unterschrift** auf **Konfigurieren**
3. Wählen Sie **Scrive** bei **Technologiepartner** aus
4. Tragen sie den **Benutzernamen**, **Passwort** und **Integrations ID** ein, welche Sie nach der [#aktivierung-in-aareon-connect](../technologie-partner/scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") erhalten haben
5. Unter der Integrations-ID können Sie bei **Vorbelegung Versandreihenfolge** die standard **Reihenfolge** nach Unterzeichner Gruppe (Intern und Extern) bestimmen, in der die Vertragsparteien unterzeichnen sollen.\
   Bei **Versand pro Gruppe** können Sie bestimmen, ob alle Unterzeichner der jeweiligen Gruppe **Gleichzeitig** oder basierend auf der Reihenfolge in der Aktivität unterzeichnen sollen.\
   Diese standard Reihenfolge können Sie, wenn gewünscht, in jedem einzelnem Vorgang überschreiben.
6. Klicken Sie auf **Speichern**

<figure><img src="../../../.gitbook/assets/image (3) (2) (1).png" alt=""><figcaption></figcaption></figure>

### Arbeitsaufträge Einrichten

Nun müssen noch die passenden Arbeitsaufträge angelegt werden:

1.  Gehen Sie auf **Systemeinrichtung** > **Organisation und Datenmanagement** > **Planung Arbeitsaufträge**<br>

    <figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXc-lfff8owMA0C_S7HbCq7sAGkSnhfQni_hkYCVhMt5-8F3gHwFBOv3y4j4lQ7wJPF6HJhrOnwPaiAINATtwc13Um9c2VLrT4zYBdWKwRlGnjcYiWkn4VQzcAyToKPTkWolQk4bMkCBUhoR26RfqHc?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>
2. Klicken Sie oben links auf **Neu anlegen**
3.  Suchen Sie im **Typ** Feld nach **Digitale Unterschrift - Dokumente versenden**<br>

    <figure><img src="../../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>
4. Geben Sie dem Arbeitsauftrag einen Namen
5. Stellen Sie einen Zeitraum ein. Wir empfehlen den Job mehrmals täglich ausführen zu lassen (z.B. alle 2 Stunden)
6. Klicken Sie auf **Speichern**
7. Wiederholen Sie die Schritte 2-6 für den Arbeitsauftrags-Typ **Digitale Unterschrift - Dokumente empfangen**

<figure><img src="../../../.gitbook/assets/image (33) (1).png" alt=""><figcaption></figcaption></figure>

## Einmalige Einrichtung je Dokumentvorlage

Die folgenden Schritte müssen Sie nur einmalig je Dokumentvorlage durchführen. Durch diese Schritte fügen Sie so genannte "Anchor Tags" zu Ihren Dokumentvorlagen hinzu.

Die Anchor Tags werden im Unterzeichnungsvorgang den passenden Unterzeichnern zugeordnet, sodass diese an den von Ihnen vorgesehenen Stellen Unterschreiben oder Felder ausfüllen.

1. Gehen Sie auf **Vorlagenverwaltung** > **Erstellung einer Serienbriefvorlage**
2. Klicken Sie, in der Vorlage, auf **Vorlage bearbeiten**
   1. Somit öffnet sich die Vorlage in Wodis Text
3. Gehen Sie im oberem Menü auf den Reiter **Seriendruck**
4. Klicken Sie im Dokument auf die Stelle, wo sie ein Anchor Tag einfügen wollen
5. Klicken Sie auf den, unter dem oberem Menü, Knopf **Feld erstellen**
6. Konfigurieren Sie das Feld und bestätigen die Konfiguration mit einem Klick auf **Einfügen**
   1. Es stehen folgende Konfigurationsmöglichkeiten zur Verfügung:
      1. Unterzeichner
         1. Intern _- Unternehmensinternem (z.B. Sachbearbeiter_
         2. Extern _- Externe Person (z.B. Mieter)_
      2. Unterzeichner Nr. _- Zuordnung der Unterzeichner innerhalb der jeweiligen Internen bzw. Externen Unterzeichner_
      3. Feldart
         1. Unterschrift
         2. Unterschriftsdatum _- Das aktuelle Datum_
         3. Datum
         4. Name
         5. Checkbox
         6. Text
         7. Email
         8. Initialen _- Die jeweils ersten Buchstaben des Vor- und Nachnamens (z.B. bei Erika Mustermann: EM)_
      4. Feld Nr. - _Zuordnung der Felder innerhalb der jeweiligen Feldarten_
      5. Feldeigenschaft
         1. Pflicht _- Das Feld muss zwingend ausgefüllt werden_
         2. Optional _- Das Feld kann ausgefüllt werden_
7. Nachdem Sie alle Anchor Tags eingefügt haben, gelangen Sie zurück in die Vorlagenverwaltung mit Klick auf **Datei**
8. Scrollen Sie zum Bereich **Archivierung**
9. Klicken Sie auf **Archivieren**
   1. _Hintergrund_: Ohne Archivierung des Dokuments ist die Digitale Unterschrift nicht möglich
10. Klicken Sie oben rechts auf **Speichern**

## Prozess je Dokument

### Einrichten und Versenden von Dokumenten

Nachdem Sie die [#einmalige-einrichtung-je-dokumentvorlage](wodis-yuneo.md#einmalige-einrichtung-je-dokumentvorlage "mention") vorgenommen haben, können Sie Dokumente ganz einfach, als Teil des regulären Schriftverkehr-Prozess, digital unterschreiben lassen.

Bei dem Schriftverkehr Erstellungs-Prozess müssen Sie dafür folgende Dinge beachten:

1. Sie können nur Dokumentvorlagen verwenden, welche Sie wie in [#einmalige-einrichtung-je-dokumentvorlage](wodis-yuneo.md#einmalige-einrichtung-je-dokumentvorlage "mention") beschrieben eingerichtet haben
2. Bei der Schriftverkehrs-Aktivität in der Sektion **Aktivität - Allgemein** folgende Einstellungen vornehmen:
   1. Systemtyp: Aufgabe
   2.  Aktivitätstyp: Digital Unterschreiben<br>

       <figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXeq_Qli9lQDkjYA7hk-MyaI8l_CFEodcsNQkU8o5o3Y__UiVCaM7OQz4Ftq8n0u16e2DSWFFNqji_vC8QNG7iexwgwYARwpqBUFW_mqxbehaxkDZgiazR553t2NiU7wHp2EodXhgyhSoLB7oI5N7uY?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>
   3.  Die weiteren Felder können Sie individuell ausfüllen

       <figure><img src="../../../.gitbook/assets/image (7).png" alt="" width="563"><figcaption></figcaption></figure>
3. Fügen Sie bei der Sektion **Bearbeitet von** mindestens einen Benutzer hinzu
4. In der Sektion **Digitale Signatur** können Sie alle Unterzeichner hinzufügen
   1. Bei **Intern** wählen Sie einen oder mehrere Yuneo Benutzer (Unternehmensinterne Person) aus
   2. Bei **Extern** wählen Sie einen oder mehrere Kontakt(e) aus (externe Personen)
5. In dem Feld **Reihenfolge** können Sie auswählen, ob Sie Ihre Auswahl aus den Standardeinstellungen übernehmen wollen oder eine andere Reihenfolge bestimmen.

<figure><img src="../../../.gitbook/assets/MicrosoftTeams-image.png" alt=""><figcaption></figcaption></figure>

***

#### **Schritte zur Erstellung des Schriftverkehrs:**

**Erstellen Sie den Schriftverkehr**

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXdHqRk_RbNY-wCzGxtZs0Fl4rJfPv0-5w-dgCaOwBzCidE53VqRXXFrJP5FzJ9-5kIwDqxQidVDe7hDH6aOTbO_anK0qGXFnwfsk86HJCzYsVDsVRbO_kK87Nu_S4TKPXsZnTsg5P8YQk3uHQ900zA?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p><strong>Schriftverkehr erstellen</strong></p></figcaption></figure>

**Wählen Sie das gewünschte Schriftstück aus**

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXewYaWbvj_dADddgc_qW4xXkrud6rwq3aqjIGypjrmZS7_GcKMpr5HGH3EKNI5FOJRt2MrDcyqg82lGZ2Q-G8TfwPZg-DyyDY2p69ixxk44sQce1VbwzQ40GUa4gwgIKjgNuoPVqxWbPhvYHy--G80?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption></figcaption></figure>

Möchten Sie das Schriftstück später bearbeiten achten Sie darauf, dass die Option **Zur Anpassung bereitstellen** gewählt ist.

Möchten Sie das Schriftstück sofort archivieren, wählen Sie die Option **Direkt verarbeiten**.

Klicken Sie auf **Schriftverkehr erstellen**

Über die Arbeitsaufträge können Sie nun das Schriftstück auswählen.

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXcaGSCG0MRTAlc_P0Z21ozVELWszIGJk6lQ381quVv86TrroPl7HvEjxhmNIeKIporuOE6s5f7W9Ddjss5V_agqXIWPMbwYZKpYA2LZtgXpVcZS7jE7YXqQrqrpJv5Hf-y4Rnyp-Q1xCqWcMnCLEfo?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Arbeitsaufträge</p></figcaption></figure>

Klicken Sie das Schriftstück an und wählen Sie **Statusmonitor öffnen**

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXeB1Bh2dXikF3k6Gay28R5_gqmYSQnPfRNQe5MuT5gejnqiMuh20WTGFbJIFTw-MDfrT2BCb3Ez1WMIOQPF9PrOaw75ERzdo21AfQcUPcP9LKl3CVd0q37Txzj-csjnqD7z9MrGU9TMQJoCIm4j358?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Statusmonitor öffnen</p></figcaption></figure>

Markieren Sie das Dokument und klicken **Dokument anzeigen**

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXdesTu9RF-8Fpjpv9b3SbZ0ErHRHC5WlVXGZNSkzjLEnA9gQRX5XxeMbXsmnLDviJk-5zndFBJMsAbmwbqZatCUBtRCyYHrNel3QO1Mjs3xjLgmjqply_bmIJuuJd906Cma_oSYKq5IKFzsEO73KJw?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Dokument anzeigen</p></figcaption></figure>

Jetzt können Sie das Dokument bearbeiten.

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXezd7eW2UnJNqIieaSp32y0f45cCUfJ_jG2qIbAjD64nos66jblzDIWHtQghurTCjIaTWfHn7WxDZ3_S75srhnSZ81rjaVaWYoi8JYHRXdH4ojgP9ShR_bQZc8aBOmiqcu2fRITR0wX8fOMPdNwusc?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Das Dokument</p></figcaption></figure>

Aus dem Statusmonitor heraus können Sie nun **YuStart** > **Archivierung** und Versand wählen.

Wählen Sie das richtige Archiv aus und klicken anschließend auf **Verarbeitung durchführen**

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXdDYrvmYNhY2uykaLLMymTYonB5Yi77VuZVFQSqhXcmlNQgp4yJ3mKvBOEbXfTfpJXwtI__cyNuL8KfpnVvQImkamqLfb_TNlC9NNEewEKm1pR8ZSlu1bh7HmUenq2CiYmkGTah1J-ka8vTNaF2DYk?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Verarbeitung durchführen</p></figcaption></figure>

#### Vor-Ort-Unterschrift

Um die Vor-Ort-Unterschrift zu nutzen, müssen diese drei Schritte befolgt werden:

1. Klicken Sie bei **Vor-Ort-Unterschrift** auf **Ermöglichen**
2. Tragen Sie eine E-Mail Adresse in dem Feld **E-Mail Adresse für Vor-Ort-Unterschrift** ein
3. Klicken Sie in die Checkbox **Vor Ort unterschreiben** für die Unterzeichner die vor Ort unterschreiben sollen

<figure><img src="../../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

### Empfangen und Sichten von unterschriebenen Dokumenten

Yuneo holt sich regelmäßig (Standard: alle 30 Minuten) den aktuellen Stand aller Dokumente.\
Die Einstellungen dafür sind wie in [#initiale-einrichtung](wodis-yuneo.md#initiale-einrichtung "mention") beschrieben hinterlegt.

1. Im Yuneo [**Cockpit**](wodis-yuneo.md#cockpit) können Sie den Status aller Digitalen Unterschrifts-Dokumente einsehen
2. Durch Klick auf einer dort angezeigten Aktivität sehen Sie die Details der Aktivität, das unterschriebene Dokument, das Unterschriftszertifikat und weitere Informationen

Zusätzlich können Sie sich einen Filter in der Aktivitäten Übersicht erstellen, sodass Sie den jeweiligen Unterzeichnungsstatus auf einen Blick sehen können:

<figure><img src="../../../.gitbook/assets/Microsoft Teams (work or school) 2025-04-03 14.01.25.png" alt=""><figcaption><p>Filtererstellung</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Aktivitäten Übersicht mit Unterzeichnungsstatus</p></figcaption></figure>

### Cockpit

Sie können den Status der digitalen Unterschrift im Cockpit verfolgen.

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXdIn-QqU4WhUY91CM94QVUXEwjhrSUCiICgM_Q_J1uZ53GXxObaLF50LxBnp4GdZoW9U8Du7jZVXUhI033EpSVoMaW87XXeQc_cgf6lqTU--8ByIa6jtc7VWfP2E5tIkpbLHZz5iwQ89y3swjdXz9s?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Cockpit</p></figcaption></figure>

## Versandprotokolle

Die Versandprotokolle geben Ihnen Auskunft, ob der Arbeitsauftrag erfolgreich war und wie viele Unterzeichner sowie Dokumente beteiligt sind.

Bei Störungen können Sie unter Arbeitsaufträge genauere Informationen über die Art des Fehlers erhalten.

<figure><img src="https://lh7-qw.googleusercontent.com/docsz/AD_4nXfBXOBT0wTtkLoFzhrX5T43DZR-eM1QCaZvEXfIuSpIFt7fFBSnF-K5i1qowaV4LSvtjqlDlD1idbIcS4_6AvwfNOf3MHmUyg1bEatmUVA0eVOufla4tTjE4afNI4k6F0BwtcLNx6sZoT0rNnplGME?key=8asTqBcXRFcgrm0oY7urdZPd" alt=""><figcaption><p>Versandprotokolle</p></figcaption></figure>

<br>
