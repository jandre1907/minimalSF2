Planning Reception
==================

Login:
------
Login, password
* LDAP
* different access right exists

Homepage:
---------

Select a warehouse

file: siege.php

example:
`http://a19web-pdb09001/dev/planning_recep/app/siege.php?depot=090-SIEGE&sgi_user=S2536428&nom_user=Stephane%20Martin&debutsem=09/16/2014&jour=16&mois=09&annee=2014#`

form:
* date
* sessionid
* current store
* targeted store
* sgi LDAP


Popup
-----

Actions:
* display warning:
  * command -> always in error 
  * transfert

* display planning
* toggle by week/ by day
* list RDV by date
    * 00H
    * 5h-15H
* show details on RDV item
* five button :
  * take quick dating
  * take dating
  * consult dating (filters)
  * print
  * refresh planning

* LINKS:
  go to help
  
file: index.php

example:
`http://a19web-pdb09001/dev/planning_recep/index.php?depot=1&sgi_user=&nom_user=&debutsem=09/16/2014&jour=16&mois=09&annee=2014`

Help
----
* cmd reliquat bordeaux
* cmd receptionné orange
* cmd rupture rouge
* cmd rdv confirmé jaune
* cmd en attente de rdv noir
* cmd client vert
* transfert inter-depot bleu 

Take a Date
-----------
read datas:

* 16 September 2014 12:10 - V3.0        
* DEPOT : 4   
* S2***8   S*****e Ma**n

Form:
* Numéro de commande	   
* Date Livraison	
* Heure   
* Livraison ds la journée
* Nom fournisseur
* Code fournisseur	
* Date livraison prévue
* Date 1ère réception	
* Date dernière récep.
* Mode Livraison	
* Type livraison		
* Nb ligne rupture	
* Nombre de colis
* Nombre de palette	
* Commande refusée
* Cmd Centrale/Dépôt		
* Commentaire


Actions:
* show history
* show article
