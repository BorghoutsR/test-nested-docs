![](RackMultipart20200914-4-1awdyd4_html_951cb241d90d6b5b.png)

# **Werkinstructie
 WordPress beheer**

| **Auteur** | Ruud Borghouts |
| --- | --- |
| **Eigenaar** | Ruud Borghouts |
| **Rubricering** | |
| **Type document** | |
| **Versie** | 0.04 |
| **Datum** | 14-juli-2020 |
| **Officieel goedgekeurd door** | |
| **Goedgekeurd in/op** | Niet van toepassing |

# Inhoudsopgave

**[1](#_Toc45630743)****Uitgangspunten 3**

**[2](#_Toc45630744)****Gebruikersbeheer 4**

[2.1Attribute mapping vanuit Office 365. 4](#_Toc45630745)

**[3](#_Toc45630746)****SSO with AAD (for WordPress) configuratie 5**

[3.1Algemeen 5](#_Toc45630747)

[3.2WordPress role to Azure AD group map 5](#_Toc45630748)

[3.3Advanced 5](#_Toc45630749)

[3.4Configuratie in Azure 5](#_Toc45630750)

**[4](#_Toc45630751)****Club.Rescue-WP configuratie 6**

[4.1Algemeen 6](#_Toc45630752)

[4.2Club.Rescue role to Azure AD group map 6](#_Toc45630753)

[4.3Advanced 6](#_Toc45630754)

[4.4Shortcodes 6](#_Toc45630755)

1.
# Uitgangspunten

Binnen de IT Suite voor non profits is voor [WordPress](https://wordpress.org/download/) gekozen als website/CMS. WordPress kan geheel naar eigen inzicht worden ingericht maar gebruikt als onderdeel van de suite 2 plugins;

- [SSO with AAD (for WordPress)](https://github.com/psignoret/aad-sso-wordpress) voor het opzetten van SSO vanuit Office 365.
- [Club.Redders-WP](https://github.com/clubrescue/clubrescue-wp) voor het integreren van de Mijn omgeving uit Club.Redders in WordPress.
 Deze plugin is alleen nodig indien je niet alle eindgebruikers wilt doorverwijzen naar de tool.

In dit document is uitgegaan van het volgende;

- De Office 365 omgeving is ingericht volgens de werkinstructie Office 365 beheer.
- WordPress is geïnstalleerd en up to date.
- Beide plugins zijn geïnstalleerd en up to date.
- De SSO with AAD plugin is geconfigureerd volgens dit document.
- Binnen Office 365 zijn de applicatie groepen aangemaakt volgens dit document.
  - In tegenstelling tot de werkinstructie Office 365 beheer worden voor externe applicaties wél andere groepen aangemaakt dan z.g.n. Office 365 groepen, namelijk security groups. Deze worden aangemaakt vanuit;
    - Het beheercentrum – groepen;
      - Met een naam volgens de volgende naamconventie;
        - App\_ als indicatie voor externe rechten groepen.
        - \&lt;NaamApplicatie\&gt;\_ naam van de externe applicatie.
        - \&lt;NaamApplicatieRol\&gt;\_ naam van de rol in de applicatie.
      - Bijvoorbeeld: App\_WordPress\_Administrator voor de applicatie WordPress en de rol Administrator in die applicatie.
      - Als beschrijving kan worden gekozen om de officiële beschrijving van de rechtengroep toe te voegen uit de documentatie van de betreffende applicatie.
    - Na het aanmaken van de groep kan deze worden voorzien van eigenaren en leden. Zoals gesteld in de werkinstructie Office 365 beheer zijn Verder zijn de eigenaren van de Office 365 groepen zelf verantwoordelijk voor het op en afvoeren van gewijzigde (actieve) leden.
      - Voor de App\_ groepen wordt het beheer vooralsnog uitgevoerd door de IT functionarissen. Zij worden tot op heden ingesteld als eigenaar.
      - De leden worden toegevoegd en verwijderd op verzoek van het bestuur. Zie hiervoor ook de standaard toekenning onder gebruikersbeheer.

- _Het SASL adres uit O365 kan indien_ _gewenst worden ingesteld voor het verzenden van E-mail berichten vanuit WordPress (_[_noreply@trb.nu_](mailto:noreply@trb.nu)_)._

1.
# Gebruikersbeheer

Dit document houd de termen aan zoals gebruikt in de werkinstructie Office 365 beheer.

De volgende situaties zijn mogelijk bij het beheer van gebruikers;

- Instroom / nieuw lid.
  - Standaard krijgt een lid geen rechten binnen WordPress.
- Doorstroom / lid krijgt, wijzigt of stopt met actieve functie.
  - Lid krijgt actieve functie.
 Het lid wordt toegevoegd of verwijderd uit de gewenste App\_ groep(en).
 Standaard wordt hiervoor nu gehanteerd;
    - Bestuur: App\_WordPress\_Editor
    - CieO: App\_WordPress\_Contributor
    - CSz: App\_WordPress\_Contributor
    - IT: App\_WordPress\_Administrator

Deze wijzigingen worden niet standaard doorgevoerd in WordPress (niet gestest…). Log na de aanpassingen in O365 in op WordPress en _ **of** _ verwijder de betreffende
 gebruiker. Deze wordt bij de eerstvolgende aanmelding in WordPress opnieuw
 aangemaakt met de juiste rechten. _ **Of** _ zoek de gebruiker op en pas de
 rechtenwijzigingen ook door in WordPress zelf.

- Uitstroom / lid meld zich af.
  - Na het disabelen of verwijderen van het account in O365 kan een lid zich niet meer aanmelden in WordPress. Het account blijft (niet getest) wel in WordPress bestaan met de laatst toegekende rechten. Het advies is om de IT functionarissen te verzoeken een WordPress account dat niet meer nodig is te laten verwijderen. Indien een gebruiker content heeft toegevoegd/bewerkt dient het eigenaarschap hiervan toegekend te worden aan een andere gebruiker. Kies hierbij bij voor de voorzitter van dezelfde eenheid (werkgroep/commissie/bestuur). Indien niet mogelijk kies dan de secretaris. Indien dat ook niet mogelijk is, kies dan de voorzitter van het bestuur.

  1.
## Attribute mapping vanuit Office 365.

De volgende attributen worden vanuit Office 365 overgenomen in WordPress;

- Login gegevens;
  - GivenName First Name
  - Surname Last Name
  - DisplayName Display name publicly as
  - UserPrincipalName Username/Nickname/Email
- Rollen
  - Alle rollen van de App\_WordPress\_ groepen waarvan de gebruiker lid is.

1.
# SSO with AAD (for WordPress) configuratie

  1.
## Algemeen

Display name Texelse Reddingsbrigade

Domain hint trb.nu

Client ID 115e93b9-98f9-4732-82bf-0cf79c0ed437

Client secret \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Redirect URL https://trb.nu/wp-login.php

Logout redirect URL https://trb.nu/

Enable full logout [X]

Field to match to UPN Login Name

Match on alias of the UPN []  do not enable this option!\*

Enable auto-provisioning [X]

Enable auto-forward to Azure AD [X]

Enable Azure AD group to WP role association [X]

Default WordPress role if not in Azure AD group (None, deny access)

\*) enabling matching on alias of the UPN will remove the domain name from the username. This will prevent apps based on WordPress authentication from matching usernames.

  1.
## WordPress role to Azure AD group map

**WordPress Role O365 Group Name Azure AD Group Object ID**

App\_WordPress\_Administrator d8d5c95d-edbe-4bef-a281-f4961770453d

App\_WordPress\_Editor 9fb802fc-c9f8-40f3-89f4-9eef560be839

App\_WordPress\_Author b77021ff-e1ca-40ca-94be-e23ee28d25d9

App\_WordPress\_Contributor 2ebcf8d9-a591-4d75-be50-502d3cc581ce

App\_WordPress\_Subscriber 37bc8060-df29-436a-b9c6-6e5f1996c253

  1.
## Advanced

OpenID Connect configuration endpoint :
 https://login.microsoftonline.com/common/.well-known/openid-configuration

  1.
## Configuratie in Azure

Volg voor de configuratie van deze plugin aan de Azure zijde de plugin handleiding:

[https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md](https://github.com/psignoret/aad-sso-wordpress/blob/master/README.md)

1.
# Club.Rescue-WP configuratie

  1.
## Algemeen

My Club.Rescue pages mijn-trb-nu

Whitelabel (OTAP) clubredders

Default source label activities

Default variable label activiteitenTable

Error message Mijn TRB.nu is tijdelijk niet beschikbaar i.v.m.
 onderhoud. Probeer het later nog een keer.

  1.
## Club.Rescue role to Azure AD group map

**Club.Rescue Role O365 Group Name Azure AD Group Object ID**

App\_ClubRedders\_Administrator 729fb8a2-8905-49e3-a0c9-d186890de1aa

App\_ClubRedders\_WP\_Editor 55ef8c35-f0ed-4a6e-8a84-ba4e21ba1ad5

App\_ClubRedders\_WP\_Contributor a790a850-c031-4847-a7e3-6fa27c526c3e

App\_ClubRedders\_Member 702eca77-824f-4dc1-99c4-7ae9b7f5be68

  1.
## Advanced

Club.Rescue link [X]

Branch (X) Master (default).

() Development (only for test environments).

  1.
## Shortcodes

De actuele uitleg van de beschikbare shortcodes is beschikbaar op de configuratie pagina:

[https://trb.nu/wp-admin/options-general.php?page=cr-wp](https://trb.nu/wp-admin/options-general.php?page=cr-wp)

De volgende shortcodes zijn (enkel) beschikbaar binnen de pagina&#39;s welke zijn toegevoegd onder de configuratie &#39;My Club.Rescue pages&#39;; [crwp\_mycr] geeft de standard submodule en dataset weer uit Mijn Club.Redders zoals geconfigureerd in de configuratie &#39;Default source&#39; en &#39;Default variable&#39;. Deze shortcode heeft drie attributen die kunnen worden gebruikt om de opgevraagde data te wijzigen:

[crwp\_mycr otap=&quot;clubredders&quot; source=&quot;mycr-attributes&quot; table=&quot;lidTable&quot;] otap bepaalt de folder van de Club.Redders installatie die gebruikt wordt. Handig om de installatie te White labelen of data uit een test installatie op te vragen. source bepaalt de Mijn C.R submodule die wordt ingevoegd. table bepaalt de dataset uit de submodule die teruggegeven wordt.

**V ![](RackMultipart20200914-4-1awdyd4_html_1433a220122ab2c7.jpg) ersie 0.04 – 14 juli 2020**