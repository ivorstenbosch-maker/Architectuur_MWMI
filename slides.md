---
theme: default
title: Architectuur MijnWerk / MijnInburgering
transition: slide-left
mdc: true
---

<style>
@import './styles/style.css';
</style>

<!-- SLIDE 1 -->

# Architectuur MijnWerk / MijnInburgering

<p class="lead" style="font-size:1.35rem; max-width:950px;">
Integrale dienstverlening met generieke bouwblokken en configureerbare ondersteuning
</p>

---

<!-- SLIDE 2 -->

# Inhoud

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>1. Visie en architectuur</h3><p>Common Ground, het vijflaagsmodel, de doelen, de architectuurcontext en de functionele cyclus.</p></div>
  <div class="content-card" v-click><h3>2. Registraties en rapportage</h3><p>Informatiebeheer, rapportage en inzicht.</p></div>
  <div class="content-card" v-click><h3>3. PoC en scenario's</h3><p>Benodigde basis en de scenario's die we willen valideren.</p></div>
  <div class="content-card" v-click><h3>4. Verdieping businessanalyse</h3><p>Routes, overgang naar Acquisitie en Matching, status, voortgang en intake.</p></div>
  <div class="content-card" v-click><h3>5. Bepalen voor een werkbare PoC</h3><p>De afspraken en keuzes die verdere uitwerking mogelijk maken.</p></div>
</div>

---

<!-- SLIDE 3 -->

# Architectuurcontext van deze ontwikkeling

<p class="lead">De ontwikkeling sluit aan op de samenhang tussen visie, architectuurkader en platformrealisatie.</p>

<div class="flow-row">
  <div class="content-card accent" v-click><h3>Common Ground</h3><p>De informatiekundige visie en richting.</p></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>Enterprise Architectuur</h3><p>Het gezamenlijke kader voor principes, keuzes en samenhang.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent"><h3>Platform Dienstverlening</h3><p>De referentie-implementatie met componenten, registraties, API's en infrastructuur.</p></div></div>
</div>

<div class="poc-section" v-click><h3>Positionering</h3><p style="font-size:13px;margin:0;">MijnWerk en MijnInburgering passen binnen het sociaal domein en bouwen voort op de samenhangende bouwblokken van Platform Dienstverlening.</p></div>

---

<!-- SLIDE 4 -->

# Common Ground en het vijflaagsmodel

<p class="lead">Eén dienst voor de inwoner; herbruikbare bouwstenen werken achter de schermen samen.</p>

<div class="flow-row">
  <div class="content-card accent" v-click><h3>1. Interactie</h3><p>De inwoner gebruikt de dienst.</p></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>2. Proces</h3><p>De dienst wordt uitgevoerd.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>3. Connectiviteit</h3><p>Componenten wisselen berichten uit.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>4. Diensten</h3><p>Gegevens worden via API's ontsloten.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent"><h3>5. Registraties</h3><p>Gegevens worden bij de bron vastgelegd.</p></div></div>
</div>

<p class="small-note" v-click>Common Ground geeft de richting; Enterprise Architectuur bewaakt de samenhang en Platform Dienstverlening maakt bouwstenen concreet.</p>

---

<!-- SLIDE 5 -->

# Doelen van de architectuur

<p class="lead">MijnWerk en MijnInburgering ondersteunen dienstverlening die voor medewerker en inwoner overzichtelijk, samenhangend en doorontwikkelbaar is.</p>

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>Overzicht voor de medewerker</h3><p>Een samenhangend beeld van de inwoner en het traject.</p></div>
  <div class="content-card" v-click><h3>Transparantie voor de inwoner</h3><p>Inzicht in afspraken, stappen en voortgang.</p></div>
  <div class="content-card" v-click><h3>Integrale dienstverlening</h3><p>Werk en Inburgering verbinden en uitbreiden naar andere domeinen.</p></div>
  <div class="content-card" v-click><h3>Efficiënte administratie en processen</h3><p>Administratie en processtappen efficiënt ondersteunen.</p></div>
  <div class="content-card" v-click><h3>Onderhoudbaar binnen het platform</h3><p>Aansluiten op de doorontwikkeling van Platform Dienstverlening.</p></div>
  <div class="content-card accent" v-click><h3>Datagedreven werken</h3><p>Beslisregels ondersteunen keuzes; rapportage geeft inzicht in de performance van processen.</p></div>
