# Club.Redders - IT Suite voor non profits

## Introductie

![](../assets/images/itsppt/IT Suite voor non profits6.png)

* <span style="color:#7BB1DB"> __Doel van__ </span>  <span style="color:#7BB1DB"> __deze__ </span>  <span style="color:#7BB1DB"> __presentatie__ </span>
* <span style="color:#000000">Een</span>  <span style="color:#000000">overzicht</span>  <span style="color:#000000">geven van de</span>  <span style="color:#000000">functionaliteiten</span>  <span style="color:#000000">\,</span>  <span style="color:#000000">architectuur en</span>  <span style="color:#000000">roadmap</span>  <span style="color:#000000">van de IT Suite voor non</span>  <span style="color:#000000">profits</span>  <span style="color:#000000">en</span>  <span style="color:#000000">Club\.Redders</span>  <span style="color:#000000">\.</span>
* <span style="color:#000000">Informeren</span>  <span style="color:#000000">van gebruikers\, beheerders en ontwikkelaars</span>  <span style="color:#000000">over hoe de verschillende</span>  <span style="color:#000000">componenten samenhangen\.</span>
* <span style="color:#000000">Bewustzijn</span>  <span style="color:#000000">creëren</span>  <span style="color:#000000">over</span>  <span style="color:#000000">de afhankelijkheden en impact van bepaalde acties door betrokkenen op de componenten\.</span>
* <span style="color:#000000">Duidelijk maken voor welke periode bepaalde wensen bij de ontwikkelaars bekend moeten zijn voor de volgende release</span>  <span style="color:#000000">\.</span>
* <span style="color:#7BB1DB"> __Doelgroep__ </span>
* Gebruikersenbeheerdersvan de IT Suite
  * Office 365\,MachForm\,Club\.Redders\, C\.R WordPress plugin
* OntwikkelaarsvanClub\.Redders
  * Core\, modulesenCMS plugins

![](../assets/images/itsppt/IT Suite voor non profits7.jpg)

* <span style="color:#7BB1DB"> __ORGANISATIE WENSEN :__ </span>
* <span style="color:#000000">Een volledige online beschikbare IT omgeving\.</span>
* <span style="color:#000000">Zo’n professioneel mogelijke kwaliteit tegen zo’n laag mogelijke kosten\.</span>
* <span style="color:#000000">Bestaande</span>  <span style="color:#000000">vrij beschikbare</span>  <span style="color:#000000">tooling</span>  <span style="color:#000000">over low\-</span>  <span style="color:#000000">cost</span>  <span style="color:#000000">tooling</span>  <span style="color:#000000">over</span>  <span style="color:#000000">bouwen\.</span>
* <span style="color:#000000">IT componenten moeten los van elkaar kunnen functioneren of individueel vervangen kunnen worden door een alternatief product met dezelfde functionaliteiten\.</span>
* <span style="color:#7BB1DB"> __IT SUITE VOOR NONPROFITS:__ </span>
* <span style="color:#000000">Maakt</span>  <span style="color:#000000">gebruik van open source of via</span>  <span style="color:#000000">TechSoup</span>  <span style="color:#000000">gratis verkrijgbare software\.</span>
* <span style="color:#000000">Gebruikt</span>  <span style="color:#000000">Office 365 als oplossing voor mail\,</span>  <span style="color:#000000">gegevens</span>  <span style="color:#000000">opslag\,</span>  <span style="color:#000000">chat en</span>  <span style="color:#000000">social</span>  <span style="color:#000000">platform\.</span>
  * <span style="color:#000000">Azure</span>  <span style="color:#000000">AD wordt ingezet voor Single</span>  <span style="color:#000000">Sign</span>  <span style="color:#000000">On en</span>  <span style="color:#000000">wachtwoordresetfunctionaliteit</span>  <span style="color:#000000">binnen de IT Suite\.</span>
* <span style="color:#000000">Gebruikt</span>  <span style="color:#000000">MachForm</span>  <span style="color:#000000">\(betaald\) als WYSIWYG formulieren</span>  <span style="color:#000000">tool\.</span>
  * <span style="color:#000000"> _SSO is mogelijk met_ </span>  <span style="color:#000000"> _Okta_ </span>  <span style="color:#000000"> _\(_ </span>  <span style="color:#000000"> _MachForm_ </span>  <span style="color:#000000"> _<> LDAP <> OKTA <> SAML <> O365\)\._ </span>
* <span style="color:#000000">Gebruikt</span>  <span style="color:#000000">WordPress</span>  <span style="color:#000000">als</span>  <span style="color:#000000">website</span>  <span style="color:#000000">content management oplossing met SSO via</span>  <span style="color:#000000">O365\.</span>
* <span style="color:#7BB1DB"> __CLUB\.REDDERS:__ </span>
* <span style="color:#000000">Zet voor vereniging specifieke wensen een zelfbouw tool in gebaseerd op</span>  <span style="color:#000000">PHP\.</span>
* <span style="color:#000000"> _Modulair opgebouwd zodat modules door verschillende ontwikkelaars kunnen worden ontwikkeld en worden toegevoegd en verwijderd zonder impact op andere modules\._ </span>
* <span style="color:#000000">Open Source</span>  <span style="color:#000000">zodat de software</span>  <span style="color:#000000">en documentatie voor</span>  <span style="color:#000000">alle betrokkenen vrij beschikbaar is en blijft\.</span>
  * <span style="color:#000000">Software is vrij beschikbaar onder de GPL en MIT licentie\.</span>
  * <span style="color:#000000">Documentatie is vrij beschikbaar onder</span>  <span style="color:#000000">de CC BY\-SA</span>  <span style="color:#000000">4\.0 licentie\.</span>

