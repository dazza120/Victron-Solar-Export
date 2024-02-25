# Victron-Solar-Export
UK Spring to Summer Solar Export What Solar You Don't Use For Victron

This is a UK Mid Spring Solar Export enabled by lowering the DVCC in NodeRED during the summer months april the 1st to September the 1st (I had to include September to get the whole of August ) You can change the cron to match your country or increse the months i have left March out as its not one of the best month for solar in the UK. This does not force solar export it merely stops the batteries from taking all the solar which allows export 
Caviat ( IF YOU ARE NOT USING THE SOLAR IT WILL ALLOW THE EXCESS SOLAR TO GO TO THE GRID SO HOUSE LOADS WILL ALWAYS TAKE FROM SOLAR FIRST BEFORE EXPORT ) 
The Cron will start at 6am lowering the DVCC Charge to the batteries to 40Amps and lower it every 30mins till it reaches 5Amps DVCC charging current this has a failsafe if the grid goes down these crons will not work during the months and time on the cron, if the grid go down and you have PV on the AC1 out of the victron system it will return to Max DVCC charging and use the PV to charge your batteries at its max rate during the grid down period.
There is also a return to Max DVCC at the end of the day ie so that it can charge from the grid at its max rate during the Off Peak window. Mine is set to revert at 2130PM you can change this time to what you want.
Thanks goes to @matt1309