</div>

---

<!-- SLIDE 6 -->

# De functionele cyclus

<p class="lead">De professional doorloopt een samenhangende cyclus met ruimte om onderweg bij te stellen.</p>

<div class="flow-row">
  <div class="content-card accent" v-click><h3>1. Profiel</h3><p>Inzicht in de inwoner.</p></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>2. Plan</h3><p>Afspraken en aanpak.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>3. Doelen en subdoelen</h3><p>Concrete richting.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>4. Aanbod selecteren</h3><p>Passende ondersteuning.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>5. Uitvoering</h3><p>Aanbod inzetten.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent"><h3>6. Evalueren</h3><p>Voortgang bespreken.</p></div></div>
</div>

<div class="poc-section" v-click><h3>Terugkoppeling</h3><p style="font-size:13px;margin:0;">Evaluatie kan aanleiding zijn om zowel het <strong>profiel</strong> als het <strong>plan</strong> bij te stellen.</p></div>

---

<!-- SLIDE 7 -->

# Eén geïntegreerde gebruikerservaring

<div class="content-grid two" style="margin-top:18px;">
  <div class="content-card accent" v-click><h3>IKO</h3><p>Ingang voor een integraal overzicht van de inwoner.</p></div>
  <div class="content-card" v-click><h3>MijnPlan</h3><p>Ingang voor interacties rond profiel, plan, doelen en evaluatie.</p></div>
</div>
<p class="small-note" v-click>Vanuit beide ingangen loopt de medewerker naadloos door naar dezelfde relevante informatie en views per procesfase.</p>

<div class="content-grid two" style="margin-top:20px;">
  <div class="content-card" v-click><h3>Wat merkt de medewerker?</h3><p>Een geïntegreerde werkomgeving met logische overgangen naar views per procesfase.</p></div>
  <div class="content-card" v-click><h3>Wat gebeurt achter de schermen?</h3><p>Zelfstandige componenten wisselen gegevens uit en ondersteunen ieder een eigen deel van het proces.</p></div>
</div>
<p class="small-note" v-click>OpenProduct is een registratie voor aanbodbeheer.</p>

---

<!-- SLIDE 8 -->

# Gebruikerservaring en procesondersteuning

<div class="arch-legend">
  <span><i class="arch-dot arch-new"></i> Nieuw t.o.v. CommLtr</span>
  <span><i class="arch-dot arch-special"></i> Speciaal ontwikkeld voor casusregie</span>
  <span><i class="arch-dot arch-existing"></i> Bestaand</span>
</div>
<div class="arch-grid">
  <div class="arch-card" v-click><div class="arch-desc">Integraal overzicht van inwoner</div><div class="arch-name arch-new-fill">IKO</div></div>
  <div class="arch-card" v-click><div class="arch-desc">Procesafhandeling (zaken, producten, intake)</div><div class="arch-name arch-existing-fill">GZAC</div></div>
  <div class="arch-card" v-click><div class="arch-desc">Inwoner in beeld, domeinspecifieke registratie</div><div class="arch-name arch-special-fill">MijnProfiel</div></div>
  <div class="arch-card" v-click><div class="arch-desc">Proces planvorming en evaluatie</div><div class="arch-name arch-special-fill">MijnPlan</div></div>
  <div class="arch-card" v-click><div class="arch-desc">Interactie inwoner en ketenpartners</div><div class="arch-name arch-new-fill">NL Portal</div></div>
  <div class="arch-card" v-click><div class="arch-desc">Inrichting beslisregels</div><div class="arch-name arch-new-fill">Valtimo & DMN Studio</div></div>
</div>

---

<!-- SLIDE 9 -->

# Registraties en domeinmodellen

<div class="arch-legend">
  <span><i class="arch-dot arch-new"></i> Nieuw t.o.v. CommLtr</span>
  <span><i class="arch-dot arch-special"></i> Speciaal ontwikkeld voor casusregie</span>
  <span><i class="arch-dot arch-existing"></i> Bestaand</span>
