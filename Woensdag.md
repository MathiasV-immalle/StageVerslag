# Woensdag 4 Oktober 2017
### Remote Support
> Vandaag heb ik maar een half dagje gewerkt, tot 13u. Dit idee kwam van het bedrijf zelf omdat ze vaak merken dat studenten in het midden van de week toch wel extra tijd kunnen gebruiken om notities bij te werken. Maar dat wil niks zeggen dat ik op een half dagje niks heb kunnen doen. Vandaag kreeg ik zicht op de verschillende softwarepakketten die VanRoey.be gebruikt, en ook kreeg ik info over hun fysieke én virtuele servers. Jammer genoeg kreeg ik wegens privacy-regels geen plannetje van de server-indeling of screenshots van de programma's. Wel heb ik een afgewerkt Ticket gekregen van een medewerker zelf. Zo overtreed ik geen privacy-regels en kunnen er geen problemen met klanten ontstaan. Dit Ticket kan u onderaan terugvinden. Eerst vertel ik kort wat ik vandaag precies gezien heb.
##### Ticketingsysteem: Microsoft Navision
- Microsoft Navision is het programma dat VanRoey.be gebruikt als Ticketingsysteem. Tickets worden handmatig aangemaakt met input die verkregen wordt via e-mail, telefoon, of via een online portal: de website.
  - Eerst maak je een nieuw ticket aan en selecteer je de klant.
  - Vervolgens selecteer je het soort incident: Major Incident - Incident - Request Fulfilment
  - Vervolgens selecteer je een prioriteit: Zeer hoog - Hoog - Normaal - Laag
  - Hierna worden de gegevens van de gebruiker zelf (en dus niet van de bedrijfsleider of dergelijke) genoteerd, en kunnen er eventuele opmerkingen geplaatst worden.
- Enkele opmerkingen:
  - Sommige klanten kopen een SLA-contract. Hier bestaan twee versies: één van 1uur en één van 4uur. Dit wil zeggen dat wanneer een klant met een probleem dit contract heeft, VanRoey.be binnen de bijhorende termijn moet reageren op het probleem, anders zullen zij een boete moeten betalen. De SLA-contracthouders worden dus sneller geholpen dan klanten zonder dit contract.
  - Sommige klanten kopen een Service-contract. Dit houd in dat de klanten 24/24 en 7/7 geholpen moeten worden door VanRoey.be, dus ook in weekends en vakanties. Hiervoor worden er techniekers stand-by gehouden, dit werkt via een beurtrollensysteem.
  - VanRoey.be is momenteel aan het kijken naar een ander systeem waar ik de naam niet van mag weten, maar met dat programma zouden er veel tickets volautomatisch kunnen worden aangemaakt, en zo zouden er ook screenshots mee opgeslagen kunnen worden (wat tot nu toe niet mogelijk was).
##### Serverniveau: VMware
- VMware: Hypervisor. Via dit programma zet VanRoey.be zijn virtuele servers op zijn fysieke servers.
  - De cluster (groep samenwerkende servers) van VanRoey.be bestaat uit 4 fysieke servers met elk 140GB werkgeheugen (en andere details). Waarom deze servers elk zoveel werkgeheugen hebben is, wanneer er 3 servers uitvallen (uitzonderlijk) moet de overblijvende server alles op zichzelf kunnen draaien.
[VMWare](https://www.vmware.com/nl.html)
 ##### Securityniveau
- Fortinet: Security vendor. Vanroey.be heeft niet één, niet geen, maar twee firewalls (waarvan 1 reserve uiteraard) met de eerste failover door Telenet (omdat VanRoey.be een partner is van Telenet), en een tweede door bijvoorbeeld Proximus (hangt er een beetje van af).
[Fortinet](https://www.fortinet.com/)
##### Switchingniveau
- VanRoey.be heeft één core-switch, in een cluster met andere switchen. De core-switch is een stack van switchen: Allerlei switchen boven elkaar in één of meerdere kasten vlak naast elkaar. Dit brengt mooie voordelen met zich mee zoals betere performantie, en zo kunnen bijvoorbeeld ook twee poorten van 1gigabit gebundeld worden tot één poort van 2gigabit, wat zorgt voor een mooie Uplink.
##### Monitoringpakket
- Assurline is een eigen programma dat VanRoey.be gebruikt om servers van hun klanten te monitoren. Klanten die deze extra feature wensen, moeten uiteraard een betalend contract tekenen. 
[Assurline](https://www.vanroey.be/Projecten/210-assurline-beheers-uw-omgeving/)

> Hier ziet u een foto van mijn tijdelijke werkplaats vandaag:

![afbeelding](afb/Werkbasis.jpg)

*//elk puntje wordt geteld als zin -> 12 zinnen*

Klik [hier](https://github.com/MathiasV-immalle/StageVerslag/blob/master/Dinsdag.md) om Dinsdag 03/10/'17 te bekijken.

Klik [hier](https://github.com/MathiasV-immalle/StageVerslag/blob/master/Donderdag.md) om Donderdag 05/10/'17 te bekijken.