## High level view

### HIGH LEVEL VIEW IT SUITE

NONPROFIT SUPPORT TOOLING

Modulaire opensource app voor maatwerk functionaliteiten

![](../assets/images/itsppt/IT Suite voor non profits8.png)

![](../assets/images/itsppt/IT Suite voor non profits9.png)

IdP& VEILIGE WERKOMGEVING

Éénaccount voor toegang tot interne en externe diensten

![](../assets/images/itsppt/IT Suite voor non profits10.png)

![](../assets/images/itsppt/IT Suite voor non profits11.png)

WYSIWYG FORMULIER EDITOR

Bouw eenvoudig veilige en versleutelde formulieren metprocesflows

![](../assets/images/itsppt/IT Suite voor non profits12.png)

![](../assets/images/itsppt/IT Suite voor non profits13.png)

WYSIWYG WEBSITE MANAGEMENT

Bouw en beheer eenvoudig je website en haar content

![](../assets/images/itsppt/IT Suite voor non profits14.png)

![](../assets/images/itsppt/IT Suite voor non profits15.png)

![](../assets/images/itsppt/IT Suite voor non profits16.png)

### IT Suite

### Interne en externe IT-componenten

<span style="color:#000000">Interne</span>  <span style="color:#000000">omgeving</span>

<span style="color:#000000">Externe</span>  <span style="color:#000000">omgeving</span>

### IT diensten derden | via KeeWeb

<span style="color:#000000">Externe omgeving</span>

## Product eisen

### Eisen Club.Redders

![](../assets/images/itsppt/IT Suite voor non profits17.png)

Werkt\-getest

Geen producten bekend\.

* Software eisen;
  * SSL\-certificaten \(met autorenewal\)\, SFTP\, SSH\,MariaDB\, \.htaccess\, PHP 7\.4 of hoger\.
* Taken/kennis eisen IT functionaris;
  * Git\, PHP\, SQL\, HTML\, JS\, Apache\,MariaDB\,phpMyAdmin\, MVC principes\, SSH\, MicrosoftGraph\.
  * Couldhaves; ervaring metWordPressPluginDevelopment\.

Werkt\-nietgetest

TransIP\.

Hostnet\.

Vimexx\.

Werktniet\-getest

PCextreme\.

![](../assets/images/itsppt/IT Suite voor non profits18.png)

### Eisen IdP & Veilige werkomgeving

Werkt\-getest

Office 365\.

* Software eisen;
  * Huidige features die worden ingezet uit O365 dienen ook aanwezig te zijn in een eventueel in te zetten alternatief\.
* Taken/kennis eisen IT functionaris;
  * Musthaves;
    * Beheercentra; Microsoft Office 365\,AzureActive Directory\, Exchange\.
    * DNS MX\-records\,Groepstype’sO365\, distributie en security\.
    * Gebruikersbeheer incl\. O365 Licenties en Apps\.
  * Shouldhaves;
    * Beheercentra; Teams\, SharePoint\, OneDrive\,Yammer\.
    * PowerShell\, Office 365 beheerdersrollen\, Office 365 licentie model \(E/A/P\)\.
  * Couldhaves;
    * Beheercentra; Microsoft Search\, Dynamics 365\, Power Apps\.

Werkt\-nietgetest

Geen producten bekend\.

Werktniet\-getest

Geen producten bekend\.

![](../assets/images/itsppt/IT Suite voor non profits19.png)

### Eisen WYSIWYG Formulier editor

Werkt\-getest

MachForm\.

* Software eisen;
  * Huidige features die worden ingezet uitMachFormdienen ook aanwezig te zijn in een eventueel in te zetten alternatief\.
* Taken/kennis eisen IT functionaris;
  * Installatie en updates van PHP software pakketten op een webserver\.
  * Apache\,MariaDB\,phpMyAdmin\.

Werkt\-nietgetest

OhMyForm\.

OrbeonForms\.

Werktniet\-getest

Geen producten bekend\.

### Eisen WYSIWYG Website management

![](../assets/images/itsppt/IT Suite voor non profits20.png)

Werkt\-getest

WordPress\.

* Software eisen;
  * Plug\-in support voor C\.R Mijn omgeving plug\-in\.
    * Indien geen support aanwezig voor plug\-ins zou de PHP code van de plug\-in geïntegreerd moeten kunnen worden in het gekozen product als vereist\.
  * WordPressis enkel een front\-end en geen vereiste voor de IT\.
* Taken/kennis eisen IT functionaris;
  * Installatie en updates van PHP software pakketten op een webserver\.
  * Apache\,MariaDB\,phpMyAdmin\.

Werkt\-nietgetest