</div>
<div class="arch-grid">
  <div class="arch-card" v-click><div class="arch-name arch-new-fill">OpenKlant</div><div class="arch-desc">Klantgegevens en ketenpartners</div></div>
  <div class="arch-card" v-click><div class="arch-name arch-existing-fill">OpenZaak</div><div class="arch-desc">Zaakregistratie en zaakcontext</div></div>
  <div class="arch-card" v-click><div class="arch-name arch-new-fill">OpenProduct</div><div class="arch-desc">Aanbod en voorzieningen</div></div>
  <div class="arch-card" v-click><div class="arch-name arch-new-fill">OpenOrganisatie</div><div class="arch-desc">Medewerkers en teams</div></div>
  <div class="arch-card" v-click><div class="arch-name arch-special-fill">OpenPlan</div><div class="arch-desc">Plan, (sub)doelen en evaluaties</div></div>
  <div class="arch-card" v-click><div class="arch-name arch-special-fill">Werk / Inburgering</div><div class="arch-desc">Relationele domeinmodellen</div></div>
</div>
<p class="arch-note" v-click>Elke registratie heeft een eigen gegevensverantwoordelijkheid. Samen ondersteunen ze de integrale dienstverlening.</p>

---

<!-- SLIDE 10 -->

# Hoe een casus door de componenten loopt

<div class="flow-row">
  <div class="content-card accent" v-click><h3>Professional</h3><p>Geïntegreerde werkomgeving.</p></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent"><h3>IKO</h3><p>Integraal overzicht van de inwoner.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent"><h3>MijnPlan</h3><p>Profiel, plan en evaluatie.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>OpenPlan</h3><p>Plan, doelen en evaluaties.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>OpenProduct</h3><p>Passend aanbod op basis van doel of subdoel.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card"><h3>GZAC</h3><p>Proces- en zaakafhandeling.</p></div></div>
</div>
<h3 v-click style="color:var(--u-red);margin-top:20px;">Ondersteunende registraties en diensten</h3>
<div class="content-grid" style="grid-template-columns:repeat(4,minmax(0,1fr));">
  <div class="content-card" v-click><h3>OpenKlant</h3><p>Inwoner en contact.</p></div>
  <div class="content-card" v-click><h3>OpenZaak</h3><p>Zaakcontext.</p></div>
  <div class="content-card" v-click><h3>VTB</h3><p>Verzoeken, taken en berichten.</p></div>
  <div class="content-card" v-click><h3>Domeinregistraties</h3><p>Werk en Inburgering.</p></div>
</div>

---

<!-- SLIDE 11 -->

# Generieke software, Utrechtse inrichting

<div class="content-grid two">
  <div class="content-card accent" v-click>
    <h3>OpenPlan</h3><p><strong>Configureert onder meer:</strong></p>
    <ul><li>Opbouw van plannen</li><li>Doelen en subdoelen</li><li>Evaluaties</li><li>Inrichting dienstverlening Werk en Inburgering</li></ul>
  </div>
  <div class="content-card" v-click>
    <h3>OpenProduct</h3><p><strong>Configureert onder meer:</strong></p>
    <ul><li>Aanbod, instrumenten en voorzieningen</li><li>Productgerichte workflows</li><li>Beslisregels per aanbod of instrument</li></ul>
  </div>
</div>
<div class="poc-section" v-click><h3>Uitgangspunt</h3><p style="font-size:13px;margin:0;">De software en componenten zijn generiek. De Utrechtse beleidskeuzes en werkwijze worden zo veel mogelijk via configuratie ingericht.</p></div>

---

<!-- SLIDE 12 -->

# Rapportage

<p class="lead">Gegevens uit de verschillende registraties worden samengebracht voor monitoring en sturing.</p>
<div class="content-grid" style="grid-template-columns:repeat(5,minmax(0,1fr));">
  <div class="content-card accent" v-click><h3>OpenPlan</h3></div>
  <div class="content-card" v-click><h3>OpenProduct</h3></div>
  <div class="content-card" v-click><h3>OpenZaak</h3></div>
  <div class="content-card" v-click><h3>OpenKlant</h3></div>
  <div class="content-card" v-click><h3>Domeinregistraties</h3></div>
