This irule is based on the TCL server irule https://wiki.tcl-lang.org/page/Tcl+DNS+server .

As it does not support edns use the dig command with +noedns

I have replaced the ::db variable with static::db to make the irule CMP compatible and I have replaced "puts" with log local0.

I also have added a bypass if the domain is not in the irule.
