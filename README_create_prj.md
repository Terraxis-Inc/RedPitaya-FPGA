1. First git the project using "git clone git@github.com:Terraxis-Inc/RedPitaya-FPGA.git".
2. Go to the project directory and run "make project PRJ=classic MODEL=Z10".
3. After this it will create vivado project for classic.
4. When block design is done, in design source make sure red_pitaya_top is set as top.
5. Now run synthesis. After it is complete open synthsized design. Open I/O ports by Window->I/O Ports.
6. In I/O ports look if there is I/O std type set as default change it to its non default type.
7. After this run Generate Bitstream. It will Generate bit file.