</div>
<div v-click style="text-align:center;color:var(--u-red);font-size:25px;margin:5px 0;">↓ &nbsp; ↓ &nbsp; ↓ &nbsp; ↓ &nbsp; ↓</div>
<div class="content-card accent" style="max-width:650px;margin:0 auto;text-align:center;" v-click><h3>Geïntegreerd informatiemodel / BI</h3><p>Samenhangende informatie voor inzicht in voortgang.</p></div>

---

<!-- SLIDE 13 -->

# Integraal informatiemodel

<img src="/integraal-informatiemodel.png" alt="Voorbeeld van een integraal informatiemodel met onder meer plan, doelen, subdoelen, evaluaties, aanbod, persoon en contactmoment" style="display:block;max-width:100%;max-height:calc(100vh - 160px);width:auto;height:auto;object-fit:contain;margin:0 auto;" />

---

<!-- SLIDE 14 -->

# Wat is nodig voor de PoC?

<div class="content-grid two">
  <div class="content-card accent" v-click>
    <h3>Werkende componentbasis</h3>
    <ul><li>MijnPlan en OpenPlan</li><li>GZAC voor proces- en zaakafhandeling</li><li>Aansluiting op relevante registraties</li><li>Beperkte, werkende gegevensuitwisseling</li></ul>
  </div>
  <div class="content-card" v-click>
    <h3>Configuratie</h3>
    <ul><li>Voorbeeldplan met doelen en subdoelen</li><li>Beperkte inrichting Werk en Inburgering</li><li>Kleine catalogus met aanbod</li><li>Voorbeeldworkflows en beslisregels waar nodig</li></ul>
  </div>
  <div class="content-card" v-click>
    <h3>Rollen en autorisaties</h3>
    <ul><li>Coach</li><li>Teamleider</li><li>Eventueel beheer- en rapportagerol</li></ul>
  </div>
  <div class="content-card" v-click>
    <h3>Testinwoners en testdata</h3>
    <ul><li>Fictieve inwoners met Werk en Inburgering</li><li>Plannen, doelen en subdoelen</li><li>Aanbod, evaluaties en zaken</li><li>Variatie in status en voortgang</li></ul>
  </div>
</div>

---

<!-- SLIDE 15 -->

# Scenario's

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>1. Overzicht van de caseload</h3><p>Kan coach en teamleider de eigen of teamcaseload overzien en prioriteiten bepalen?</p></div>
  <div class="content-card" v-click><h3>2. Eén inwonerplan voor Werk én Inburgering</h3><p>Kan informatie uit beide domeinen integraal worden getoond, bewerkt en gemuteerd, met één plan per inwoner?</p></div>
  <div class="content-card" v-click><h3>3. Voortgang evalueren en herijken</h3><p>Kan een afgerond subdoel leiden tot een volgend subdoel en kan het inwonerplan worden herijkt?</p></div>
  <div class="content-card" v-click><h3>4. Managementrapportage</h3><p>Zijn gegevens voldoende beschikbaar en consistent om betrouwbare rapportages te maken?</p></div>
</div>
<div class="poc-section" v-click><h3>Praktische aanpak</h3><p style="font-size:13px;margin:0;">Maak mockdata aan voor meerdere fictieve testinwoners met verschillende routes, domeinen, statussen en voortgang. Gebruik een inwoner met zowel Werk als Inburgering als rode draad voor scenario 2 en 3; vul dit aan met testinwoners voor caseload en rapportage.</p></div>

---

<!-- SLIDE 16 -->

# Verdieping: verschillende routes

<p class="lead">Verschillende routes kunnen andere keuzes vragen voor doelen, aanbod en evaluatie.</p>

<div class="content-grid">
  <div class="content-card accent" v-click><h3>Reguliere werkdienstverlening</h3><p>Welke doelen worden opgebouwd en in welke volgorde? Welk aanbod past per stap, en wanneer evalueren inwoner en coach de voortgang?</p></div>
  <div class="content-card" v-click><h3>Fastlane naar UW</h3><p>De inwoner wordt direct gekoppeld aan UW. Welke doelen zijn dan leidend, welk aanbod wordt ingezet en hoe wordt de voortgang geëvalueerd?</p></div>
  <div class="content-card" v-click><h3>Werk en Inburgering samen</h3><p>Hoe hangen doelen uit beide domeinen samen? Hoe wordt aanbod op elkaar afgestemd en hoe evalueren betrokkenen de gezamenlijke voortgang?</p></div>
