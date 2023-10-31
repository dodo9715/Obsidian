Dostava paketa:

Paketi
	-tipski paketi s predefiniranim dimenzijama (A,B,C,D,E) i slobodnim (X)
	-svaki pipski paket ima predefiniranu max težinu dok je kod paketa X određena argumentom --mt
Usluge dostave
	-standardna S
	-hitna H
	-plaćanje pouzećem P
	-povratak paketa R
Radno vrijeme
	--pr za početak rada
	--kr za kraj rad
Ureda za prijem paketa evidentira za svaki paket vrijeme prijema paketa, pošiljatelja, primatelja, vrstu paketa (kod X i ostale podatke), vrstu usluge (iznos kod plaćanja pouzećem). Podaci za pakete na prijemu se kronološki evidentiraju. Za svaki primljeni paket potrebno je naplatiti iznos dostave (svaki tipski paket ima svoju cijenu dostave, a za paket X slobodnih dimenzija formula se nalazi u tablici 1), osim kod paketa s uslugom plaćanja pouzećem. Njega naplaćuje vozilo koje odrađuje isporuku.

Ured za dostavu paketa raspolaže s određenim voznim parkom (od bicikla, skutera do automobila). Svako vozilo ima kapacitet prijevoza (težina u kg, prostor u m3).

Pakete koje treba dostaviti ukrcavaju se u slobodno vozilo tako da se ne prekorači njegova dozvoljena težina i prostor. Vozila se odabiru prema oznaci redoslijeda, od manjeg broja prema većem. Prvo se ukrcavaju paketi koji imaju hitnu dostavu. Nakon što se popuni kapacitet vozila ili nakon punog sata vozilo koje ima barem jedan ukrcani paket hitne dostave ili je popunjeno minimalno 50% kapaciteta (težine ili prostora) kreće prema odredištima paketa.

Paketi se isporučuju prema redoslijedu kako su ukrcani u vozilo. Za svaki paket potrebno vrijeme za isporuku određeno je argumentom/opcijom (--vi u minutama) prilikom izvršavanja programa. Kod isporuke paketa primatelju potrebno je evidentirati vrijeme preuzimanja paketa. Ako je paket s uslugom plaćanja pouzećem potrebno je kod vozila ažurirati prikupljeni novac s iznosom pouzeća.