Geen producten bekend\.

Werktniet\-getest

Geen producten bekend\.

### Eisen externe systemen

![](../assets/images/itsppt/IT Suite voor non profits21.png)

Werkt\-getest

Sportlink\.

Rabobank CSV\.

* Software eisen extern ledenadministratie pakket;
  * CSV export van leden met attributen\.
  * CSV export van bondsfuncties met attributen\.
  * CSV export van bondsdiploma’s met attributen\.
* Software eisen internetbankieren;
  * CSV export vantransactiesmetattributen\.
  * MT940 export vantransactiesmetattributen\.
* Taken/kennis eisen IT functionaris;
  * Het beheer van externe systemen valt buiten de scope t\.a\.v\. het takenpakket en kennis vereiste van IT functionarissen\.
* Advies: houd domeinregistratie en webhosting gescheiden tussen bestuur en IT functionarissen\.
  * Zorg dat toegang van MFA is voorzien en bij voorkeur ook van persoonlijke accounts\.

Werkt\-nietgetest

Rabobank MT940\.

Werktniet\-getest

Geen producten bekend\.

### Begroting

## Componenten

### Sheet TOELICTING

<span style="color:#000000">IT Suite voor</span>  <span style="color:#000000">nonprofits</span>

<span style="color:#000000">IT diensten derden</span>

Pictogrammen

Persoonlijk account

Persoonlijk account 3de

Legacyomgeving

Doel omgeving

Externe omgeving

Interne omgeving

Database

LDAP\*

Legacy/Doel stroom

Data

RechtenSameSignOn

\*\) Identiteits\- entoegangsbeheer database

![](../assets/images/itsppt/IT Suite voor non profits22.png)

![](../assets/images/itsppt/IT Suite voor non profits23.png)

<span style="color:#000000">Tijdelijke Excel tools</span>

Huidige situatie

### Vereenvoudigde weergave

<span style="color:#000000">Externe</span>  <span style="color:#000000">leden</span>  <span style="color:#000000">administratie</span>

![](../assets/images/itsppt/IT Suite voor non profits24.png)

Leden\-vergelijking

Release targets

Club\.Redders:

Rechten lopen viaWordPress

Rechten gaan naar O365

Office 365:

Levert inlog account voor WP\, O365 enMachForm\(SameSO\)

MachForm:

Procesflows/approvals

Levert formulier data aan C\.R

WordPress:

Statische website

Club\.ReddersWPplugin:

Bied toegang tot Mijn C\.R

Excel modules:

Bevatten functies die nog ingebouwd moeten worden in C\.R\, alleen het jaarrooster levert ook nog data terug\.

SingleSignOn

<span style="color:#000000">Bank\-</span>  <span style="color:#000000">afschriften</span>

![](../assets/images/itsppt/IT Suite voor non profits25.png)

Transacties MT940

![](../assets/images/itsppt/IT Suite voor non profits26.png)

<span style="color:#000000">Jaarrooster module</span>

<span style="color:#000000">Competenties support module</span>

<span style="color:#000000">Contributie</span>  <span style="color:#000000">module</span>

<span style="color:#000000">Boekhouding</span>  <span style="color:#000000">module</span>

__Overzicht IT\-componenten__

Huidige situatie

### Weergave met extensies

<span style="color:#000000">Externe</span>  <span style="color:#000000">leden</span>  <span style="color:#000000">administratie</span>

![](../assets/images/itsppt/IT Suite voor non profits27.png)

Leden\-vergelijking

Release targets

Club\.Redders:

Rechten lopen viaWordPress

Rechten gaan naar O365

Office 365:

Levert inlog account voor WP\, O365 enMachForm\(SameSO\)

MachForm:

Procesflows/approvals

Levert formulier data aan C\.R

WordPress:

Statische website

Club\.ReddersWPplugin:

Bied toegang tot Mijn C\.R

Excel modules:

Bevatten functies die nog ingebouwd moeten worden in C\.R\, alleen het jaarrooster levert ook nog data terug\.

SingleSignOn

<span style="color:#000000">Bank\-</span>  <span style="color:#000000">afschriften</span>

![](../assets/images/itsppt/IT Suite voor non profits28.png)

Transacties MT940

![](../assets/images/itsppt/IT Suite voor non profits29.png)

<span style="color:#000000">Outlook/Exchange</span>

<span style="color:#000000">Jaarrooster module</span>

<span style="color:#000000">Competenties support module</span>

<span style="color:#000000">Contributie</span>  <span style="color:#000000">module</span>

<span style="color:#000000">Boekhouding</span>  <span style="color:#000000">module</span>

__Overzicht IT\-componenten__

Beoogde eindsituatie

### Modulaire tool met P-A-O releases

<span style="color:#000000">Externe</span>  <span style="color:#000000">leden</span>  <span style="color:#000000">administratie</span>

![](../assets/images/itsppt/IT Suite voor non profits30.png)

Leden\-vergelijking

Release targets

Club\.Redders:

Verbonden metAPI’s

CSV\-Importsvia POST\-API\.

CSV\-Exports via SQL Query\.

Office 365:

Geeft alle rechten direct uit binnen alle systemen\.

