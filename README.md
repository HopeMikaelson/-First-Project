# -First-Project
AutoHotKey  LOL  accept {color Rac} not complet

space::

loop {   ; First loop it makes it start when LoL is the first window when the (accept) comes 

      If WinActive("League of Legends") 
		break
     }

loop {                                               ; clicks the accept  color Rac
		mousemove 508, 441
		Pixelgetcolor, pix, 508, 441
		if pix = 0xF4F3C6
			break
      }

click 508, 441


loop  {                                              ; flash color Rac   for the chat
          mousemove 585, 542
          Pixelgetcolor, pix2, 585, 542
          if pix2 = 0x60FFFF
	        break  
      }
	  
	  
loop 10 {
        
        click 142, 542
	      send, mid{Enter}             
        }
sleep 5000
click 632, 84
sleep 500
send Katarina
sleep 500
click 315, 140
Esc:: ExitApp
return
F1:: Reload
ExitApp
