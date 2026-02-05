# ultragiga
STP Spanning Tree Protocol
Mire való az STP?

Az STP (Spanning Tree Protocol) egy hálózati protokoll, amelynek célja, hogy megakadályozza a hurkok loopok kialakulását kapcsolt switch-elt hálózatokban. A hurkok adatforgalmi problémákat okozhatnak, például hálózati túlterhelést vagy adatvesztést. Az STP biztosítja, hogy a hálózat hurkok nélkül, stabilan működjön.

1. Beállításának menete

Az STP alapértelmezetten engedélyezve van a legtöbb menedzselhető switchen. A beállítás során először kiválasztásra kerül a root bridge, amely a hálózat központi eleme lesz. Ez prioritás és MAC-cím alapján történik.
Ezután a switchek meghatározzák a legjobb útvonalakat a root bridge felé, és azokat a portokat, amelyek hurkot okoznának, automatikusan blokkolják. A beállítás után a hálózat működését ellenőrizni kell.

2. Előnyei

Az STP legnagyobb előnye, hogy megelőzi a hálózati hurkok kialakulását, ezzel biztosítva a hálózat stabilitását. Automatikusan működik, nem igényel folyamatos emberi beavatkozást. Növeli a hálózat megbízhatóságát, és megakadályozza a broadcast storm jelenséget.

3. Hátrányai

Hátránya, hogy az STP lassan reagál a hálózati változásokra, például egy link kiesésére. Emellett a blokkolt portok miatt nem használja ki teljes mértékben a rendelkezésre álló sávszélességet. Nagyobb hálózatok esetén a konfigurálása és felügyelete bonyolult lehet.

4. Gyakorlati példák

Az STP-t leggyakrabban vállalati hálózatokban használják, ahol több switch van összekötve egymással. Például egy iskolai vagy irodai hálózatban, ahol a redundáns kapcsolatok fontosak a folyamatos működéshez. Ha egy kábel megszakad, az STP új útvonalat választ, így a hálózat továbbra is működőképes marad.
