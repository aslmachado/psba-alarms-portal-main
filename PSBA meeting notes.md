# Alarms portal summary

The PSBA Alarms portal  extracts alarms from PSBA Enigma System (ICT Monitoring System). 
It provides technical provides technical staff with an interactive interface to view alerts from alarms and nodes in PSBA's infrastructure such as node status and SNMP Traps. It features tools to assist in the browsing experience via filters, data visualisation and geolocation. For example it can display active alarms which also allow filtering by:
Agency (QAS / QFES / QPS) Site / Region (Cairns /Townsville / Kedron and so on) Type of Device (IP Radio, Circuit Brakes, Radios, Telephone PCs, UPS and so on)

It is developed as a custom SharePoint Framework (Microsoft's model for SharePoint development) web part and retrieves data from a document library that syncs read-only data from Enigma. The flow of data is read-only for all its functionality.

Custom SharePoint Framework solutions including extensions and web parts are deployed into SharePoint sites via the tenancy's app catalog (or a site specific app catalog which restricts apps to a single site). 
To deploy solutions into an app catalog, the .sppkg (solution package) file needs to be uploaded and checked in. 
After that, it will be available for site installation via the site's Site Contents.
Once available, it will appear alongside other SharePoint web parts when editing a page.
There is an existing solution for ICT Health in the PSBA app catalog https://psbaqld.sharepoint.com/sites/appcatalog

# PSBA meeting notes

## Current status

-Implemented interactive portal view
-Overview screen
-Based of data modelled from supplied data export
-Alert chart (app logic)
-Filters (app logic)
-Alert with history (app logic)
-Some missing data, BOSS ticket, Hardware maintenance contact
-Fullscreen display

### Made up stuff
-Map lat lng locations
-Priority
-Impact time

### Misc
-What are the visualisations?
-Dependent on available data

### Circuit view
-Some display and filtering logic implemented
-Design choice
-Circuit logic/schematic required

## Data source
-Access (internal env out, not in)
-API
-Schema
-Any available object models? For alerts, nodes and circuits


## Site_List fields
site_id					
site_name				
site_cst_id					
site_str_type			
site_com_dt					
site_tst		
site_ph			
site_ph_secondary					
site_comment
site_access_info						
site_power_info 						
site_owner_cst_id					
site_street_address	
site_street_address_aux					
site_code			
site_net_clients_count					
site_site_class_id				
site_site_sla_id					
site_contract_id				
site_status					
site_svc_code						
site_gps				
site_priority_id					
site_region_id					
cst_id						
cst_dsc				
cst_code					
site_class_dsc					
region_name			
contract_maindesc

## Node fields
hst_id	
hst_dsc
hst_namea
hst_cst_id
hst_rqstr
hst_rquts	
hst_admin
hst_sysName
hst_sysContact	
hst_sysLocation
hst_snmp_update_tst
hst_contract_id	
hst_upstream_hst_id	
hst_UpTime
hst_last_alive_tst
hst_added_tst	
hst_modified_per_id	
hst_modified_tst	
hst_snmp_sysdesc
hst_vendor_id	
hst_config_id
hst_nat_ip	
hst_dns_compliant_name
hst_connection_comment	
hst_status_tst		
hst_ovmgt_tst
hst_connection_comment_tst		
hst_sysObjectID
hst_priority_id		
hst_uuid
hst_parent_hst_id	
hst_central_hst_id		
hst_remote_hst_id
typ_dsc		
vendor_dsc		
model_dsc
status_dsc	
cst_dsc	
cst_code
site_name
site_code
site_class_dsc	
contract_maindesc		

