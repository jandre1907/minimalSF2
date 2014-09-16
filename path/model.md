Model
=====
genesix affected tables:
* pedcab : commande client fournisseur 
* tracab : transferts
* pwb_plan_recep : appointment
* com_alb : numéro de réception de la table

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
