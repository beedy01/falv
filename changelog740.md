#Changes V 740.1.0.14
Small change in mass replace function - data is no longer directly move to output table but only passed to grid by set_delta_celss method. This is done to avoid omitting event on_data_change 

#Changes V 740.1.0.13
Internal event for user comand handling was removed. Instead all code from this method was moved to evf_user_command, so you have to call super->evf_user_command if you want standard functions to work.Additionally hot spot bug with delayed events was solved.

#Changes V 740.1.0.12
Getters added for columns settings + get_cell_enabled method + some minor bugs

#Changes V 740.1.0.7 - 740.1.0.11
New demo program ZDEMO_FALV16 for check if FALV is working on split container, few bugs correction ( Loop in PAI, split container ).

#Changes V 740.1.0.6
new method "SEND" for sending grid as an XLSX attachment
correction of zcl_falv->export_to_excel 

#Changes V 740.1.0.4
Run in BG mode error solved.

#Changes V 740.1.0.3
Top_of_page event is now raised and handled.

Changed Classes: ZCL_FALV
Changed Programs: ZDEMO_FALV02, ZDEMO_FALV13

#Changes V 740.1.0.2
All event handlers methods were renamed to use prefix evf_* instead of evt_*. This was because some of super classes were already containing such methods and to keep one naming range I've used other prefix. 

Additionally issue with not showing grid on full screen at first call.  
