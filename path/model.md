Model
=====
genesix affected tables:
* pedcab : commande client fournisseur 
* peddet : commande reçue partiellement ou entièrement
* pwb_plan_recep : appointment
* com_alb : reçus des commandes (bon de réception)
* com_alb_dep : montant par famille
* pwb_even_com : l’historique des informations d’une commande
* prove : table des fournisseur
* cde_clifour: table de liaison commande_fournisseur/client
* pla_tracab : table des transferts


Command
=======
* id
* Appointment id nullable
* denied boolean
* central/warehouse
           

Appointment
===========

* warehouse_id
* user
* command_id 
* delivery_expected
* delivery_date
* delivery_time
* delivery_today
* delivery_mode
* delivery_type
* first_reception_date
* last_reception_date
* provider_name
* provider_code
* Nb ligne rupture	
* package_quantity
* pallet_quantity
* Comment

pwb_plan_recep
==============
* cod_emp          		decimal(8,0)   	code société                             
* num_enreg       		decimal(12,0)  	num cmd frn ou transfert ou bon de récep 
* num_ini         		decimal(12,0)  	Num cde et transfert initiale            
* cod_pro         		decimal(8,0)   	num fournisseur                          
* nom_fournisseur 		char(20)       	nom fournisseur                          
* cod_pto         		decimal(4,0)   	point de gestion                         
* date_livraison  		date           	date liv prévue fec_pre ou fec_tra       
* type            		decimal(2,0)   	1 commande 2 transfert                   
* date_debut      		date           	date début rendez-vous                   
* date_fin        		date           	date fin rendez-vous                     
* heure_debut     		char(5)        	heure début rendez-vous                  
* heure_fin       		char(5)        	heure fin rendez-vous                    
* full            		decimal(1,0)   	rendez-vous dans la journée              
* nb_colis        		decimal(8,0)   	nombre de colis                          
* nb_pal          		decimal(8,0)   	nombre de palette                        
* nb_rupture      		decimal(8,0)   	nombre de ligne en repture               
* date_rel        		date           	date liv reliquat                        
* date_recep      		date           	date de la réception                     
* tip_liv         		char(3)        	mode de livraison STD CRD cross docking  
* cmd_supprimer   		char(1)        	cmd supprimer                            
* cmd_refuse      		decimal(1,0)   	cmd refusé                               
* type_recep        		char(1)        	C = num_ped num_tra / R = reg_mov 

Warehouse
=========
id
type