MachForm:

Levert formulier data als JSON aan bijClub\.Redders

WordPress:

Kan vervangen worden door elk CMS met SSO support op basis van O365 en code support voor deplugin\.

Excel modules:

Zijn komen te vervallen en functionaliteiten zitten in C\.R modules\.

SingleSignOn

<span style="color:#000000">Bank\-</span>  <span style="color:#000000">afschriften</span>

![](../assets/images/itsppt/IT Suite voor non profits31.png)

Transacties MT940

![](../assets/images/itsppt/IT Suite voor non profits32.png)

<span style="color:#000000">Outlook/Exchange</span>

<span style="color:#000000">Jaarrooster module</span>

<span style="color:#000000">Competenties support module</span>

<span style="color:#000000">Contributie</span>  <span style="color:#000000">module</span>

<span style="color:#000000">Boekhouding</span>  <span style="color:#000000">module</span>

__Overzicht IT\-componenten__

Beoogde eindsituatie

<span style="color:#000000">Externe</span>  <span style="color:#000000">leden</span>  <span style="color:#000000">administratie</span>

![](../assets/images/itsppt/IT Suite voor non profits33.png)

Leden\-vergelijking

Release targets

Club\.Redders:

Verbonden metAPI’s

CSV\-Importsvia POST\-API\.

CSV\-Exports via SQL Query\.

Office 365:

Geeft alle rechten direct uit binnen alle systemen\.

MachForm:

Levert formulier data als JSON aan bijClub\.Redders

WordPress:

Kan vervangen worden door elk CMS met SSO support op basis van O365 en code support voor deplugin\.

Excel modules:

Zijn komen te vervallen en functionaliteiten zitten in C\.R modules\.

SingleSignOn

<span style="color:#000000">Bank\-</span>  <span style="color:#000000">afschriften</span>

![](../assets/images/itsppt/IT Suite voor non profits34.png)

Transacties MT940

![](../assets/images/itsppt/IT Suite voor non profits35.png)

Tool extensies\(te integreren in C\.R\)

<span style="color:#000000">Outlook/Exchange</span>

<span style="color:#000000">Jaarrooster module</span>

<span style="color:#000000">Competenties support module</span>

<span style="color:#000000">Contributie</span>  <span style="color:#000000">module</span>

<span style="color:#000000">Boekhouding</span>  <span style="color:#000000">module</span>

__Overzicht IT\-componenten__

## C.R Releases

### Actuele wijzigingen

* Inkomende gegevens
  * Leden gegevens van overschrijven naar vergelijken\.Hierdoor hebben wijzigingen in de structuur van Sportlink geen impact meer op de tool\.Met name met de wijziging van Java Web Start app naar Web app\.
* Uitgaande gegevens
  * Van VBA IE koppeling naar CSV bestanden\.Hierdoor kunnen ontwikkelingen van de tool doorgaan zonder dat deze koppeling stuk kan gaan\.
* Uitfaserenvan de Excel bewakingstool
  * Hierdoor wordt het gebruik van de data buiten de tool \(CSV/Excel\) beperkt tot een select aantal gebruikers binnen het bestuur enCSz\.
  * Omhelst het bouwen van een competentie beheer en toekenningssysteem \(70%\)
  * Omhelst een eenmalige ‘migratie’ van een deel van de reeds in Sportlink verlengde competenties door deze in de tool nogmaals te verlengen\.
* Na bovenstaande wijzigingen volgt het technisch herschikken van de tool naarafgekaderdemodules\.
  * Hierna kanonderhoud per module door een aparte ontwikkelaar plaats vinden\.

### Release schema

### Ontstaan en doorontwikkeling van de IT Suite en Club.Redders

* Ontstaan IT Suite
  * Geleidelijk aan ontstaan op basis van best\-practicebij de ontwikkeling vanClub\.Redders
  * Bestaande gratistoolingover low\-costtoolingover bouwen
* OntwikkelingClub\.Redderstot en met 2020
    * 2015start ontwikkelingentool in Excel
    * 2016 tool omgebouwd naar PHP
    * 2017 toevoeging vanMachForm
    * 2018 toevoeging van Office 365
    * 2019 integratie vande diverse componenten tot één geïntegreerde omgeving
    * 2020 pre\-seizoen koppelingen tussen componenten ombouwen/omgebouwd zodat deze zelfstandig van elkaar blijven werken
    * 2020 post\-seizoen ombouwen van de tool naar een modulaire inrichting t\.b\.v\. betere code en doorontwikkeling \(future\-proofing\)
* OntwikkelingClub\.Reddersvanaf 2021 en verder
  * Ontwikkeling volgens Proces\-Architectuur\-Optimalisatie principe
    * Pre\-seizoen worden proces \(functionaliteiten\) toegevoegd in de diverse modules
    * Tijdens het seizoen worden \(op de achtergrond in OTA\) technische verbeteringen doorgevoerd
    * Na het seizoen worden de functionele en technische wijzigingen geoptimaliseerd
      * Functioneel door input vanuit het seizoen door te voeren in de modules
      * Technisch door de technische verbeteringen in decoreuit te lijnen met de modules en de IT suite

