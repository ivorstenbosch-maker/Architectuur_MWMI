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
Eén geïntegreerde gebruikerservaring aan de voorkant,<br>
meerdere zelfstandige en samenwerkende componenten aan de achterkant.
</p>

<div style="margin-top:24px;">
  <span class="utrecht-pill">Common Ground</span>
  <span class="utrecht-pill">Platform Dienstverlening</span>
  <span class="utrecht-pill">Casusregie</span>
</div>

---

<!-- SLIDE 2 -->

# Van dienstverlening naar casusregie

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>Van losse contactmomenten</h3><p>Niet een verzameling afzonderlijke contactmomenten of registraties.</p></div>
  <div class="content-card" v-click><h3>Naar één samenhangend traject</h3><p>Professional en inwoner werken vanuit een gedeeld beeld, doelen en passende ondersteuning.</p></div>
  <div class="content-card" v-click><h3>Inzicht in de situatie</h3><p>Profiel en context van de inwoner vormen het vertrekpunt.</p></div>
  <div class="content-card" v-click><h3>Plan en doelen</h3><p>Afspraken worden vertaald naar doelen en subdoelen.</p></div>
  <div class="content-card" v-click><h3>Passend aanbod</h3><p>Ondersteuning en instrumenten worden ingezet op basis van de doelen.</p></div>
  <div class="content-card" v-click><h3>Volgen en evalueren</h3><p>De voortgang wordt besproken en waar nodig wordt de aanpak bijgesteld.</p></div>
</div>

---

<!-- SLIDE 3 -->

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

<!-- SLIDE 4 -->

# Eén geïntegreerde gebruikerservaring

<div class="flow-row" style="align-items:center;">
  <div class="content-card accent" style="text-align:center;" v-click><h3>Professional</h3><p>Werkt vanuit één geïntegreerde werkomgeving.</p></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card accent" style="text-align:center;"><h3>MijnPlan</h3><p>Interacties rond profiel, plan, doelen en evaluatie.</p></div></div>
  <div class="flow-step" v-click><div class="flow-arrow">→</div><div class="content-card" style="text-align:center;"><h3>Samenwerkende componenten</h3><p>Registraties en procesdiensten op de achtergrond.</p></div></div>
</div>

<div class="content-grid two" style="margin-top:20px;">
  <div class="content-card" v-click><h3>Wat merkt de medewerker?</h3><p>Eén samenhangende werkomgeving. Geen losse registraties om de casusregie uit te voeren.</p></div>
  <div class="content-card" v-click><h3>Wat gebeurt achter de schermen?</h3><p>Zelfstandige componenten wisselen gegevens uit en ondersteunen ieder een eigen deel van het proces.</p></div>
</div>
<p class="small-note" v-click>OpenProduct is een registratie voor aanbodbeheer; het is geen aparte werkomgeving voor casusregie.</p>

---

<!-- SLIDE 5 -->

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

<!-- SLIDE 6 -->

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

<!-- SLIDE 7 -->

# Hoe een casus door de componenten loopt

<div class="flow-row">
  <div class="content-card accent" v-click><h3>Professional</h3><p>Geïntegreerde werkomgeving.</p></div>
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

<!-- SLIDE 8 -->

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

<!-- SLIDE 9 -->

# Waar worden gegevens vastgelegd?

<div class="content-grid" style="grid-template-columns:repeat(3,minmax(0,1fr));gap:16px;margin-top:22px;">
  <div class="content-card" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>OpenKlant</h3><p>Inwoners, ketenpartners, adressen en contactmomenten.</p>
  </div>
  <div class="content-card accent" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>OpenPlan</h3><p>Plannen, doelen, subdoelen en evaluaties.</p>
  </div>
  <div class="content-card" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>OpenProduct</h3><p>Aanbod, instrumenten en voorzieningen.</p>
  </div>
  <div class="content-card" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>OpenZaak</h3><p>Zaken en bijbehorende context.</p>
  </div>
  <div class="content-card" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>Domeinregistraties</h3><p>Domeinspecifieke gegevens, bijvoorbeeld Werk of Inburgering.</p>
  </div>
  <div class="content-card" v-click style="min-height:175px;display:flex;flex-direction:column;justify-content:center;">
    <h3>VTB</h3><p>Verzoeken, taken en berichten.</p>
  </div>
</div>
<p v-click style="color:var(--u-red);font-weight:700;margin-top:14px;">Leg gegevens vast bij de component die daarvoor verantwoordelijk is.</p>

---

<!-- SLIDE 10 -->

# Van registraties naar inzicht

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
<div style="text-align:center;margin-top:14px;" v-click><span class="utrecht-pill">Voortgang volgen</span><span class="utrecht-pill">Ontwikkelingen signaleren</span><span class="utrecht-pill">Managementinformatie</span></div>

---

<!-- SLIDE 11 -->

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

<!-- SLIDE 12 -->

# Vier scenario's valideren

<div class="content-grid two">
  <div class="content-card accent" v-click><h3>1. Overzicht van de caseload</h3><p>Kan coach en teamleider de eigen of teamcaseload overzien en prioriteiten bepalen?</p></div>
  <div class="content-card" v-click><h3>2. Eén inwonerplan voor Werk én Inburgering</h3><p>Kan informatie uit beide domeinen integraal worden getoond, bewerkt en gemuteerd, met één plan per inwoner?</p></div>
  <div class="content-card" v-click><h3>3. Voortgang evalueren en herijken</h3><p>Kan een afgerond subdoel leiden tot een volgend subdoel en kan het inwonerplan worden herijkt?</p></div>
  <div class="content-card" v-click><h3>4. Managementrapportage</h3><p>Zijn gegevens voldoende beschikbaar en consistent om betrouwbare rapportages te maken?</p></div>
</div>
<div class="poc-section" v-click><h3>Praktische aanpak</h3><p style="font-size:13px;margin:0;">Gebruik één representatieve testinwoner met zowel Werk als Inburgering als rode draad voor scenario 2 en 3. Voeg enkele testinwoners toe voor caseload en rapportage.</p></div>

---

<!-- SLIDE 13 -->

# Het totaalbeeld

<p class="lead">Eén dienstverleningservaring, gedragen door samenwerkende componenten en duidelijke gegevensverantwoordelijkheden.</p>
<div style="height:390px;border:2px dashed var(--u-border);border-radius:12px;background:#FAFAFA;display:flex;align-items:center;justify-content:center;text-align:center;color:var(--u-mid);font-weight:700;margin-top:15px;">
  VOEG HIER HET TOTALE ARCHITECTUURPLAATJE TOE
</div>

---

<!-- SLIDE 14 -->

# Vragen & gesprek

<p class="lead" style="font-size:1.35rem;max-width:900px;">Wat betekent dit voor ontwerp, realisatie, beheer en dagelijks gebruik?</p>
<div style="margin-top:24px;">
  <span class="utrecht-pill">Functionaliteit</span>
  <span class="utrecht-pill">Samenwerking</span>
  <span class="utrecht-pill">Configuratie</span>
  <span class="utrecht-pill">Beheer</span>
</div>
<p class="small-note" style="position:absolute;bottom:55px;">Dank voor jullie bijdrage.</p>
