---
description: >-
  Diese Dokumentation beschreibt den Prozess zur Anbindung eines ERP-Kunden an
  einen Partner über Yuneo Connect Direct. Ziel ist es, Partnern einen sicheren
  API-Zugriff auf ERP-Daten bereitzustellen.
---

# Aareon Connect Direct

### Überblick

Der Onboarding-Prozess besteht aus vier Schritten:

1. Umstellung auf Keycloak (Authentifizierung)
2. Erstellung von API-Benutzern
3. Backend-Konfiguration durch Yuneo
4. Bereitstellung der API-Zugangsdaten

### 1. Umstellung auf Keycloak (Verantwortlich: Kunde / Aareon)

Die Nutzung von Yuneo Connect Direct setzt zwingend die Verwendung von **Keycloak** voraus.

#### SaaS-Kunden

* Umstellung erfolgt eigenständig im System
* Navigation: _Optionen → Allgemein → Multifaktorauthentifizierung_
* Vorlaufzeit: ca. 14 Tage
* Detaillierte Informationen finden Sie außerdem in unserem HelpCenter unter dem Stichwort Keycloak.
* Die Umstellung kann bei Bedarf bereits vor Vertragsunterzeichnung durchgeführt werden, um Zeit zu sparen.

#### On-Premise (In-House) Kunden

* Die Umstellung muss durch die Aareon IT-Infrastruktur bzw. Aareon Consultants durchgeführt werden.
* Bitte erstellen Sie hierfür ein Zendesk-Ticket mit Adressierung an IT Infrastruktur und folgendem Inhalt:

„_Bitte um Umstellung auf das aktuelle Keycloak-Authentifizierungsverfahren für unser In-House-System. Die Umstellung ist Voraussetzung für die Connect Direct Anbindung an PLATZHALTER._“



### 2. Erstellung von API-Benutzern (Verantwortlich: Kunde)

Nach erfolgreicher Keycloak-Umstellung müssen API-Benutzer angelegt werden.

#### Grundprinzip

* Pro Partner wird **ein eigener Benutzer** benötigt

#### Benutzerdaten

* Benutzername / E-Mail: `svc_<partner_name>@aareon.com`
* Nachname: Partnername
* Option „Alle Mandanten“: aktivieren
* Benutzerrolle: partnerspezifische Rolle zuweisen

> Hinweis: Die Benutzerrollen lassen sich in Yuneo unter „Benutzerrollen“ einrichten und können anschließend dem Yuneo Benutzer zugeteilt werden. Bitte teilen Sie uns per Mail mit, sobald der Nutzer erstellt ist.

### 3. Backend-Konfiguration (Yuneo) (Verantwortlich: Aareon / Yuneo)

Dieser Schritt erfolgt vollständig durch Yuneo (Aareon).

* Einrichtung im API Gateway (Kong)
* Verknüpfung von Kunde, Benutzer und Partner

**Keine Aktion durch den Kunden erforderlich, wenn Schritte 1 + 2 vollständig erledigt wurden.**



### 4. Bereitstellung der Zugangsdaten (Verantwortlich: Aareon)

Nach Abschluss aller Schritte:

* Erstellung von API-Zugangsdaten pro Kunde/Partner
* Bereitstellung an den jeweiligen Partner durch Aareon

#### Hinweise

* Wichtig ist, dass der Benutzer genau die E-Mail-Adresse verwendet, wie in Schritt 2 angegeben.
* Sichere Weitergabe erforderlich

***

### Zusammenfassung

Für die erfolgreiche Anbindung sind folgende Schritte erforderlich:

1. Keycloak aktivieren
2. API-Benutzer je Partner anlegen
3. Yuneo konfiguriert das Backend
4. API-Zugangsdaten werden bereitgestellt







