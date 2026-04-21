---
description: >-
  Diese Dokumentation beschreibt den Prozess zur Anbindung eines ERP-Kunden an
  einen Partner über Yuneo Connect Direct. Ziel ist es, Partnern einen sicheren
  API-Zugriff auf ERP-Daten bereitzustellen.
---

# Aareon Connect Direct

## Überblick

Aareon Connect Direct ermöglicht Partnern einen sicheren API-Zugriff auf ERP-Daten.

Das Onboarding umfasst vier Schritte:

1. Keycloak aktivieren
2. API-Benutzer anlegen
3. Backend konfigurieren
4. Zugangsdaten bereitstellen

{% hint style="info" %}
Pro Partner wird ein eigener API-Benutzer benötigt.
{% endhint %}

### Ablauf

{% stepper %}
{% step %}
### 1. Keycloak aktivieren

**Verantwortlich:** Kunde / Aareon

Die Nutzung von Aareon Connect Direct setzt **Keycloak** voraus.

#### SaaS-Kunden

* Die Umstellung erfolgt direkt im System.
* Navigation: **Optionen → Allgemein → Multifaktorauthentifizierung**
* Planen Sie etwa 14 Tage Vorlauf ein.
* Die Umstellung kann auch vor Vertragsunterzeichnung erfolgen.

#### On-Premise-Kunden

* Die Umstellung erfolgt durch Aareon IT Infrastruktur oder Aareon Consultants.
* Erstellen Sie dafür ein Zendesk-Ticket an **IT Infrastruktur**.

Verwenden Sie dabei diesen Text:

> Bitte um Umstellung auf das aktuelle Keycloak-Authentifizierungsverfahren für unser In-House-System. Die Umstellung ist Voraussetzung für die Connect Direct Anbindung an **\[Partnername]**.
{% endstep %}

{% step %}
### 2. API-Benutzer anlegen

**Verantwortlich:** Kunde

Legen Sie nach der Keycloak-Umstellung den API-Benutzer an.

#### Benutzerdaten

* Benutzername / E-Mail: `svc_<partner_name>@aareon.com`
* Nachname: Partnername
* Option **Alle Mandanten** aktivieren
* Partnerspezifische Benutzerrolle zuweisen

{% hint style="info" %}
Die Benutzerrolle richten Sie in Yuneo unter **„Benutzerrollen“** ein. Anschließend weisen Sie diese Rolle dem entsprechenden Yuneo-Benutzer zu.

Sobald der Benutzer angelegt wurde, informieren Sie uns bitte per E-Mail. Eine kurze Nachricht an **connect@aareon-dach.zendesk.com** mit dem Benutzernamen sowie dem Hinweis, dass der Benutzer erfolgreich erstellt wurde, ist hierfür ausreichend.
{% endhint %}
{% endstep %}

{% step %}
### 3. Backend konfigurieren

**Verantwortlich:** Aareon / Yuneo

Dieser Schritt erfolgt vollständig durch Aareon.

* Einrichtung im API Gateway
* Verknüpfung von Kunde, Benutzer und Partner

Wenn Schritt 1 und 2 abgeschlossen sind, ist hier keine Aktion des Kunden nötig.
{% endstep %}

{% step %}
### 4. Zugangsdaten bereitstellen

**Verantwortlich:** Aareon

Nach Abschluss aller Schritte erstellt Aareon die API-Zugangsdaten je Kunde und Partner.

Die Zugangsdaten werden anschließend an den jeweiligen Partner übermittelt.

#### Wichtig

* Verwenden Sie exakt die E-Mail-Adresse aus Schritt 2.
* Übermitteln Sie Zugangsdaten nur auf sicherem Weg.
{% endstep %}
{% endstepper %}

### Checkliste

Die Anbindung ist abgeschlossen, wenn diese Punkte erfüllt sind:

* Keycloak ist aktiviert.
* Der API-Benutzer ist je Partner angelegt.
* Das Backend ist durch Aareon konfiguriert.
* Die Zugangsdaten wurden bereitgestellt.

