![](RackMultipart20200914-4-eojfhr_html_951cb241d90d6b5b.png)

# **Werkinstructie
 MachForm/Okta beheer**

| **Auteur** | Ruud Borghouts |
| --- | --- |
| **Eigenaar** | Ruud Borghouts |
| **Rubricering** | |
| **Type document** | |
| **Versie** | 0.03 |
| **Datum** | 7-april-2020 |
| **Officieel goedgekeurd door** | |
| **Goedgekeurd in/op** | Niet van toepassing |

# Inhoudsopgave

**[1](#_Toc37155699)****Uitgangspunten 3**

**[2](#_Toc37155700)****Gebruikersbeheer 4**

[2.1Attribute mapping vanuit Office 365. 4](#_Toc37155701)

**[3](#_Toc37155702)****SSO with AAD (through Okta) configuratie 5**

[3.1Algemeen 5](#_Toc37155703)

[3.2MachForm role to Azure AD group map 5](#_Toc37155704)

[3.3Okta Configuration 5](#_Toc37155705)

[3.4Azure Configuration 5](#_Toc37155706)

1.
# Uitgangspunten

Binnen de IT Suite voor non profits is voor [MachForm](https://wordpress.org/download/) gekozen als WYSIWYG formulieren editor. MachForm kan geheel naar eigen inzicht worden ingericht (met o.a. workflows etc.) maar vereist als onderdeel van de suite 3 basis formulieren (welke niet zonder impact op Club.Redders kunnen worden aangepast;

- Inschrijfformulier
- Doorlopende machtiging SEPA
- Uitschrijfformulier

Optioneel geld dit ook voor het &quot;Administratie formulier YYYY&quot; indien de declaratie module wordt gebruikt.

In dit document is uitgegaan van het volgende;

- De Office 365 omgeving is ingericht volgens de werkinstructie Office 365 beheer.
- MachForm is geïnstalleerd en up to date.
- Het SASL adres uit O365 is vereist voor het verzenden van E-mail berichten vanuit MachForm ([noreply@trb.nu](mailto:noreply@trb.nu)).
- De vereiste formulieren zijn geconfigureerd volgens dit document.
- Binnen Office 365 zijn de applicatie groepen aangemaakt volgens dit document.
  - In tegenstelling tot de werkinstructie Office 365 beheer worden voor externe applicaties wél andere groepen aangemaakt dan z.g.n. Office 365 groepen, namelijk security groups. Deze worden aangemaakt vanuit;
    - Het beheercentrum – groepen;
      - Met een naam volgens de volgende naamconventie;
        - App\_ als indicatie voor externe rechten groepen.
        - \&lt;NaamApplicatie\&gt;\_ naam van de externe applicatie.
        - \&lt;NaamApplicatieRol\&gt;\_ naam van de rol in de applicatie.
      - Bijvoorbeeld: App\_MachForm\_Administrator voor de applicatie MachForm en de rol Administrator in die applicatie.
      - Als beschrijving kan worden gekozen om de officiële beschrijving van de rechtengroep toe te voegen uit de documentatie van de betreffende applicatie.
    - Na het aanmaken van de groep kan deze worden voorzien van eigenaren en leden. Zoals gesteld in de werkinstructie Office 365 beheer zijn Verder zijn de eigenaren van de Office 365 groepen zelf verantwoordelijk voor het op en afvoeren van gewijzigde (actieve) leden.
      - Voor de App\_ groepen wordt het beheer vooralsnog uitgevoerd door de IT functionarissen. Zij worden tot op heden ingesteld als eigenaar.
      - De leden worden toegevoegd en verwijderd op verzoek van het bestuur. Zie hiervoor ook de standaard toekenning onder gebruikersbeheer.

1.
# Gebruikersbeheer

Dit document houd de termen aan zoals gebruikt in de werkinstructie Office 365 beheer.

De volgende situaties zijn mogelijk bij het beheer van gebruikers;

- Instroom / nieuw lid.
  - Na het aanmaken van een account in O365 kan een lid hiermee inloggen in WordPress. Het account wordt daar automatisch aangemaakt vanuit O365. Standaard krijgt een lid daar de rol subscriber. Hiervoor hoeft de gebruiker niet in de groep App\_WordPress\_Subscriber te zitten,
- Doorstroom / lid krijgt, wijzigt of stopt met actieve functie.
  - Lid krijgt actieve functie.
 Het lid wordt toegevoegd of verwijderd uit de gewenste App\_ groep(en).
 Standaard wordt hiervoor nu gehanteerd;
    - IT: App\_MachForm\_Administrator
    - Bestuur: App\_MachForm\_Administrator
    - CieO: App\_MachForm\_User
    - CSz: App\_MachForm\_User

Deze wijzigingen worden niet standaard doorgevoerd in WordPress (niet gestest…). Log na de aanpassingen in O365 in op WordPress en _ **of** _ verwijder de betreffende
 gebruiker. Deze wordt bij de eerstvolgende aanmelding in WordPress opnieuw
 aangemaakt met de juiste rechten. _ **Of** _ zoek de gebruiker op en pas de
 rechtenwijzigingen ook door in WordPress zelf.

- Uitstroom / lid meld zich af.
  - Na het disabelen of verwijderen van het account in O365 kan een lid zich niet meer aanmelden in WordPress. Het account blijft (niet getest) wel in WordPress bestaan met de laatst toegekende rechten. Het advies is alle subscriber accounts periodiek te verwijderen. Voor leden die nog toegang nodig hebben wordt dit account automatisch opnieuw aangemaakt zodra zij weer inloggen.

  1.
## Attribute mapping vanuit Office 365.

De volgende attributen worden vanuit Office 365 overgenomen in MachForm;

- Login gegevens;
  - DisplayName Name
  - UserPrincipalName Username/Email Address
- Rollen
  - Alle rollen van de App\_MachForm\_ groepen waarvan de gebruiker lid is.

1.
# SSO with AAD (through Okta) configuratie

  1.
## Algemeen

LDAP Server OpenLDAP, ApacheDS, etc.

LDAP Hostname trb-nu.ldap.okta.com

LDAP Port 636
 Encryption Method SSL (ldaps://)

Base DN ou=users,dc=trb-nu,dc=okta,dc=com

Required Group(s)\* ?

Use LDAP Exclusively [O] ß Make sure all settings are valid!

\*) The groups, if any, that authenticating LDAP users must belong to.

  1.
## MachForm role to Azure AD group map

**WordPress Role O365 Group Name Azure AD Group Object ID**

App\_MachForm\_Administrator ?

App\_MachForm\_User ?

  1.
## Okta Configuration

Volg voor de configuratie van deze plugin aan de Okta zijde de handleiding:

[https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md](https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md)

  1.
## Azure Configuration

Volg voor de configuratie van deze plugin aan de Azure zijde de handleiding:

[https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md](https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md)

NOOT: BIJ VIMEXX HOSTING: ACTIVEER DE OPTIE LDAP BIJ DE PHP MODULES.

**V ![](RackMultipart20200914-4-eojfhr_html_1433a220122ab2c7.jpg) ersie 0.03 – 7 april 2020**