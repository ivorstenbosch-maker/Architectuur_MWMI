# AGENTS.md — instructies voor het MijnWerk/MijnInburgering Slidev-project

## Werkwijze: eerst voorstellen, nooit zelfstandig aanpassen

- Begin iedere opdracht met het bekijken van de relevante projectbestanden.
- Als de gebruiker vraagt om de presentatie te beoordelen of te verbeteren, maak dan eerst een analyse en een concreet verbeterplan.
- Wijzig geen bestanden voordat de gebruiker expliciet akkoord geeft op de voorgestelde wijzigingen.
- Voer na akkoord alleen de afgesproken wijzigingen uit.
- Beperk wijzigingen tot de bestanden en slides die voor de opdracht nodig zijn.
- Meld na iedere wijziging precies welke bestanden en slides zijn aangepast.
- Benoem eventuele onzekerheden of technische beperkingen; verzin geen projectstructuur of componenten.

## Inhoudelijke uitgangspunten

Gebruik de door de gebruiker aangeleverde informatie als leidend. Verander de betekenis of onderlinge verantwoordelijkheden van componenten niet.

- **MijnPlan** is de werknemersinteractie voor profiel, plan, doelen/subdoelen en evaluatie. Het ondersteunt gesprekken en evaluaties. Het is zelfstandig en losjes gekoppeld en gebruikt GZAC voor proces- en zaakafhandeling.
- **OpenPlan** is de relationele registratie voor plannen, doelen, subdoelen en evaluaties. Het configureert de Utrechtse dienstverlening voor Werk en Inburgering.
- **OpenProduct** registreert aanbod, instrumenten en voorzieningen van ketenpartners. Productspecifieke workflows en beslisregels worden daar ingericht. Medewerkers werken niet in de OpenProduct-interface; OpenProduct is geen casusregie-interface.
- **Domeinregistraties** bevatten domeinspecifieke gegevens, bijvoorbeeld opleidings- en taalniveaus voor Werk en gegevens voor Inburgering.
- **OpenKlant** bevat gegevens over inwoners en ketenpartners, adressen en contactmomenten.
- **OpenZaak** ondersteunt de onderdelen van zaakregistratie die in een zaak passen.
- **VTB** ondersteunt verzoeken, taken en berichten. Taken kunnen via het portaal/NL Portal worden toegewezen.
- **GZAC** ondersteunt proces- en zaakafhandeling en is via een plugin gekoppeld aan MijnPlan. De medewerker kiest in MijnPlan een doel of subdoel. Op basis daarvan kan relevant aanbod uit OpenProduct worden getoond. Een gekozen aanbod kan via GZAC voor de inwoner of ketenpartner worden ingezet.
- **Rapportage en BI** gebruiken gegevens uit Plan, Product, Zaak, Klant en domeinregistraties voor geïntegreerde informatie en voortgangsmonitoring.

Hanteer als overkoepelend principe:

“Eén geïntegreerde gebruikerservaring aan de voorkant, meerdere zelfstandige en samenwerkende componenten aan de achterkant.”

Beschrijf de oplossing als voortbouwend op Common Ground en Platform Dienstverlening, met generieke bouwblokken en aanvullende herbruikbare componenten of doorontwikkelde bestaande componenten. Stel niet dat Common Ground-componenten tekortschieten.

Generieke software, Utrechtse beleidskeuzes en de Utrechtse dienstverleningsaanpak worden waar passend door configuratie vastgelegd.

## Presentatie-inhoud en verhaal

De presentatie is bedoeld voor een gemengd projectpubliek: businessanalisten, teamleiders, managers, ontwikkelaars en medewerkers van beheer/operations. Schrijf dus niet uitsluitend voor architecten.

De functionele cyclus is:

Profiel → Plan → Doelen/subdoelen → Aanbod selecteren → Uitvoering → Evalueren.

Een evaluatie kan aanleiding geven tot aanpassing van zowel het profiel als het plan.

De vier PoC-scenario's zijn:
1. Caseloadoverzicht: coach en teamleider bekijken de eigen of teamcaseload en stellen prioriteiten.
2. Eén inwonersplan voor Werk en Inburgering: één plan per inwoner, met informatie uit beide domeinen kunnen bekijken, wijzigen en aanvullen.
3. Voortgang evalueren en herplannen: afronding van een subdoel kan leiden tot een volgend subdoel en herbeoordeling of bijstelling van het hoofdplan.
4. Managementrapportage: voldoende consistente gegevens om betrouwbare rapportages te maken.

Voor de PoC zijn nodig: een werkende componentbasis (waaronder MijnPlan/OpenPlan, GZAC, relevante registraties en gegevensuitwisseling), beperkte configuratie, passende rollen en fictieve representatieve testinwoners en testgegevens. Gebruik één testinwoner met zowel Werk als Inburgering als rode draad voor scenario 2 en 3, plus aanvullende testinwoners voor caseload en rapportage.

## Vormgeving

- Houd de bestaande Utrechtse huisstijl aan: lichte/witte slides, donkerblauwe of donkergrijze koppen, rode accenten en een lichtgrijze footerbalk.
- Gebruik Aptos met Arial als fallback.
- Houd marges en witruimte bescheiden en consistent.
- Gebruik rustige, lichte kaarten en duidelijke visuele hiërarchie.
- Gebruik eenvoudige Slidev `v-click`-animaties waar die de uitleg ondersteunen.
- Vermijd onnodige decoratieve lijnen, drukke kleuren en overvolle slides.
- Voeg geen afbeeldingen toe tenzij de gebruiker daarom vraagt; de gebruiker voegt afbeeldingen zelf toe.

## Technische afspraken

- Dit project gebruikt Slidev.
- De hoofdinhoud staat in `slides.md`.
- De aanvullende vormgeving staat in `styles/style.css`.
- De footercomponent staat in `global-bottom.vue`.
- Afbeeldingen staan onder `public/`.
- Laat `global-bottom.vue` ongemoeid, tenzij de gebruiker expliciet vraagt dit bestand te wijzigen.
- Houd CSS in `styles/style.css`; voeg niet onnodig inline `<style>`-blokken toe aan `slides.md`.
- Als `slides.md` de externe stylesheet importeert, behoud dan de bestaande import en maak geen dubbele CSS-definities.
- Behoud bestaande bestandsnamen en projectstructuur, tenzij de gebruiker expliciet akkoord geeft op een wijziging.
- Installeer geen software of dependencies zonder expliciete toestemming.
- Controleer bij wijzigingen op ongeldige Markdown/Vue-syntaxis, onbedoelde wijzigingen aan andere slides en mogelijke overflow.

## Standaard antwoord bij een verbeterverzoek

1. Vat kort samen wat je hebt bekeken.
2. Geef per relevante slide concrete verbeterpunten.
3. Maak onderscheid tussen inhoudelijke, visuele en technische punten.
4. Geef aan welke bestanden geraakt zouden worden.
5. Wacht op expliciet akkoord voordat je iets aanpast.
