# DocuSign

{% hint style="warning" %}
[**Scrive**](scrive-technologie-partner.md) ist seit 2023 unser präferierter Technologiepartner und DocuSign wird nur für DocuSign Bestandskunden unterstützt.
{% endhint %}

## Aktivierung in Aareon Connect

Mit der Migration von der Digitalen Unterschrift zu Aareon Connect, wird die Verbindung zwischen WODIS Sigma/SAP Blue Eagle und DocuSign über Locoia hergestellt, statt wie bisher über einen API Service von Aareon selber.

Dies ermöglicht die Migration zu [scrive-technologie-partner.md](scrive-technologie-partner.md "mention"), wodurch wir Ihnen neue Funktionen anbieten können ([#vorteile-scrive](scrive-technologie-partner.md#vorteile-scrive "mention")).

Als **DocuSign Bestandskunde** können Sie bis auf weiteres weiterhin DocuSign für die Digitale Unterschrift nutzen und müssen einmalig folgende Schritte für die Migration durchführen.

Die Schritte und möglichen Einstellungen sind dabei auch in diesem Video zusammengefasst:

<figure><img src="../../../.gitbook/assets/image (2) (3).png" alt=""><figcaption><p><a href="https://www.loom.com/share/8531337f269c44f2a4cd506b84fd16a5?sid=2bc293ed-8459-42d8-8820-0fc2a1a12012">KLICKEN SIE HIER</a> - Dabei wird Loom in einem neuem Tab, außerhalb von Aareon Connect, geöffnet</p></figcaption></figure>

1. Öffnen Sie Aareon Connect in Ihrem ERP System ([mehr Details](../../../#aareon-connect-per-video-verstehen))
2. Gehen Sie auf **DocuSign**
3. Geben Sie bei der Integration **Digitale Unterschrift mit DocuSign** die Zugangsdaten für den DocuSign Nutzter ein (muss ein Admin Nutzer sein), den Sie für die Integration verwenden möchten
   1.  Wir empfehlen, dass Sie einen Admin Nutzer speziell für die Integration nutzen um Probleme bei z.B. Passwort Änderung eines regulären Nutzers zu vermeiden

       <figure><img src="../../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>
4. Klicken Sie auf **Autorisieren**
   1. Die Nutzerdaten werden direkt überprüft und bei falschen Informationen erhalten Sie eine Meldung mit weiteren Informationen
5.  _Optional:_ Suchen Sie nach dem DocuSign Account Namen den Sie verwenden wollen und suchen Sie den passenden Namen aus der Liste aus. Wenn Sie das Feld leer lassen wir der Standard Account verwendet.<br>

    <figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
6. Sie können weitere Einstellungen vornehmen:
   1. _Optional_: Geben Sie die Bezeichnung der von Ihnen genutzten (Alternativer) QES Identitätsüberprüfung an, mehr Details in [#nutzung-von-qes](umstellung-docusign-integration.md#nutzung-von-qes "mention")
   2. _Optional_: Geben Sie die Bezeichnung der von Ihnen genutzten SMS PIN Identitätsüberprüfung an, mehr Details in [#nutzung-von-sms-pin](umstellung-docusign-integration.md#nutzung-von-sms-pin "mention")
   3. _Optional_: Setzen Sie einen benutzerdefinierten E-Mail Betreff und/oder E-Mail Text, mehr Details in [#benutzerdefinierter-e-mail-betreff-und-text](umstellung-docusign-integration.md#benutzerdefinierter-e-mail-betreff-und-text "mention")
   4. _Optional_: Defineren Sie eine Signiergruppe für bestimmte Unterziechern, mehr Details in [#nutzung-von-signiergruppen](umstellung-docusign-integration.md#nutzung-von-signiergruppen "mention")
7. Die Integration ist nun aktiviert
8. Sie erhalten somit in den kommenden Stunden via E-Mail die nötigen Informationen um die Integration im ERP System fertig einzurichten
9. Folgen Sie den Anleitungen der jeweiligen ERPs für die weiteren Einrichtungsschritte (Scrive kann dabei mit DocuSign ersetzt werden)

### Nutzung von QES

Mehr Details zu [#qualifizierte-elektronische-unterschrift](../#qualifizierte-elektronische-unterschrift "mention") finden Sie im verlinkten Artikel.

Um QES mit DocuSign nutzen zu können müssen Sie eine entsprechende "Identitätsüberprüfung" in Ihrem DocuSign Account haben.\
[Mehr Details dazu finden Sie hier bei DocuSign direkt](https://support.docusign.com/s/document-item?language=de\&rsc_301=\&bundleId=pik1583277475390\&topicId=eya1583277454804.html&_LANG=dede).

Um diese integriert Nutzen zu können müssen Sie den genauen Namen im 6. Schritt (Anleitung oben) eingeben.\
Den genauen Namen können Sie bei DocuSign unter **Einstellungen** > **Identitätsüberprüfung** sehen, wo sie die passende Identitätsüberprüfung aus der Liste auswählen können und diese dann so markieren und kopieren können:

<figure><img src="../../../.gitbook/assets/Screenshot 2024-05-15 at 17.14.58.png" alt=""><figcaption></figcaption></figure>

#### QES Alternative Identitätsüberprüfung

Wenn Sie für bestimmte Unterzeichner eine alternative QES Identitätsüberprüfung nutzen wollen, können Sie diese unter **QES Alternative Identitätsüberprüfung** konfigurieren.

Geben Sie, wie bei der regulären QES Identitätsüberprüfung, den Namen der Identitätsüberprüfung ein und geben Sie unter **QES Alternative Identitätsüberprüfung - E-Mail Domain Filter** die E-Mail Domain als Filter für die Alternative QES Identitätsüberprüfung ein. Nur Unterzeichner mit dieser E-Mail Domain nutzen die alternative Identitätsüberprüfung, alle anderen Unterzeichner nutzen die reguläre QES Identitätsüberprüfung.

Die Einstellungen könnten z.B. so aussehen:

<figure><img src="../../../.gitbook/assets/image (2) (2).png" alt=""><figcaption><p>Beispielhafte QES Alternative Identitätsüberprüfung Einstellungen</p></figcaption></figure>

In dem Fall nutzen alle Unterzeichner die Identitätsüberprüfung **IDV Premier Selfie Ident**, _außer_ die Unterzeichner die in ihrer E-Mail **@wodis-wohnau.de** enthalten haben, diese nutzen **IDNow (Video Ident)**.

Dies kann z.B. nützlich sein, wenn Sie für Ihre internen Unterzeichner Video Ident nutzen wollen, da das Wallet länger gültig ist, aber Ihren Kunden den Komfort von Selfie Ident bieten wollen.

### Nutzung von SMS PIN

Um SMS PIN mit DocuSign nutzen zu können müssen Sie eine entsprechende "Identitätsüberprüfung" in Ihrem DocuSign Account haben.\
[Mehr Details dazu finden Sie hier bei DocuSign direkt](https://support.docusign.com/s/document-item?language=de\&rsc_301=\&bundleId=pik1583277475390\&topicId=eya1583277454804.html&_LANG=dede).

Um diese integriert Nutzen zu können müssen Sie den genauen Namen im 6. Schritt (Anleitung oben) eingeben.\
Den genauen Namen können Sie bei DocuSign unter **Einstellungen** > **Identitätsüberprüfung** sehen, wo sie die passende Identitätsüberprüfung aus der Liste auswählen können und diese dann so markieren und kopieren können:

<figure><img src="../../../.gitbook/assets/Screenshot 2024-05-15 at 17.14.58.png" alt=""><figcaption></figcaption></figure>

### Benutzerdefinierter E-Mail Betreff und Text

Sie können während der Aktivierung einen benutzerdefinierten E-Mail Betreff und/oder E-Mail Text setzen:

<figure><img src="../../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

Jeder Umschlag der über das ERP verschickt wird, wird diesen Betreff und/oder Text in der E-Mail von DocuSign haben und somit den Standard von DocuSign überschreiben.

{% hint style="info" %}
Der Betreff und Text kann keine Variablen enthalten und ist somit für jeden Umschlag und jeden Empfänger der E-Mail identisch.

Entsprechend sollte der Betreff und Text möglichst generisch sein, sodass diese für alle Situationen passen.
{% endhint %}

### Marken Nutzung

Wenn Sie in DocuSign eine Marke erstellt haben ([mehr Details](https://support.docusign.com/s/document-item?language=de\&bundleId=pik1583277475390\&topicId=lfr1583277366660.html&_LANG=dede)), können Sie die ID der Marke, die Sie für alle Umschläge nutzen wollen, die mit der Digitalen Signatur versendet werden, in der **Marken ID** Einstellung hinzufügen.

Die Marken ID finden Sie hier in DocuSign:

<figure><img src="../../../.gitbook/assets/Arc 2024-10-29 14.26.24.png" alt=""><figcaption><p>Marken-ID in DocuSign einsehen</p></figcaption></figure>

### Nutzung von Signiergruppen

Wenn Sie für bestimmte Unterzeichner aus dem ERP System eine Signiergruppe benutzen wollen, müssen Sie beide Felder ausfüllen:

*   **Signiergruppen-ID**: Diese finden Sie in den DocuSign Einstellungen unter **Benutzer und Gruppen** > **Signiergruppen** > **Signiergruppen-ID**<br>

    <figure><img src="../../../.gitbook/assets/Screenshot 2024-09-13 at 17.42.12.png" alt=""><figcaption></figcaption></figure>
* **Signiergruppe - E-Mail Domain Filter**: E-Mail Domain als Filter für die Signiergruppe. Nur Unterzeichner mit dieser E-Mail Domain werden durch die Signiergruppe ersetzt, alle anderen Unterzeichner werden wie im ERP System definiert zu dem Umschlag hinzugefügt.
