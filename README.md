# amplificatore-audio-8-ohm
Il circuito descritto è un amplificatore audio in classe A per altoparlanti da 8 ohm di impedenza.
L'amplificazione in tensione avviene tramite un amplificatore operazionale (uA741), e quella in corrente invece mediante un buffer costituito dal BJT (bd911).
Mediante il trimmer (R4) è possibile regolare l'amplificazione dell'operazionale. Il circuito integrato che ho scelto (uA741) lavora con una tensione duale, data l'impossibilità di generarla sul circuito ho scelto una soluzione più semplice.Ho dato al op-amp un riferimento di massa_virtuale (vcc/2) mediante il pin non invertente (+), e ho posto il GND del Vin allo stesso potenziale del riferimento che sappiamo essere a VCC/2 = 6V.Con questo sistema il segnale audio in uscita dall'op amp si sovrappone al riferimento di massa di massa virtuale (6V), invece che alla massa vera propria (0V); così all'uscita del circuito integrato avremo un segnale completo sinosuidale senza le semionde negative tosate.
Tengo a precisare che questo è ovviamente solo un prototipo, realizzato con calcoli semplici e veloci.