### Proces-Architectuur-Optimalisatie cyclus

* Proces cyclus
  * Januari t/m april \(pre\-seizoen\)
  * Doel: toevoegen functionaliteiten aan diverse modules\, geen wijzigingen in decore\.
  * Deadline wijzigingsverzoeken: 1 november\.
    * Om verzoeken goed voor te bereiden dienen deze 2 maanden vooraf bekend te zijn\.
* Architectuur cyclus
  * Mei t/m augustus \(tijdens seizoen\)
  * Doel: doorvoeren van technische verbeteringen aan decore\, geen nieuwe functionaliteiten\.
  * Deadline wijzigingsverzoeken: 1maart\.
    * Om verzoeken goed voor te bereiden dienen deze 2 maanden vooraf bekend te zijn\.
* Optimalisatie cyclus
  * September t/m december \(post seizoen\)
  * Doel: verbeteren van bestaande functionaliteiten en technische uitlijning tussen de diverse modules en decore\.
    * Indien van toepassing ook het optimaliseren van de componenten binnen de IT Suite\.
  * Deadline wijzigingsverzoekentechnisch: 1september\.
    * Deze verzoeken ontstaan vanuit de wijzigingen in de architectuur cyclus en zijn z\.s\.m\. bekend bij de module ontwikkelaars\.
  * Deadline wijzigingsverzoeken functioneel: 15 september\.
    * Deze verzoeken ontstaan vanuit de ervaringen in het seizoen en dienen uiterlijk 2 weken hierna bekend te zijn bij de module ontwikkelaars\.

### Gantt chart model 1

<span style="color:#A6A6A6">Task bars \(length = duration\)</span>

<span style="color:#A6A6A6">To change the length of the duration bars go to Format/Size \(on far right\)\.</span>

To change the length of the duration bars go to Format/Size \(on far right\)\. For  extreme length changes\, ungroup the duration bars and scale the highlight independently\.

Task bars \(length = duration\)

## C.R Modules

### Club.Redders met modulaire opzet

Functionaliteiten

Alle functionaliteiten die niet worden ondersteund door reeds beschikbare software\.

* Corecomponenten
  * Generieke technische functionaliteiten
  * Bruikbaar in alle modules
  * Gedeeltes van modules kunnen t\.z\.t\. overgaan naar decore
* Modules
  * Bevatten één enkele functionaliteit
  * Kunnen los van elkaar en decoreontwikkeld worden
  * Maken geen gebruik van andere modules
    * M\.u\.v\. dejaarroostermodule\(afhankelijk vancompetentiesmodule\)

Afhankelijkheden

Office 365

MachForm

WordPress\(indien gebruik wordt gemaakt van deplugin\)

Architectuur

Ruud Borghouts\.

Sander de Boer\.

__Optimization__  __Sep\-Dec__

__Architecture Mei\-Aug__

### Module: Core

Functionaliteiten

Maakt het mogelijk dat module ontwikkelaars zich kunnen focussen op het bouwen van functionaliteiten\.

* Dezecorebiedt de volgendetechnische functionaliteiten;
  * Logging
  * DBConnections
  * Environment variabelen
  * SMTP
  * RBAC \(todo\)
* Afhankelijkheden;
  * Indien van toepassing zijn deze als software bibliotheken toegevoegd aan decorem\.u\.v\.;
    * IdPfunctionaliteit\, wordt geboden door Office 365 /AzureActive Directory
    * WYSIWYG formulier editor met procesflow functionaliteit\, geboden doorMachForm\(intern gebrand totClub\.Forms\)

Afhankelijkheden

PHP

MariaDB

Apache \(\.htaccess\)

Microsoft Graph \(O365\-API\)

MachFormPOST\-API

Ontwikkelaars

Ruud Borghouts\.

Sander de Boer\.

### Module: Mijn C.R

Functionaliteiten

Inzage in eigen gegevens

Toegang tot documenten

Toegang tot formulieren

Toegang tot overige tools

* Deze module biedt de volgende mogelijkheden;
  * Inzage persoonlijke gegevens
  * Inzage bewakingshistorie
  * Inzage verenigingsdiploma’s
  * Inzage bondsdiploma’s
  * Inzage bondsfuncties
  * Inzage in declaraties \(in ontwikkeling\)
  * Toegang tot intern gedeelde documenten
  * Toegang tot gekoppelde \(pre\-filled\) formulieren
* Afhankelijkheden ;
  * Core
  * Import van gegevens uit extern leden administratie systeem

Afhankelijkheden

Core\.

Import gegevens 3rd party

Ontwikkelaars

_Ruud Borghouts\._

_Sander de Boer\._

FactSheet

### Module: Mijn C.R – WordPress plugin

![](../assets/images/itsppt/IT Suite voor non profits36.png)

Functionaliteiten

Whitelabeling

* Deze module biedt de volgende mogelijkheden;
  * Biedt de mogelijkheden van Mijn C\.R aan binnen eenWordPresswebsite\. Hierdoor zien eindgebruikers niet dat de gegevens vanuit een ander pakket worden aangeboden\.
* Afhankelijkheden ;
  * Originele Mijn C\.R module

Afhankelijkheden

Core\.

