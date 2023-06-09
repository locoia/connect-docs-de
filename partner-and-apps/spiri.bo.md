---
description: >-
  Die Mieter-App der Wohnungswirtschaft. Spiri.Bo digitalisiert Ihren
  Kundenservice.
---

# Spiri.Bo

## Übersicht

* **Kategorien**: [Mieterkommunikation](../kategorien/mieterkommunikation.md)
* **Use Cases**: [Stammdaten](spiri.bo.md#stammdaten)
* **Marketplace**: [Spiri.Bo](https://marketplace.aareon.com/de/listings/spiribo)
* **API Dokumentation**: [Link](https://api.spiri.bo/v1/docs/silo#tag/building)

## Beschreibung

Spiri.Bo ist ein PropTech-Unternehmen der meravis Immobiliengruppe. Spiri.Bo digitalisiert die Wohnungswirtschaft für Mieterservice der begeistert. Spiri.Bo's Kern-Produkt ist die Spiri.Bo Mieterapp als All-In-One-Lösung:

## Mit Spiri.Bo verbinden

1. Um einen Spiri.Bo-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Spiri.Bo API Zugansdaten**. Diese erhalten Sie folgendermaßen:
   1. Fordern Sie per Email an [dev+api-key@spiri.bo](mailto:dev+api-key@spiri.bo) mit dem Betreff "API-Key Aareon Connect" und Inhalt "Hallo, bitte sendet mir einen API-Key für Aareon Connect zu. Vielen Dank" den API Key an.&#x20;
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **Spiri.Bo Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren. Mehr Details dazu finden Sie hier[^1].

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](spiri.bo.md#stammdaten)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                           | Spiri.Bo      |
| ------------------------------------------------------------- | ------------- |
| [Gebäude](../entitaeten/gebaeude.md)                          | Gebäude       |
| [Verwaltungseinheiten](../entitaeten/verwaltungseinheiten.md) | Wohnungen     |
| [Mietverträge](../entitaeten/mietvertraege.md)                | Verträge      |
| [Mieter](../entitaeten/mieter.md)                             | Mieterbestand |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="151">Name</th><th width="487.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einem hinterlegten Nachnamen synchronisiert
* Es werden nur Stammdaten synchronisert, welche mit einem Mieter verknüpft sind
  * Beispiel: Ein Wohnung welche leer ist, wird nicht synchronisert

#### Wohnungstypen Mapping

Die im ERP hinterlegt Nutzungsart (des Mietvertrags) wird wie folgt auf die Wohnungstypen in Spiri.Bo gemappt:

| ERP                          | Spiri.Bo   |
| ---------------------------- | ---------- |
| Wohnraum                     | living     |
| Wohnung                      | living     |
| Praxis                       | commercial |
| Einzelhandel                 | commercial |
| Büro                         | commercial |
| Gastronomie                  | commercial |
| Pflegedienst                 | commercial |
| Werkstatt                    | commercial |
| Gewerbe                      | commercial |
| Produktion                   | commercial |
| Logistik                     | commercial |
| gewerbliche Nutzung          | commercial |
| Garagen                      | parking    |
| Stellplatz außen             | parking    |
| Carport                      | parking    |
| Tiefgarage                   | parking    |
| Fahrradraum                  | parking    |
| Hochgarage                   | parking    |
| Garage                       | parking    |
| Lager                        | storage    |
| _Alle anderen Nutzungsarten_ | other      |

{% hint style="info" %}
Da die Nutzungsart im ERP System frei definierbar ist, wird das Mapping laufend erweitert.
{% endhint %}

[^1]: (Link zu ERP overview)
