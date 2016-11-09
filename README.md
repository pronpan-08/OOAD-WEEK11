# OOAD-WEEK11
พรพรรณ  เกิดรัตน์ 57030201
State Diagram
รูปที่1
@startuml
title Blender
state "switch1ON" as switch1ON
switch1ON :  do/turn on the Blender
state "switch2ON" as switch2ON
switch2ON :  do/turn on the Blender
state "switch3ON" as switch3ON
switch3ON :  do/turn on the Blender
[*] --> switch1ON :turnON
[*] --> switch2ON :turnON
[*] --> switch3ON :turnON
switch1ON --> BlenderLow :switch on
switch2ON --> BlenderModerate :switch on
switch3ON --> BlenderLowFast :switch on
BlenderLow -->[*]
BlenderModerate -->[*]
BlenderLowFast -->[*]
@enduml

![](http://www.plantuml.com/plantuml/img/ZP5D2i8m48NtSugXIw68oQuBAIvS-NC0SH5ie8MOG3EbrtUYDIQMYfimUU_bcna2jIVLqt0t0DIHqRWpsZQw1zP9O-77ZcxjvdmgK7cCDuWLLeYDMzFGMtGMgLr0Y0mX8aByZv0PGaQ4_8cuhAvObbjC9WunVfqxOj6HYVEX17_gSN0ZLY-7koUB9PcZuoCiCmlA6MolFAMvf0q7UJZuXkRo6p6fDOlF7tu0)

รูปที่2
@startuml

title OpenComputer
state "switch1ON" as switch1ON
switch1ON :  do/turn on the computer
[*] -r-> switch1ON :TurnOn
switch1ON -r-> moniterON :switch on
moniterON -r->[*]
@enduml

![](http://www.plantuml.com/plantuml/img/JOun2uD038Nt_8g7Oq5ALuSYTEyjtKe7qO07NaxkSlZt6vLQjoJlUnzfitP9IvY8rEl4S3FB8uQvA2UoK1bLNhpsuyqzAtGPnqR7X0OOubLB4aI1Zep-vtXVFgXJVSU9VXdevDJVW135MsC5ziHSz3-kZCcePHcsX-aB)

รูปที่3

@startuml
title OpenElectricDrill
state "switch1ON" as switch1ON
switch1ON : do/ElectricDrill is rtate 
[*] --> switch1ON:turnOn
switch1ON --> ElectricDrillRotate :switch ON
ElectricDrillRotate -->[*]
switch1ON --> ElectricDrillIsnotRotate :switch OFF
ElectricDrillIsnotRotate -->[*]
@enduml

![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuIh9BCb9LV0lICrppKbDBYdAJ7Ofoip9uG8gA4bLK2ekpon9pZ3qzrDII2nMWFEuu2m5AuMKV7qKlGgPnGf5OErSqLgn2hgwTWYDLYMbHNd-UKZwGT8eseFomNgj84eKW9PXamPg0ngEpnpFuhpy4dJ3tDouS2g26kcGcfS22XakBW00)

รูปที่4

@startuml
title OpenCDplayer
state "switchCDtrayON" as switchCDtrayON
switchCDtrayON : do/open the CDtray
[*] --> switchCDtrayON:turnOn
switchCDtrayON -->CDtrayOpen :switchNO
state "switchCDtrayOFF" as switchCDtrayOFF
switchCDtrayOFF : do/open the CDtray
[*] --> switchCDtrayOFF:turnOn
switchCDtrayOFF -->CDtrayClose :switchOFF
CDtrayClose -->[*]
CDtrayOpen -->[*]
@enduml  

![](http://www.plantuml.com/plantuml/img/bP312eCm38RlUOhWSI2xzp04fKVx06E7CWCANIjjH7pxHNH3dPVTcZ_fbwyj4jl8myi1T-m8JK--h7fd9ueWFIRCqjZnioqhZdOoTOOsuJw2VOaAct0DGa9k2PSOxfS7vldjS5Nn4BtnHu8ChkUPefPkRKwDjFvLqXeEzHzIMfzQ2UEhLRgGwECrRzl6CYLSs3nWJGhoZNmr8W2y0G00)

รูปที่5

@startuml
title HairDryer
state "switcON" as switchON
switchON : do/turn on the Heating panels and  the Fan
[*] --> switchON:turnOn
switchON -->HeatingPanelsON
switchON -->FanON
FanON -->[*]
HeatingPanelsON -->[*]
state "switcOFF" as switchOFF
switchOFF : do/turn off the Heating panels and  the Fan
[*] --> switchOFF:turnOFF
switchOFF -->HeatingPanelsOFF
switchOFF -->FanOFF
FanOFF -->[*]
HeatingPanelsOFF -->[*]
@enduml  

![](http://www.plantuml.com/plantuml/img/bL4z3u8m5DpVhtXXD27k38R1D4xWJXmQAT847wPznFZlVHJvrCMbVRthNU_IrBDstDqROCkDmPEsxkXUne4GR33oJylNF8jGUmnpdMSm3fXWsUwvSuGj8TUYDvejtV2XoJGUDPKOSAK9Yjq5u_WmsIIzCAVPJSYF_XpaovU44mz1mjeVnGusrqTubLsfPNYbO9gMyQlgt_nA3GLMZbyLjcmVNx1X-rrZnbD3fVmD8W2y0G00)

รูปที่6

@startuml

title blender - Activity Diagram 
start
if (Press switch 1) then (yes)
  :soft;
else (no)
  if (Press switch 2) then (yes)
  :windy;
  else (no)
    if (Press switch 3) then (yes)
    :strong wind;
    else (no)
      :shut down;
    endif
  endif
endif
stop
@enduml

![](http://www.plantuml.com/plantuml/img/RP1D3e9038NtFSLRmiA5kfCD9Xx0Ao1Je0dCc6cHS7iPrCI_JTkylkyrQQbMHHk7diZ4UiQbP-yuOeDZRN8Jct6IgetL05gz90soSsHLw2HMTzZci8uzifar9-2WeR62k5T6vaEIVfZTDpE9TtEnJE_O7t3_1QPp5eDlaHAALVcCI8vkDBWm-UVUEsderHzLBLofNERqYpi0)

รูปที่7

@startuml
title Drill  Activity Diagram 
(*) --> "CHECK_SWITCH OFF"
 if "" then
         -->[TRUE] "STOP_Drill"
         STOP_Drill --> (*)
else
        -->[FALSE] "Drill_ON"
        Drill_ON --> (*)
      endif
@endum

![](http://www.plantuml.com/plantuml/img/JOz12u9048NlyoiUUwh0ln3AgXX5HXeT8cJ9jGPM3-iM-EzJoVHTXddptWT3VkkKTU_Qa6DdD1B55gNjj4NmSFnXro5azRIg1j5giuRdRI5a4ibzaLrtkKoGnh4WS0KXu5ww8KpgixVyV8dk45cUdehGiZ5Yli_cYEtnf4shQTcFWqCs0CPOaHxd-kJykrZej-Ycv8h8x-Vmv1S0)

รูปที่8

@startuml
title Hair dryer Activity Diagram 

(*) --> "CHECK_SWITCH OFF"
 if "" then
         -->[TRUE] "STOP_FAN"
         STOP_FAN --> (*)
else
        -->[FALSE] "CHECK_SWITCH_degreeheat = 0"
        if "" then 
            -->[TRUE]"START_FAN"
            START_FAN --> (*)
        else
            -->[FALSE]"STOP_FAN"
            
        endif
endif
@enduml

![](http://www.plantuml.com/plantuml/img/RP312e9048RlynJ3dYeGUe52iSGeCjJe425BZhgW7jOjyErRBLkDvZ0BC_l_yys0tIWkrQCgGGbL4lfSI4nbInATkn9FeLhS29vBNY70R357oreZS_sjkq-YoovsVGmyZm6A31b3LL0DE8J-Uut3y_Q6B8g3K-8vHsQwGwctrDP0PKCmrdhE8Uh4ut59IhaaAeWhNE7I-1a0D3F649h12UCVY9xZK_w239q9q1Jgtq8wZBHEHGRlREkdE_4B)

รูปที่ 9


@startuml
title CdPlayer Activity Diagram 

(*) --> "CHECK_SWITCH OFF"
   
    if "" then
         -->[TRUE] "END"
         
        
    else
        -->[FALSE] "CHECK_SWITCH_OPenClose_tray = 0"
                if " " then 
                        -->[TRUE]"END"
                else
                    -->[FALSE]"trayOpen"
                    -->"CHECK_SWITCH_OPenClose_tray = 0"
                        --> if " " then
                                -->[TRUE] "END"
                            else
                                -->[FALSE]"trayClose"
                                trayClose --> (*)
                                END --> (*)
                            endif
          
                endif
    endif

@enduml

![](http://www.plantuml.com/plantuml/img/bP9XIyCm48Q_twzukKyg3Fm3oaRQig7OuIP-a562kyr0LgMDGl-zJJiqtTPL3q8ktFicpuMZSUbquJvtbfnnLg3MSwihAJ1vTURBk0gHqTj2xq1qSNM9qUWMhAQnkiiMpxEbcY9D4YO0Vi5im0pt9dbpRAAsl2mVd-8LE7w8-BT0dKHiAHHwaidzmfl2rx9qBhcoxwLahj0LRd0TNBWF3u6M0aV58we3g7rqQ0vzBHbxWlH3SkuJ_XyzC8TjzEe6__X4zBPsfis6cmTTFzAcWNfU1XqrxP-qag_D9b1Glw3DQ5plVgw_0G00)

รูปที่ 10

@startuml
 (*) --> if "switchoff" then
        -left->[false] "end"
        else
      --> if "buttonChengHotLaveloff" then
          -->[false] "end"
          else
         --> if "buttonStartoff" then
          -->[false] "end"
          else
          -->"macnstart"
          endif
          endif
          endif

@enduml
@startuml
(*) --> "CHECK_SWITCH = OFF"
   
    if " " then
         -->[TRUE] "END"
         
        
    else
        -->[FALSE] "CHECK_SWITCH_HOT = 0"
                if " " then 
                        -->[TRUE]"END"
                else
                    -->[FALSE]"CHECK_BUTTON_START = OFF" 
                        --> if " " then
                                -->[TRUE] "END"
                            else
                                -->[FALSE]"START"
                                START --> (*)
                                END --> (*)
                            endif
          
                endif
    endif

@enduml
 
![](http://www.plantuml.com/plantuml/img/SoWkIImgAStDuTBGqbJGrRLJK7BsS7NsZWyEzmnnzb2mLV1tSrFYKb1G0665p3G59I0ioKZD0_F10AWhEYGer3LMGSdLpqK98S65maZDAKxbGjRZvkWJ3DA4R66yXty8q58395EW0Cbg1Gn93AUWkGGAK9o0hW_Y7AXhd493GlpzueD378D2e860rrRi8KF8bGhOdKcKat4u7-nY9O8w81u3EHmOxmHL0rr9bDhKl9JCD2GLNBWLG5XS3a0QbFe0)
