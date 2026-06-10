---
description: >-
  Optimieren der Immobilienkommunikation durch einfach integrierbare,
  mehrsprachige K.I.-Chat- und Voicebots von Bots4You, datenschutzkonform und
  benutzerfreundlich.
---

# Bots4You

## Übersicht

* **Kategorien**: [Mieterkommunikation](../kategorien/mieterkommunikation.md), [Reporting](../kategorien/reporting.md), [Dokumentenmanagement](../kategorien/dokumentenmanagement.md)
* **Use Cases**: [Stammdaten](../use-cases/allgemein/stammdaten.md), [Tickets](../use-cases/crm/tickets.md)
* **Marketplace**: [Bots4You](https://marketplace.aareon.com/de/listings/bots4you)

## Beschreibung

Bots4You bietet K.I.-gestützte Chatbots und Voicebots, die speziell für den Einsatz im Immobilienmanagement entwickelt wurden. Diese Technologie zielt darauf ab, die Kommunikation zwischen Immobilienunternehmen und ihren Kunden oder Mitarbeitern zu verbessern. Die Plattform von Bots4You, die keine Programmierkenntnisse erfordert, ermöglicht es Nutzern, K.I.-Lösungen einfach zu implementieren. Die Bots sind mehrsprachig, anpassbar und können auf verschiedenen Plattformen wie Websites oder als Telefon-Assistenten eingesetzt werden, wobei sie stets datenschutzkonforme Richtlinien befolgen. Durch die Integration mit internen Systemen der Unternehmen können die Bots effektiv Informationen austauschen, wodurch Prozesse optimiert und die Kundenzufriedenheit potenziell gesteigert wird. Bots4You bietet somit eine Vielzahl von Anwendungsmöglichkeiten für die interne und externe Kommunikation im Immobiliensektor. Bei weiteren Fragen zur Anbindung melden Sie sich direkt bei Bots4You.

## Server und Hosting

Die [KI-basierte virtuelle Assistentin Neela](https://einfach.aareon.de/CRM-Portal-App.727021.html), die mit dem Aareon CRM. erworben wird, ist im Aareon-Rechenzentrum gehostet (die Server betrieben).

Andere Produkte wie der VoiceBot oder Omni-Channel von Bots4You werden primär in der Telekom Cloud in Deutschland, aber auch bei Stack IT gehostet.

## Mit Bots4You verbinden

1. Um einen Bots4You-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Bots4You API Zugangsdaten**. Diese sind folgendermaßen:
   1. **Username**
   2. **Passwort**

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](https://connect-docs-de.locoia.com/use-cases/stammdaten)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1fLwCGcttemtlDpznO3O00352cZZ5SPJXBPv6IRWQ6Bk/edit?gid=1022321755#gid=1022321755)

Die Stammdaten werden nur vom ERP zu Bots4You übertragen.

#### Entitäten

| ERP                                                                         | Bots4You |
| --------------------------------------------------------------------------- | -------- |
| [Mieter](https://connect-docs-de.locoia.com/entitaeten/mieter)              | Mieter   |
| [Mietverträge](https://connect-docs-de.locoia.com/entitaeten/mietvertraege) | Mieter   |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

### 2. Tickets

#### Übersicht

* [Allgemeine Informationen](../use-cases/crm/tickets.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1fLwCGcttemtlDpznO3O00352cZZ5SPJXBPv6IRWQ6Bk/edit?gid=1996564035#gid=1996564035)

Die Ticket Kategorien werden nur vom ERP zu Bots4You übertragen.

Tickets die in Bots4You erstellt werden, werden an das ERP übertragen und der Status dieser Tickets wird zurück vom ERP an Bots4You übertragen.\
Tickets die im ERP erstellt wurden, werden nicht an Bots4You übertragen.

#### Entitäten

| ERP               | Bots4You          |
| ----------------- | ----------------- |
| Tickets           | Tickets           |
| Ticket Kategorien | Ticket Kategorien |

## Best Practices

### In der Vorbereitung

* Nur **ein Projektleiter** aus der Abteilung für Mieterkommunikation kann **bis zu 80 % des gesamten Go-Live-Prozesses eigenständig** steuern. Es benötigt keine große Projektteams oder lange Implementierungszeiten.
* **Beginnen Sie** schrittweise **mit einem bestimmten Anwendungsfall**, z. B. der Bearbeitung von Schadensmeldungen außerhalb der Bürozeiten, um sich an die Technologie und den Prozess zu gewöhnen.
* Verlassen Sie sich auf die **umfangreiche FAQ- und Dialogaufbau-Erfahrung** etablierter Player, die Anpassungen gehen schneller als bei 0 anzufangen. Somit können Sie mit wenig Aufwand schnell live gehen.
* Entscheiden Sie intern, die **gewollte Kommunikationssprache**. Wollen Sie nur auf Deutsch kommunizieren oder wollen Sie beispielsweise den VoiceBot auch in mehreren Sprachen anbieten. Ein **Großteil der WoWi-Kunden** entscheidet sich **nur Deutsch**, um bei den Mietern nicht die Erwartung zu wecken, dass mehrere Sprachen im Team gesprochen werden können.
* Machen Sie sich bewusst, dass **sich Mieter an den neuen Prozess** und die Stimme des virtuellen Agenten **gewöhnen** müssen, kommunizieren Sie die Änderungen weiterhin aktiv und stellen Sie sicher, dass die Mieter ständig informiert sind. Die Anliegen der Mieter können somit deutlich schneller bearbeitet werden.

### Während der Implementierung

* **Kanalisieren Sie alle Einträge über einen Bot** (z. B. eine Nummer für alle Schadensmeldungen oder eine zentrale E-Mail-Adresse). Dies kostet am Anfang möglicherweise etwas Zeit, automatisiert jedoch den Prozess und schafft hohe Synergien. Nutzung von Sammel-Postfächern und weg von einzelnen Mitarbeiter-Emails
* Ermitteln Sie gemeinsam mit Ihrem KI-Partner **alle möglichen Dialogsituationen**, sodass, wenn beispielsweise der VoiceBot den Anliegen nicht erkennen kann, ein klarer Prozess festgelegt wird. Ein klarer Fallback-Szenerio über alle Kommunikationskanäle hinweg.
* Verlassen Sie sich auf eine **eindeutige Authentifizierungsmethode** (z. B. Mieternummer oder PLZ und Hausnummer) und schulen Sie Ihre Mieter, indem Sie ihnen beispielsweise empfehlen, die Mieternummer in ihren Kontaktdaten zu speichern.

### In der kontinuierlichen Optimierung

* Legen Sie intern klar fest, wer dafür verantwortlich ist, **gemeinsam mit dem Partner die KI kontinuierlich zu optimieren** (Dialoge, FAQs, etc.). Es ist eine gemeinsame Arbeit, die Leistung der verschiedenen Bots weiterzuentwickeln.
* **Kommunizieren Sie intern** klar und deutlich zwischen den verschiedenen Teams, welche **neuen Prozesse vom KI-Bot abgedeckt werden** und wie sich dieser positiv auf die Kollegen auswirkt
* Hinweise an Ihre Mieter um die virtuellen Assistenten zu nutzen:
  * im **Impressum** der Webseite und auf der „Kontakt“-Webseite
  * in der normalen **Telefonanlagen-Schleife** (während der Öffnungszeiten), „über unseren virtuellen Telefon-Assistenten Neela können sie fast alle Anliegen rund um die Uhr an uns übermitteln oder bekommen sofort eine Antwort auf Ihre Frage.“
  * ein “wie funktioniert unser Bot“ **Video**, dass sich Mieter ansehen können
  * Newsletter **Rundmail**
  * Hinweis im **CRM-Portal**

## Sonstiges

### Voicebot: Fragen und Schritte zur Vorbereitung

* Nennen Sie uns bitte einen Kontakt des Anbieters Ihrer Telefonanlage und den Namen der Anbieterfirma?
* Wie lassen sie heute Anrufer sich authentifizieren?
* In welche Sprachen lassen Sie rechtsverbindliche Aussagen am Telefon zu?
* Wer reguliert Schäden - intern vs. extern?
* Sind Sie selbst als Verwalter aktiv oder haben Sie Unterverwalter?



### FAQs



**Wo stehen die Server?**\
Europa, DSGVO-Konform.<br>

**Wie sind die Authentifizierungsmöglichkeiten?**

Klassische Authentifizierung über Mietvertragsnummer sowie andere gewünschte Parameter (individuell einstellbar). <br>

**Wie kann ich eine Telefonanlage für den VoiceBot verbinden?**

Es gibt folgende Möglichkeiten:

1. Weiterleitung einer Rufnummer and die Rufnummer des Bots. Diese wird von Bots4You eingerichtet.
2. Man kann zu verschiedenen Telefonzeiten verschiedene Aktionen durchführen, wobei die  Möglichkeiten von der Telefonanlage abhängt.

**Welche Telefonnummern kann man hinter den VoiceBot schalten?**

1. Mit SIP Trunk kann man die Nummer einer Telefonanlage direkt nutzen.
2. Ansonsten wird eine Nummer von Bots4You vorgegeben auf diese üblicherweise weitergeleitet.

**EmailBot: Wie kann dieser mit Outlook verknüpft werden?**

Die Outlook Microsoft Azure App muss verwenden werden.

Neben dem Email-Bot kann man dann zusätzlich selbst schreiben auf z.B. einem Sammelpostfach. Allerdings wird Bots4You die einkommenden E-Mails auslesen und darauf direkt reagieren.



**Erfolgt eine Aufzeichnung der Telefonate oder wird nur transkribiert?**\
Es wird im Standard nur transkribiert.



**Kann ein Telefonanlage schon vorab Anrufer authentifizieren und diese Identifizierung weitergeben an den Voicebot?**

Ja, der einfachste Weg ist, wenn die Telefonanlage an den Voicebot anruft und dabei in Abhängigkeit des Authentifizierungsstatus die Rufnummer in der Weiterleitung mitschickt, wenn der Anrufer nicht authentifiziert ist und die Mietvertragsnummer, wenn der Anrufer authentifiziert ist.\
<br>

**Verlängert sich die Dauer eines Telefonast des Voicebots, wenn dieser den Mieter identifizieren soll?**\
Ja, die Identifizierung kostet einige Sekunden.



**Angenommen in der Telefonwarteschleife befinden sich 5 Wartende: Kann der Voicebot alle Mietenden gleichzeitig bedienen?**\
&#x20;Ja, es können gleichzeitig verschiedne Anrufer weitergeleitet werden.



**Was passiert, wenn der Voicebot ein Anliegen nicht versteht?**\
Das kann im Dialog-Builder definiert werden. Z.B. kann eine Rückrufbitte eingestellt werden.



**Müssen Audio-Dateien gelöscht werden?**\
Nein, es werden keine Audio-Dateien aufgezeichnet. Daher muss nichts gelöscht werden.



**Kann die anrufende Telefonnummer im ERP aktualisiert werden, wenn unter der legitimierten Vertragsnummer noch eine alte Telefonnummer hinterlegt ist?**\
Nein, nicht im Standard. Das wäre eine zusätzlich zu beauftragende Zusatzfunktion.
