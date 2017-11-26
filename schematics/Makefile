%.ps : %.sch
	gschem -p -o $*.ps -s print.scm $*.sch
EtherCAT_ET1200.ps : EtherCAT_ET1200_power.ps EtherCAT_ET1200_PHY_ports.ps EtherCAT_ET1200_ASICs.ps EtherCAT_ET1200_uCs.ps 
	./psmerge $^ > $@

%.pdf : %.ps
	ps2pdf $< $@

