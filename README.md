Terminology Terminal Emulator
  
        Last night I finally got sick of the same ole plain Jane terminal. I mean even if I add some color to it or made shortcuts or not matter how many scripts and binds I did. It was just boring! So I hopped on DuckDuckGo and searched around for a new one and "Terminology" is the one I decided on.        
        Now after tracking down the original developers I realized that with this fresh install on my odroid Im missing a lot of the dependencies to even be able to run this terminal. And the original developers hadnt exactly kept up with the dependencies names as they change over time so I went ahead and tracked down every single one of the dependencies and threw them into a little bash script for future use and thought I would share it with everyone here. Maybe save some people some time. 
 
 
        SO BEFORE BUILDING THE PACKAGE, IF YOU HAVENT CONFIRMED WHETHER OR NOT YOU HAVE ALL OF THE DEPENDENCIES INSTALLED ON YOUR MACHINE OR BETTER YET YOU KNOW YOU DONT. GO AHEAD AND FIND THAT BASH SCRIPT "TerminologyDepends.sh" and pop this in the terminal:
        
"chmod +x TerminologyDepends.sh"

        FOLLOW BY:
        
"sudo ./TerminalDepends"
  
  
 
        AFTER THAT HAS FINISHED GO AHEAD AND EXTRACT THE "e16-1.0.18.tar.gz" PACKAGE WITH:
        
"tar zxf e16-1.0.18.tar.gz"

        FOLLOW BY:
        
"./configure"
"sudo make"
"sudo make install"
"sudo ldconfig # needed on Linux to update linker library database"

                                                                                         -sLaveBOX-
      
       