</div>

<div class="poc-section" v-click><h3>Businessanalyse</h3><p style="font-size:13px;margin:0;">Beschrijf per route de aanleiding, gewenste uitkomst, betrokken rollen en momenten waarop doelen of aanbod worden bijgesteld.</p></div>

---

<!-- SLIDE 17 -->

# Verdieping: overgang Acquisitie en Matching

<p class="lead">Als een inwoner werkfit is, volgt een overgang naar een losse applicatie. De inwoner moet in de dienstverlening zichtbaar en te volgen blijven.</p>

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>Continuïteit van doelen</h3><p>Welke doelen en afspraken blijven relevant bij de overgang, en hoe ziet de ontvangende professional de actuele stand?</p></div>
  <div class="content-card" v-click><h3>Voortgang en terugkoppeling</h3><p>Welke voortgang uit Acquisitie en Matching moet terugkomen, wie legt die vast en hoe wordt deze meegenomen in evaluaties?</p></div>
  <div class="content-card" v-click><h3>Verantwoordelijkheid</h3><p>Wie volgt de inwoner tijdens de overgang en daarna? Hoe zijn overdracht en opvolging voor inwoner en professionals duidelijk?</p></div>
  <div class="content-card" v-click><h3>In beeld blijven</h3><p>Welke informatie is nodig voor caseload, monitoring en een actueel beeld van de inwoner over beide applicaties heen?</p></div>
</div>

---

<!-- SLIDE 18 -->

# Verdieping: status, voortgang en intake

<p class="lead">Maak onderscheid tussen de fase waarin iets zich bevindt en de ontwikkeling richting een resultaat.</p>

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>Status</h3><p>Welke statussen horen bij plan, doel/subdoel en aanbod of product? Wie wijzigt ze en welke overgangsmomenten zijn betekenisvol?</p></div>
  <div class="content-card" v-click><h3>Voortgang</h3><p>Hoe wordt ontwikkeling richting een doel zichtbaar gemaakt? Welke evaluatiemomenten en informatie ondersteunen bijsturen?</p></div>
  <div class="content-card" v-click><h3>Monitoring en fasering</h3><p>Welk onderdeel is leidend voor caseload en rapportage: planfase, doelvoortgang, ingezette producten of een combinatie?</p></div>
  <div class="content-card" v-click><h3>Reikwijdte van intake</h3><p>Is intake een brede verkenning van de situatie van de inwoner, of richt deze zich alleen op werkdienstverlening? Wat vraagt elke keuze van doelen en vervolg?</p></div>
</div>

---

<!-- SLIDE 19 -->

# Bepalen voor een werkbare PoC

<p class="lead">Maak de belangrijkste afspraken expliciet voordat de scenario's worden ingericht en getest.</p>

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>Rollen en toegang</h3><p>Wie bekijkt of wijzigt profiel, plan, domeingegevens en aanbod? Hoe verschillen coach, teamleider en beheer?</p></div>
  <div class="content-card" v-click><h3>Gegevens en uitwisseling</h3><p>Welke gegevens uit Werk en Inburgering zijn nodig in het gezamenlijke plan, en welke component is daarvoor verantwoordelijk?</p></div>
  <div class="content-card" v-click><h3>Proces en aanbod</h3><p>Welke stappen en beslisregels horen bij het selecteren en inzetten van aanbod via GZAC?</p></div>
  <div class="content-card" v-click><h3>Succescriteria</h3><p>Wanneer zijn caseload, één inwonerplan, herplannen en managementrapportage voldoende aangetoond?</p></div>
</div>

<div class="poc-section" v-click><h3>Resultaat</h3><p style="font-size:13px;margin:0;">Een afgebakende inrichting, duidelijke verantwoordelijkheden en toetsbare uitkomsten voor de PoC.</p></div>

---
