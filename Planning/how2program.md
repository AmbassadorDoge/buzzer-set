i suck at programming!

im thinking of having the controller send out syncs every reset that allow all buzzers to know their "synced" time through micros() or millis()-havnet decided yet

all buzzers will send periodic timestamps at staggered times to avoid interferance

when buzzers are pressed, they send the elapsed time since last reset in micros, and all are compared for which is lower

when the controller wants to indicate incorrect or correct, it can do that normally(hopefully)