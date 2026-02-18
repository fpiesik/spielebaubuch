so sieht code aus
```lua
function _init()
 b=13 --breite
 h=40 --hoehe
 x=10
 y=10
 v=0 --wert
 d=0
 spd=3
 akt=1 --
end

function _draw()
 cls()
 print(v)
 if btn(4) then akt=0 end
 if btn(5) then akt=0 end

 if akt == 1 then v=v+d end

 if v<=0 then d=spd end
 if v>=h then d=-spd end	
	
 rrectfill(x,y+h-v-1,b,v,1,3)
 rrect(x,y,b,h,1,2)
end
```
