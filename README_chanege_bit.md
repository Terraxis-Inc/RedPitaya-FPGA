1. First export bit file and name it as red_pitaya_top.bit
2. Run this command "echo all:{ red_pitaya_top.bit } >  red_pitaya_top.bif" inside same folder as bit file.
3. Now run following command "bootgen -image red_pitaya_top.bif -arch zynq -process_bitstream bin -o red_pitaya_top.bit.bin -w"
4. Run "scp red_pitaya_top.bit.bin root@rp-f0908b.local:/root" it will copy .bit.bin file redpitaya.
5. Go to redpitaya terminal and look for this file in root folder.
6. Run "fpgautil -b ./red_pitaya_top.bit.bin" this command. It will upload bit file and give following prints.
	Time taken to load BIN is 37.000000 Milli Seconds
	BIN FILE loaded through FPGA manager successfully
