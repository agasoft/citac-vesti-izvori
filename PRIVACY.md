# Politika privatnosti / Privacy policy

**Aplikacija: Čitač vesti (News Reader), za Windows i Android**

Poslednja izmena: 26. novembar 2026.

## Srpski

Čitač vesti ne prikuplja, ne čuva i ne šalje autoru aplikacije nikakve lične podatke. Aplikacija nema nalog, analitiku, praćenje grešaka ni oglase. Jedini server aplikacije služi za sinhronizaciju između vaših uređaja, samo ako je sami uključite, i čuva samo šifrovane podatke koje ne može da pročita.

**Šta ostaje na vašem uređaju**

- Podešavanja, lista izvora, pročitane i sačuvane vesti čuvaju se u lokalnoj bazi na vašem računaru ili telefonu. Autor aplikacije nema pristup tim podacima.
- Windows: ključ za AI rezime, ako ga unesete, čuva se u Windows Credential Manager-u (sistemskom skladištu lozinki) i koristi se samo za servis koji ste izabrali.

**Kome se aplikacija obraća preko interneta**

- **Sajtovima medija** koje pratite: preuzima njihove RSS feedove i tekstove vesti koje otvorite, kao što bi to uradio pregledač. Aplikacija se predstavlja kao „CitacVesti“. Kada dodate izvor po adresi, aplikacija posećuje taj sajt da bi pronašla njegov RSS feed.
- **GitHub** (raw.githubusercontent.com): preuzima javnu listu izvora da bi ispravke feedova stizale bez nove verzije aplikacije.
- **Open-Meteo** (open-meteo.com), samo na Windowsu i samo ako ste izabrali grad: šalje koordinate grada da bi dobila trenutnu temperaturu, i naziv grada dok ga tražite u podešavanjima.
- **Servis za AI rezime**, samo na Windowsu i samo ako ga sami podesite i zatražite rezime: Google Gemini, Groq, OpenAI, DeepSeek ili Anthropic Claude, sa vašim ključem. Šalju se samo naslovi i prve rečenice do 30 vesti iz trenutnog prikaza, nikakvi podaci o vama. Na ovaj zahtev se primenjuju uslovi izabranog servisa; aplikacija za svaki servis navodi kako on koristi podatke. Na primer, Google na besplatnom nivou može da koristi poslate tekstove za poboljšanje svojih proizvoda, a DeepSeek obrađuje podatke na serverima u Kini.
- **Google obrazac (Google Forms)**, samo kada sami predložite novi izvor ili prijavite neispravan: šalje se ono što ste upisali (vrsta prijave, naziv izvora, adresa, zemlja i vaša napomena) i verzija aplikacije. Ne šalju se nikakvi podaci o vama, a obrazac ne prikuplja imejl adrese.

**Sinhronizacija između uređaja (samo ako je sami uključite)**

Ako povežete uređaje (na primer računar i telefon), pročitane i sačuvane vesti se prenose preko servera za sinhronizaciju na Cloudflareu (citac-vesti-sync.citac-vesti-sync.workers.dev). Nalog nije potreban.

- Podaci se šifruju na vašem uređaju pre slanja (AES-256-GCM), ključem koji imaju samo vaši povezani uređaji. Ni autor aplikacije ni Cloudflare ne mogu da pročitaju koje vesti čitate ili čuvate, ni sa kojih sajtova.
- Uređaji se povezuju kodom od šest cifara i kontrolnim brojem koji poredite na oba uređaja; ključ za šifrovanje nikad ne prolazi kroz server nešifrovan.
- Na serveru se čuvaju samo šifrovani zapisi, njihova veličina, vreme promene i rok brisanja. Iz roka brisanja može se približno videti oko kog dana su vesti pročitane, ali ne i koje.
- Zapisi o pročitanim vestima brišu se posle 10 dana, uklonjene sačuvane vesti posle 30 dana, a svi podaci grupe ako se nijedan uređaj ne javi 180 dana.
- Sve podatke možete odmah obrisati dugmetom „Obriši sve podatke sa servera“ u aplikaciji.
- IP adrese se ne upisuju na server; Cloudflare ih vidi kao i za svaki sajt.

**Android: osvežavanje u pozadini i obaveštenja**

Ako ih uključite, aplikacija u pozadini proverava vaše izvore i obaveštava vas o novim vestima. Obaveštenja se prave na samom telefonu, bez ikakvog spoljnog servisa za obaveštenja.

Linkovi iz vesti i dugme „Otvori original“ otvaraju se u vašem podrazumevanom pregledaču.

**Kontakt:** agasoft@gmail.com

## English

Čitač vesti (News Reader) does not collect, store or send any personal data to the app's author. The app has no account, no analytics, no crash reporting and no ads. Its only server is for syncing between your own devices, only if you turn it on, and it stores only encrypted data that it cannot read.

**What stays on your device**

- Settings, the source list, and read and saved articles are stored in a local database on your computer or phone. The author has no access to this data.
- Windows: the AI summary key, if you enter one, is stored in Windows Credential Manager and is used only for the service you chose.

**What the app connects to**

- **The news sites you follow:** it downloads their RSS feeds and the articles you open, as a browser would. The app identifies itself as "CitacVesti". When you add a source by its address, the app visits that site to find its RSS feed.
- **GitHub** (raw.githubusercontent.com): it downloads the public source list, so feed fixes arrive without a new app version.
- **Open-Meteo** (open-meteo.com), on Windows only, and only if you chose a city: it sends the city's coordinates to get the current temperature, and the city name while you search for it in settings.
- **The AI summary service**, on Windows only, and only if you set it up yourself and ask for a summary: Google Gemini, Groq, OpenAI, DeepSeek or Anthropic Claude, with your own key. Only the headlines and first sentences of up to 30 articles from the current view are sent, never data about you. That request is governed by the chosen service's terms; the app explains how each service uses data. For example, Google may use text sent on its free tier to improve its products, and DeepSeek processes data on servers in China.
- **Google Forms**, only when you suggest a new source or report a broken one yourself: what you typed (type of report, source name, address, country and your note) and the app version are sent. No data about you is sent, and the form does not collect email addresses.

**Sync between devices (only if you turn it on)**

If you link devices (for example a computer and a phone), read and saved articles are shared through a sync server on Cloudflare (citac-vesti-sync.citac-vesti-sync.workers.dev). No account is needed.

- Data is encrypted on your device before it is sent (AES-256-GCM), with a key that only your linked devices have. Neither the app's author nor Cloudflare can read which articles you read or save, or from which sites.
- Devices are linked with a six-digit code and a check number that you compare on both devices; the encryption key never passes through the server unencrypted.
- The server stores only encrypted records, their size, the time of change and the deletion date. The deletion date can roughly show around which day articles were read, but not which ones.
- Records of read articles are deleted after 10 days, removed saved articles after 30 days, and all of a group's data if no device checks in for 180 days.
- You can delete all data at once with the "Delete all data from the server" button in the app.
- IP addresses are not stored on the server; Cloudflare sees them as it does for any website.

**Android: background refresh and notifications**

If you turn them on, the app checks your sources in the background and notifies you about new articles. Notifications are created on your phone; no outside notification service is used.

Links in articles and the "Open original" button open in your default browser.

**Contact:** agasoft@gmail.com
