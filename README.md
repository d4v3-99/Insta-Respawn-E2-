# Insta-Respawn-E2-

if(first()) {
    runOnDeath(1)
    O = owner()
}

if(deathClk()) {
    if(!O:isAlive()) {
        timer("spawn", 1)
    }
}

if(clk("spawn")) {
    stoptimer("spawn")
    O:plySpawn()
}
entity():setMaterial("models/wireframe")
entity():setColor( vec( 0,255,0) )
"        __ __     _____
  ____/ / // /_   _|__  /
 / __  / // /| | / //_ < 
/ /_/ /__  __/ |/ /__/ / 
\__,_/  /_/  |___/____/  
                        " 
"
hint("by d4v3",7)
