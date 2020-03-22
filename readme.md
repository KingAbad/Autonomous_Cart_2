#Project - Atonomous cart

Het doel van het project is om van een alledaagse golf cart te automatiseren, en deze een autonome golf cart te maken dat binnen de Corda campus rondrijd . 

De bedoeling is dat er op de golf cart een touchscreen gaat zijn met een user interface. Op deze user interface komt er een map van de Corda campus met alle mogelijke gebouwen. De bestuurder kan via de touchscreen feature kiezen naar welk gebouw hij of zij zich wil verplaatsen. Er gaan ook smart LED’s zijn die de bestuurder gaan informeren over de obstakels die zich op de rijbaan bevinden. Bij een atonomous project hoort zeker ook een failsafe wat het mogelijk gaat maken om de controle terug aan de bestuurder te bezorgen.

De aanpak is als volgt. Het hart van de golf cart is de motorcontroller. De motorcontroller stuurt de nodige output signalen naar de motor, remmen enz. aan de hand van de inputsignalen van het gaspedaal, rempedaal enz. Er gaat voor gezorgd worden dat deze inputsignalen ‘gefaket’ kunnen worden om de cart dan autonoom te kunnen controleren. Deze ‘fake’ signalen gaan ingestuurd worden door middel van een PLC. 

Alle mogelijke routes gaan voorgeprogrammeerd worden. De cart weet dus welke wegen hij moet raadplegen en waar het moet afslaan. Corda cumpus is echter een actieve campus. Er worden evenementen georganiseerd of er lopen mensen rond. Natuurlijk moet het cart met deze variabelen rekening houden. 

Het opsporen van obstakels gaat gebeuren via sensoren en camera’s. Deze elektronica gaat rechtstreeks op de pinnen van de Jetson Nano geïnstalleerd worden. Er gaat code geschreven worden om mensen, muren en dergelijke op te sporen. 

De verkregen data moet door de Jetson Nano behandelt, en doorgestuurd worden als commando’s aan de PLC. De PLC moet ook kunnen communiceren met de Jetson Nano. Het moet kunnen bevestigen dat een bepaald commando is ontvangen en uitgevoerd aan de Jetson Nano. De communicatie tussen deze twee gebeurt via ethercat.

Hier komen alle nodige bestanden en code.
