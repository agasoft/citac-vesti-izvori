# Izvori za Čitač vesti

Lista RSS izvora koju koristi Čitač vesti, pristupačan čitač vesti za slepe i slabovide korisnike iz Srbije, Hrvatske, Bosne i Hercegovine i Crne Gore.

Aplikacija pri pokretanju preuzima [`sources.json`](sources.json) iz ovog repozitorijuma. Kada se ovde ispravi pokvaren feed ili doda novi medij, svi korisnici dobijaju izmenu bez nove verzije aplikacije.

## Kako se menja lista

1. Izmenite, dodajte ili uklonite izvor (jedan izvor po redu).
2. **Povećajte `version`.** Format je `GGGGMMDDNN`, na primer `2026110401`, pa `2026110402` za drugu izmenu istog dana. Aplikacija preuzima listu samo ako je njena verzija veća od one koju već ima.
3. Proverite da feed radi i da se iz članka izvlači ceo tekst.

Aplikacija odbacuje celu listu ako nešto nije u redu: nepoznata zemlja, ponovljen `id`, adresa koja nije `http` ili `https`, ili lista sa manje od 10 izvora. Tada ostaje na prethodnoj ispravnoj listi.

## Pravila

- `id` se nikad ne menja kad je izvor jednom objavljen, jer korisnička podešavanja pamte izvore po `id`-u. Kad se promeni adresa feeda, menja se samo `url`.
- Ne dodaju se izvori čiji su članci dostupni samo uz pretplatu.

## Predlozi

Ako znate medij iz regiona koji ima RSS feed, otvorite issue sa nazivom medija i adresom feeda.