ModuleMijn C\.R

Ontwikkelaars

_Ruud Borghouts_  _\._

### Module: Competenties

![](../assets/images/itsppt/IT Suite voor non profits37.png" width=48px />

Functionaliteiten

Beheer van competenties\.

* Deze module biedt de volgende mogelijkheden;
  * Beheer van beschikbare competenties
  * Toekennen van beschikbare competenties
  * Inzage van decompetentiekaart
* Afhankelijkheden ;
  * Core
  * Import van gegevens uit extern leden administratiesysteem voor zover deze ingezet dienen te worden als instroom eisen\.
  * Excel Competenties supportsubmodule
    * De online module ondersteund nog geen controle op instroom eisen\.

Afhankelijkheden

Core\.

Import gegevens 3rdparty

Excel Competenties supportsubmodule

Ontwikkelaars

_Ruud_  _Borghouts\._

Excelsubmodulewordt beheerd doorCSz\.

### Module: Jaarrooster

![](../assets/images/itsppt/IT Suite voor non profits38.png" width=48px />

Functionaliteiten

Roosteren

* Deze module biedt de volgende mogelijkheden;
  * Inlezen van rooster voorkeuren en bijbehorendecompententiesvan leden om zo een rooster samen te stellen\.
* Afhankelijkheden ;
  * Competenties module \(enigste module met uitzondering\)\.Nog enkel beschikbaar alsExcel module voor zoverde gegevens daaruitingezet dienen te worden alsroostereisen\.
  * Dient nog omgezet te worden naar een rooster applicatie \(MicrosoftShifts/Diensten\) of rooster module\.

Afhankelijkheden

Competenties module\.

Excel\.

Ontwikkelaars

PHP module niet beschikbaar\.

Excelmodulewordt beheerddoorCSz\.

### Module: Weekrooster

Functionaliteiten

Week roosters maken\.

* Deze module biedt de volgende mogelijkheden;
  * Inzien rooster gegevens van leden per week\.
  * Roosteren van leden op basis van deze gegevens\.
  * Genereren van een roosterlayoutop basis van roostering\.
* Afhankelijkheden ;
  * Core

Afhankelijkheden

Core\.

Ontwikkelaars

_Ruud Borghouts\._

_Sander de Boer\._

### Module: Pasfotos

Functionaliteiten

Pasfotosbeheren van leden\.

* Deze module biedt de volgende mogelijkheden;
  * Uploaden van pasfoto voor leden door kaderleden\.
  * Uploaden van eigen pasfoto door leden\.
  * Zowel intern als t\.z\.t\. via MicrosoftGraph\.
* Afhankelijkheden ;
  * Core

Afhankelijkheden

Core\.

Ontwikkelaars

_Ruud Borghouts\._

_Sander de Boer\._

### Module: Maillijsten

Functionaliteiten

Mail lijsten maken\.

* Deze module biedt de volgende mogelijkheden;
  * Genereren van maillijsten op basis van vooraf aangevraagde selectie criteria\.
* Afhankelijkheden ;
  * Core

Afhankelijkheden

Core

Ontwikkelaars

_Sander_  _de Boer\._

### Module: Data import

Functionaliteiten

CSV dataimports\.

* Deze module biedt de volgende mogelijkheden;
  * Importeren van gegevens uit externe leden administratie systemen\.
  * Importeren van bankgegevens t\.b\.v\. boekhouding\.
  * Importeren van jaarrooster gegevens uit Excel tool\.
* Afhankelijkheden ;
  * Core
  * Velden\, veldnamen en veldformat vereisten\.

Afhankelijkheden

Core\.

Ontwikkelaars

Gelijk aancore\.

### Module: Data export

Functionaliteiten

Extern beschikbaar stellen van vertrouwelijke gegevens\.

* Deze module biedt de volgende mogelijkheden;
  * Exporteren van bepaalde gegevens sets t\.b\.v\. het gebruik in Excel tools \(componenten welke functies bevatten die nog niet als module binnenClub\.Reddersbeschikbaar zijn\)\.
* Afhankelijkheden;
  * Core
  * Documentatie van de export bestanden
* Ondersteund;
  * Excel Jaarroostermodule \(CSz<10 personen\)
  * Excel Competenties supportsubmodule\(CSz<10personen\)
  * Excel Contributiemodule \(bestuur <5personen\)
  * Excel Boekhoudingmodule \(bestuur <5personen\)

Afhankelijkheden

Core\.

Documentatie van export bestanden\.

Ontwikkelaars

Gelijk aancore\.

### Module: PDF-merger

Functionaliteiten

Samenvoegen van PDF bestanden\.

* Deze module biedt de volgende mogelijkheden;
  * Samenvoegen van PDF bestanden tot één bestand\.
* Afhankelijkheden ;
  * Geen\.

Afhankelijkheden

Geen\.

Ontwikkelaars

Wouterde Boer\.

### Module: Contributie

![](../assets/images/itsppt/IT Suite voor non profits39.png" width=48px />

Functionaliteiten

Contributie inning en registratie\.

* Deze module biedt de volgende mogelijkheden;
  * Genereren van een overzicht met te innen contributies\.
  * Registreren van het negatieve contributie saldo per lid\.
  * Genereren van een SEPA\-XML \(via Excel\)\.
  * Registreren van het positieve contributie saldo per lid\.
  * Registreren van storneringen en stortingen per lid\.
* Afhankelijkheden ;
  * Core
  * ExcelContributiemodule
    * De online module ondersteund nog geen directe exporteren naar een SEPA\-XML bestand\.

Afhankelijkheden

Core\.

Excel Contributie module

Ontwikkelaars

_Ruud Borghouts\._

\(Externe\) Excelmodule wordt beheerddoor:RonaldFerdinandus\.

### Module: Boekhouding

![](../assets/images/itsppt/IT Suite voor non profits40.png" width=48px />

Functionaliteiten

Boekhouden

* Deze module biedt de volgende mogelijkheden;
  * Boekhouden
* Afhankelijkheden ;
  * Core
  * ExcelBoekhoudingmodule
    * De online module ondersteund nog geenjournaalposten en weergave van de W&V rekening\.

Afhankelijkheden

Core\.

ExcelBoekhoudingmodule

Ontwikkelaars

Ruud Borghouts\.

Excel module wordt beheerd door: Ruud Borghouts\.

## C.R Generaties

Generatie / release

### Sheet TOELICTING

<span style="color:#000000">Externe IT componenten</span>

<span style="color:#000000">Beveiligings laag</span>

<span style="color:#000000">Front\-end / Gebruikersomgeving</span>

Pictogrammen

Persoonlijk account

Persoonlijk account 3de

Legacyomgeving

Doel omgeving

Externe omgeving

Interne omgeving

Database

LDAP\*

Data stroomrichting  >

Data stroom richting <>

\*\) Identiteits\- entoegangsbeheer database

![](../assets/images/itsppt/IT Suite voor non profits41.png)

![](../assets/images/itsppt/IT Suite voor non profits42.png)

1egeneratie – fase 1

### Concept met Excel front- & back-end

Concept tool

Bestuur/commissieshadden:

Toegang tot Dropbox waar de leden adm\. Excel werkboek was opgeslagen\.

Handmatig wijzigen van hetjaarroosterin de Excel\-gegevens\.

Weekroostersautomatisch aanmaken met de Excel tool\.

Handmatig alle Access data gemigreerd naar een Excel\-bestand met dezelfde functionaliteit\.

![](../assets/images/itsppt/IT Suite voor non profits43.png)

![](../assets/images/itsppt/IT Suite voor non profits44.png)

![](../assets/images/itsppt/IT Suite voor non profits45.png)

Dataverwerking

Geen ondersteuning meer op de Access database\.

Beheer van alle gegevens in één enkel Excel werkboek\.

__2015__  __pre\-seizoen__

__2015__  __post\-seizoen__

1egeneratie – fase 2

### PHP back-end met Excel front-end

![](../assets/images/itsppt/IT Suite voor non profits46.png)

Nieuwetool

Bestuur/commissiesacties:

Gedeelde toegang tot C\.R met Sportlink data import/export functies\.

Via C\.R toegang tot het Excel werkboek in plaats van Dropbox\.

Ondersteuning voor competentiekaarten in de Excel tool\.

Toegang tot Sportlink om competenties toe te voegen\.

![](../assets/images/itsppt/IT Suite voor non profits47.png)

![](../assets/images/itsppt/IT Suite voor non profits48.png)

![](../assets/images/itsppt/IT Suite voor non profits49.png)

Dataverwerking

Handmatig met exports uit Sportslink in C\.R en vervolgens handmatig de gegenereerde data terug in Sportlink te zetten\.

__2016__  __pre\-seizoen__

__2016__  __post\-seizoen__

2egeneratie – fase 1

### DB back-end met PHP & Excel front-end

![](../assets/images/itsppt/IT Suite voor non profits50.png)

* Autorisaties
* Ledenkregen:
* Toegangtot de website
  * Mijn TRB\.nu
  * Club\.Redders
* Bestuur/commissieshebben:
* Ledentoegangen;
* Toegang tot Sportlink
* Extra rechten op de website\,MachFormen inClub\.Redders

<span style="color:#000000">WordPress</span>

<span style="color:#000000">Mijn TRB\.nu</span>

![](../assets/images/itsppt/IT Suite voor non profits51.png)

<span style="color:#000000">https://trb\.nu/clubforms</span>

![](../assets/images/itsppt/IT Suite voor non profits52.png)

Dataverwerking

Handmatig met exports uit Sportslink in C\.R en vervolgens handmatig de gegenereerde data terug in Sportlink te zetten\.

__2017__  __pre\-seizoen__

__2017__  __post\-seizoen__

### Implementatie Office 365

![](../assets/images/itsppt/IT Suite voor non profits53.png)

* Autorisaties
* Ledenhebben:
* Toegangtot de website
  * Mijn TRB\.nu
  * Club\.Redders
* Bestuur/commissieshebben:
* Ledentoegangen;
* Toegang tot Sportlink
* Extra rechten op de website\,MachFormen inClub\.Redders

<span style="color:#000000">WordPress</span>

<span style="color:#000000">Mijn TRB\.nu</span>

![](../assets/images/itsppt/IT Suite voor non profits54.png)

<span style="color:#000000">Active Directory</span>

<span style="color:#000000">https://trb\.nu/clubforms</span>

![](../assets/images/itsppt/IT Suite voor non profits55.png)

Nieuwefuncties

Mailbox en Teams voor kader\, functionarissen en ledenraad\.

2egeneratie – fase 2

### Geïntegreerde IT suite met 1ID/SSO

![](../assets/images/itsppt/IT Suite voor non profits56.png)

* Autorisaties
* Ledenhebben:
* Toegangtot de website
  * Mijn TRB\.nu
  * Club\.Redders
* Bestuur/commissieshebben:
* Ledentoegangen;
* Toegang tot Sportlink
* Extra rechten op de website\,MachForm\, C\.R en Office 365\.
* Functionarissen en ledenraad;
* Leden toegang en;
* Toegang tot O365\.

<span style="color:#000000">WordPress</span>

<span style="color:#000000">Mijn TRB\.nu</span>

![](../assets/images/itsppt/IT Suite voor non profits57.png)

<span style="color:#000000">Active Directory</span>

<span style="color:#000000">https://trb\.nu/clubforms</span>

![](../assets/images/itsppt/IT Suite voor non profits58.png)

Nieuwefuncties

1 gebruikersnaam voor alle IT accounts en één account \(O365\) waar mogelijk\.

M\.u\.v\.MachFormenkel gratis software binnen de Suite\.

__2019__  __pre\-seizoen__

__2019__  __post\-seizoen__

3egeneratie – fase 1

### Tool zonder externe afhankelijkheden

![](../assets/images/itsppt/IT Suite voor non profits59.png)

* Autorisaties
* Ledenhebben:
* Toegangtot de website
  * Mijn TRB\.nu
  * Club\.Redders
* Bestuur/commissieshebben:
* Ledentoegangen;
* Extra rechten op de website\,MachForm\, C\.R en Office 365\.
* Enkel secretaris heeft toegang tot Sportlink \(nodig\)\.

<span style="color:#000000">WordPress</span>

<span style="color:#000000">Mijn TRB\.nu</span>

![](../assets/images/itsppt/IT Suite voor non profits60.png)

<span style="color:#000000">Active Directory</span>

<span style="color:#000000">https://trb\.nu/clubforms</span>

![](../assets/images/itsppt/IT Suite voor non profits61.png)

Nieuwefuncties

C\.R is een volledig zelfstandig component binnen de IT Suite\.

__2020__  __pre\-seizoen__

__2020__  __post\-seizoen__

3egeneratie – fase 2

### Modulaire tool met P-A-O releases

![](../assets/images/itsppt/IT Suite voor non profits62.png)

* Autorisaties
* Ledenhebben:
* Toegangtot de website
  * Mijn TRB\.nu
  * Club\.Redders
* Bestuur/commissieshebben:
* Ledentoegangen;
* Extra rechten op de website\,MachForm\, C\.R en Office 365\.
* Opleiders krijgen t\.z\.t\.:
* Ledentoegangen;
* C\.R afteken module

<span style="color:#000000">WordPress</span>

<span style="color:#000000">Mijn TRB\.nu</span>

![](../assets/images/itsppt/IT Suite voor non profits63.png)

<span style="color:#000000">Active Directory</span>

<span style="color:#000000">https://trb\.nu/clubforms</span>

![](../assets/images/itsppt/IT Suite voor non profits64.png)

Nieuwefuncties

Ontwikkeling van C\.R kan plaatsvinden in P\-A\-O releases waardoor functionaliteiten en technische verbeteringen elkaar niet in de weg zitten\.

__Optimization__  __Sep\-Dec__

__Architecture Mei\-Aug__

3egeneratie – fase 2

Nieuwein C\.R

Corefunctionaliteiten:

Coreis losgekoppeld van modules\.

Modulefunctionaliteiten:

Modules zijn nu los van elkaar te onderhouden\.

Excel tools:

Maken voor zover deze \(nog bestaan\) gebruik van een vaste set CSV bestanden vanuit C\.R en tools dienen z\.s\.m\. omgebouwd teworden in PHP\.

Nieuwin IT Suite

Suite blijft ongewijzigd\.

__Optimization__  __Sep\-Dec__

__Architecture Mei\-Aug__

### Openstaande punten m.b.t. full-saas

* Club\.Redders
  * Enigste component dat niet als SAAS oplossing kan draaien\.
  * Vereist gereedkomen API koppelingen met alle componenten\.
  * Tenant ID & Tenant ID filter binnen de database en query's\.

![](../assets/images/itsppt/IT Suite voor non profits65.png)

### Eisen online boekhoudpakket

Werkt\-getest

Akounting\.

* Software eisen;
  * CSV import vantransactiesmetattributen\.
  * MT940 import vantransactiesmetattributen\.
* Taken/kennis eisen IT functionaris;
  * Installatie en updates van PHP software pakketten op een webserver\.
  * Apache\,MariaDB\,phpMyAdmin\.

Werkt\-nietgetest

Geen producten bekend\.

Werktniet\-getest

Geen producten bekend\.

