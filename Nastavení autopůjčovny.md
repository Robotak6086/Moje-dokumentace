NASTAVENÍ ČÍSELNÍKU PRO AUTOPŮJČOVNU  

Číselníky pro nastavení fungování autopůjčovny jsou seskupeny na Role centre -> v oblasti Akce ->  pod záložku -> Nastaveni  

NASTAVENÍ AUTOPŮJČOVNY (API RENT A CAR SETUP (4027400)

Základné nastavení pro modul Autopůjčovny + nastavení ceny paliv 
Ceny paliv
Uživatel nastavuje ceny paliv, pro dopočet chyběného množství paliva po vrácení vozidla a lze jim nastavovat i časovou platnost dle vývoje na trhu.
Po kliknutí na Ceny palív sa otevře číselník Ceníku PHM. V této tabulce jsou nastavené řádky s jednotlivými typmi produktů pro pohonní hmoty
  

Pro každý zadaný řádek s produktem pro Ceník PHM (napr: Benzín) existuje samostatní tabulka se sazbami PHM. Uživatel může zadávat vždy platní sazby omezené datumy

 

2.1.1.2	Záložka Obecné
 

Obsahuje Pole:

•	Benzín kód (Petrol Code)
•	Nafta kód (Diesel Code)
•	Tolerance vrácení vozidla (Car Return Toleration [h])
o	počet hodin, které nemají vliv na cenu výpůjčky při pozdním vrácení. Vrácení v rámci dne, pak nastavit toto pole na 0.
•	Upozornění před koncem data EK/TK a pojištění (dny) (Warning Interval For Insurance Ending)
o	počet dnů, které zbývají do vypršení pojištění nebo technické kontroly. Dojde k upozornění v případě, že je tento vůz je nabídnut k vypůjčení.
•	Garance – sleva % (Warranty - Discount %)
o	nastavení procentuální slevy, v případě výpůjčky na Garanci.
•	Mechanik – skupina zdrojů (Mechanic Resource Group)
•	Kód důvodu pro fakturaci (Reason Code for Invoice)
o	Určuje kód příčiny pro připojení k položce na fakture.Zobrazuje se ve fakturách a finančních dennících
•	Vozy před vrácením (dny) (Rent Before Return days)
o	Hodnota v poli slouží pro výpočet data v dlaždici „Vozy před vrácením „ na role centre. 
o	Po kliknutí na dlaždice se zobrazí seznam z vozidly,který mají pronájem do (datum) menší nebo rovný jako je : systemový den – hodnota v tomto poli 
•	Vytíženost vozu text (Utilization Vehicle Text)
o	Defaultní hodnota = Ne
o	Pokud je nastavená hodnota  = Ne nebudou se ve vytíženosti vozidel zobrazovat textové hodnoty aktuálního stavu vozidla. Zobrazí se jenom znak svislé čárky ( - ) a textově se budou zobrazovat jenom nevypůjčené vozidla „Nezadáno“.   
 
o	Pokud je nastavená hodnota = Ano budou se ve vytíženosti vozidel zobrazovat textově hodnoty aktuálního stavu vozidla, zvýrazněné barvami. Barvy se nedají uživatelsky měnit. 
 
Text v matici: Nezadáno, Vypůjčeno, K dispozici / Vypůjčeno, K dispozici, Rezervováno, K dispozici / Rezervováno, K dispozici / Vypůjčeno / Rezervováno, Rezervováno / Vypůjčeno, Nedostupné (příznak na kartě vozu autopůjčovny - Vozidlo dočasně nedostupné = ANO)

•	Zahrnout do konsolidované faktury (Include To Consolidate Inv.)
o	Nastavit na hodnotu = Ano, pokud majé být faktury za nájem, součastí konsolidované faktury pro zákazníka
•	Vozy před vrácením (dny) (Rent Before Return days)
o	Hodnota v poli slouží pro výpočet data v dlaždici „Vozy před vrácením „ na role centre. 
o	Po kliknutí na dlaždice se zobrazí seznam z vozidly,který mají pronájem do (datum) menší nebo rovný jako je : systemový den – hodnota v tomto poli 


2.1.1.3	Záložka Číslování 
 
Obsahuje pole:
•	Čísla rezervací (Reservation Nos.)
•	Čísla pronájmů (Rent Nos.)
•	Čísla interních rezervací (Internal Reservation Nos.)
•	Čísla interních pronájmů (Internal Rent Nos.)
•	Čísla faktur autopůjčovny (Rent a Car Invoices Nos.)
•	Čísla dobropisů autopůjčovny (Rent a Car Credit Memo Nos.)
•	Čísla předávacích protokolů (Hand-over Protocols Nos.)
•	Čísla vozů (Car Rent Nos.)
2.1.1.4	 Záložka Dimenze
 
Obsahuje pole:
•	Dimenze zakázky (Order Dimension)
•	Dimenze VIN (VIN Dimension)
2.1.1.5	 Záložka Smlouva
Tato záložka slouži pro doplnení polí (aby byli na jenom míste), kterých hodnota se může tisknout na Smlouvu. Aktuálne obsahuje pole:
 
•	Zahraniční cesta (Travel Abroad)
o	Textové pole 250 znakov
•	Poznámka (Note)
o	Textová poznámka 80 znakov

2.1.1.6	 Záložka Obrázek
 
Do záložky může uživatel vložit kliknutim obrázek pro využití zobrazení obrázku v tiskových výstupech. Napr: protokol o předáni a vrácení.
 

2.1.2	NASTAVENÍ OBECNÉHO ÚČTOVÁNÍ AUTOPŮJČOVNY (RENT A CAR POSTING SETUP (4027419)
Číselník pro nastavení finančního účtování, jednotlivých položek výpůjčky (pronájem, km, poplatky, spoluúčast…)
 
Po kliknutí na Spravovat -> Úpravy / Zobrazit se nám zobrazí karta řádku seznamu, který je označen. 
 

Pole:
2.1.2.1	 Záložka Obecné (General)
•	Obecná obchodní účto skupina (Gen. Bus. Posting Group)
o	Určuje typ položky produktu k propojení transakcí pro tuto položku s odpovídajícím účtem hlavní knihy podle obecného nastavení pro zaúčtování transakcí.
•	Obecná účto skupina zboží (Gen. Prod. Posting Group)
o	Určuje typ položky produktu k propojení transakcí pro tuto položku s odpovídajícím účtem hlavní knihy podle obecného nastavení pro zaúčtování transakcí.
2.1.2.2	 Záložka Autopůjčovna (Car Rental)
•	Pronájem (Rent)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka faktury za pronájem 
•	Sleva (Discount)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka slevy z pronájmu 
•	Účtované kilometry (Billed Kms)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka za projeté km
•	Palivo (Fuel)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka za nedotankované palivo
•	Spoluúčast (Participation)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka případné spoluúčasti z pojistné události
•	Ostatní poplatky (Other Fees)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka poplatků
•	Paušální náhrada škody (Overall Indemnity)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka škody způsobené na vozidle
•	Poplatek za přistavení (Apposition Fee 40) 
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka za přistavení vozidla
•	Poplatek za vyzvednutí (Pickup Fee 45)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka za vyzvednutí vozidla
•	Smluvní pokuta (Penal Clause)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka případná smluvně dohodnutá pokuta
•	Výjezdy (Trips)
o	Uživatel vybere hodnotu finančního účtu, na který účet se má účtovat částka za nadstandartní výjezdy k vozidlu

2.1.3	TARIFNÍ SKUPINY (API TARIF GROUP (4027405))
Ve formuláři Tarifní skupiny nastavuje uživatel tarifní skupiny, ke kterým jsou nadefinovány účto skupiny a DPH na jejichž základě budou účtovány jednotlivé položky na finanční konta. 
Tarifní skupiny také zajišťují základní (nejvyšší) členění vozidel autopůjčovny
 
Pole:
•	Kód (Code)
o	Uživatelsky zadaný kód pro daný řádek 
•	Popis (Description)
o	Uživatelsky popis pro daný řádek
•	DPH obchodní účto skupina (VAT Bus. Posting Group)
o	Určuje specifikaci DPH příslušného řádku pro propojení transakcí provedených pro tento záznam s příslušným finančním účtem dle nastavení účtování DPH.
•	DPH účto skupina zboží (VAT Prod. Posting Group)
o	Určuje specifikaci DPH souvisejícího zboží nebo zdroje pro propojení transakcí provedených pro tento záznam s příslušným finančním účtem dle nastavení účtování DPH.
•	DPH % (VAT %)
o	Needitovatelné pole, dotáhne se podle nastavené DPH účto skupina zboží (VAT Prod. Posting Group)
•	Obecná účto skupina zboží (Gen. Prod. Posting Group)
o	Určuje typ položky produktu k propojení transakcí pro tuto položku s odpovídajícím účtem hlavní knihy podle obecného nastavení pro zaúčtování transakcí.

Pro jednotlivé možné položky služby vztažené k fakturaci za výpůjčku je potřeba nastavit také čísla účtů, na které se budou vytvářet řádky služby prodejní faktury (Nastavení obecného účtování)


2.1.4	TARIFNÍ PODSKUPINY (API TARIFF SUBGROUP (4027404))
Tento formulář slouží k definici tarifních podskupin. Tarifní podskupiny slouží ke slučování podobných typů vozidel autopůjčovny.
 

Pole:
•	Skupina kód (Group Code)
o	Uživatel vybere kód tarifní skupiny
•	Kód (Code)
o	Uživatelský zadaný kód pro daný řádek
•	Popis (Description)
o	Text 50
o	Uživatelský zadaný popis řádku

2.1.5	TARIFNÍ CENÍKY (API TARIFF PRICELIST (4027402))
Karta ceníku pro výběr k danému vozidlu obsahuje hlavičku ceníku pro identifikaci ceníku v časti Obecné a část s řádkami podrobného ceníku v podformuláři Tarifní ceník subformulář	

 
2.1.5.1.1	Záložka obecné
Pro definici ceníku je nutno vyplnit pole Tarifní skupina. Následně bude ceník nabízen jen u vozů, které mají v nastavení stejnou tarifní skupinu. 
Pole:
•	Tarifní skupina (Tariff Group)
o	Pro nastavení Tarifní skupiny musí být nastavená tabulka Tarifní skupina
o	Uživatel vybere kód požadované tarifní skupiny
o	po nastavení tarifní skupiny bude tento ceník nabízen u vozů, které mají nadefinovánu stejnou tarifní podskupinu.
o	Povinné pole
•	Tarifní podskupina (Tariff Subgroup)
o	Uživatel vybere z tabulky Tarifní podskupiny kód 
o	Tabulka filtrovaná na zadanou Tarifní skupinu v poli Tarifní skupina
o	Povinné pole
•	Kód ceníku ((Pricelist Code)
o	Kód na 10 znaků 
o	uživatel zvolí (zapíše) kód ceníku. Tento kód závisí na volbě uživatele, je doporučeno aby kód symbolizoval skupinu, pro niž je určen.
•	Popis (Description)
o	Text 60 znaků
o	pole pro textový popis ceníku. Zvolí Uživatel
o	nepovinné pole
•	DPH
o	tato hodnota je načtena dle přiřazené DPH účto skupiny na Tarifní skupině vložené na kartě konkrétního ceníku.
 
•	Počet disponibilních vozidel (Available Car Count)
o	toto pole indikuje počet vozidel, na nichž je konkrétní ceník navázán
o	kliknutím na číslo v poli se otevře Přehled vozů autopůjčovny pro tento tarifní ceník
•	Sazba – měsíční pronájem (Tariff - Month Rent)
o	hodnota v Kč bez DPH, která definuje defaultní měsíční cenu za vypůjčení vozidla.
o	Po zadání hodnoty se automaticky doplní také hodnota v poli Sazba – měsíční pronájem s DPH
•	Sazba – měsíční pronájem s DPH (Tariff - Month Rent Incl. VAT)
o	hodnota v Kč včetně DPH, která definuje cenu vč. DPH za vypůjčení vozidla.
o	Po změně hodnoty v poli se automaticky propočte také hodnota v poli Sazba – měsíční pronájem
•	Účtování po hodině ((Post By Hour)
o	Defaultní hodnota = Ne
o	po zatržení tohoto pole bude výpůjčka účtována po hodinách podle nastaveni ceny v poli Pronájem od (hodina) a Pronájem do (hodina)
•	Záloha na nájem (Deposit For Rent)
o	zde může vložit uživatel výšku zálohy, která je požadována při vypůjčení vozidla s tímto ceníkem.
•	Zahrnuté kilometry (Included Kms)
o	zde může uživatel nadefinovat zda budou počítány u tohoto ceníku volné kilometry. Jsou dostupné dvě volby
	Bez omezení – v tomto případě jsou volné kilometry ignorovány
	Dle ceníku – v tomto případě budou volné kilometry počítány podle množství a počtu období definované v poli Volné km a Volné km pro. V těchto polích definuje uživatel období na které jsou volné kilometry nastaveny.
•	Volné kilometry (Free Kilometers)
o	Počet volných km, které se počítají na dané období v poli Volné km pro pokud je nastaveno Dle ceníku v poli Zahrnuté kilometry
•	Volné km pro (Free Km for)
o	Období pro km nastavené v poli Volné kilometry
•	Platnost od (Validity From)
o	datum od něhož se bude ceník nabízet. Toto pole musí být vyplněno, pokud chceme aby mohl být ceník užíván.
•	Platnost do (Validity To)
o	nepovinné pole, je jím možno určit datum konce platnosti ceníku.
•	Změněno dne (Changed Date)
o	datum poslední změny ceníku.
•	Změněno ID (Changed By User ID)
o	zde je uvedeno identifikační název pracovníka, který změnu provedl.
•	Centrum odpovědnosti (Responsibility Center)
o	zde může vložit uživatel Centrum odpovědnosti. Dle tohoto centra odpovědnosti se bude ceník zobrazovat pouze pracovníkům majícím právo na toto centrum odpovědnosti.
o	Nepovinné pole
2.1.5.1.2	 Řádky Tarifního ceníku.

 

Tyto řádky slouží k definici cen dle délky doby vypůjčení. Do pole Pronájem od (den) uvede spodní hranici počtu dnů výpůjčky a do pole Pronájem do (den) horní hranice počtu dnů pro něž je tento řádek ceníku platný.
Pole: 
•	Pronájem od [den] (Rent From (Day))
o	Uživatel nastaví spodní hranici počtu dnů výpůjčky
o	Do pole musí nastavit hodnotu tak aby se nekryla s obdobím zadaným na jiném řádku v poli Pronájem do (den)
o	V případě pokryti z jiným řádkem nedovolí systém řádek založit a uživateli se zobrazí hláška
	Existuje jiný řádek tohoto ceníku, který se kryje s obdobím zadaném na právě zadaném řádku!
 
•	Pronájem do [den] (Rent To (Day))
o	Uživatel zadá horní hranice počtu dnů, pro něž je tento řádek ceníku platný.
•	DPH % (VAT %)
o	tato hodnota je načtena dle přiřazené DPH účto skupiny na Tarifní skupině vložené na kartě konkrétního ceníku.
•	Sazba (den) (Tariff (Day)) 
o	v tomto poli definuje uživatel cenu platnou pro jeden den výpůjčky daného řádku ceníku.
•	Sazba s DPH (den) (Tariff Incl. VAT (Day))
o	V poli se dopočte hodnota ceny s DPH podle zadané sazby v poli Sazba (den)
o	Pokud Uživatel změní hodnotu v tomto poli přepočte se také hodnota v poli Sazba (den)
•	Pronájem od [hodina] (Rent From (Hour))
o	Uživatel doplní sazbu, která bude použitá v případě hodinových nájmu. Lze zadat jenom když je hodnota v poli Účtování po hodině = Ano
•	Pronájem do [hodina] (Rent To (Hour))
o	Uživatel zadá horní hranice počtu hodin, pro něž je tento řádek ceníku platný
o	Lze zadat jenom když je hodnota v poli Účtování po hodině = Ano
•	Volné kilometry (Free kilometers)
o	Defaultne se dotáhne hodnota z pole Volné kilometry ze záložky Obecné, pokud je v poli zahrnuté km hodnota dle ceníku
o	Uživatel počet volných kilometrů, které nebudou počítány dle zvoleného období, může propsat
o	Pokud Uživatel změní hodnotu v poli Zahrnuté km na Bez omezení hodnoty v tomto poli se pro všechny řádky vynulují
•	Pevná částka (Fixed Amount)
o	zde může uživatel nadefinovat sazbu, která bude vždy počítána bez závislosti na ostatních hodnotách.
•	Pevná částka s DPH (Fixed Amount Incl. VAT)
o	V poli se dopočte hodnota Pevné částky s DPH podle zadané sazby v poli Pevná částka
o	Pokud Uživatel změní hodnotu v tomto poli přepočte se také hodnota v poli Pevná částka
•	Sazba za km nad limit (Price Per Km Over Limit) 
o	 uživatel může vložit sazbu za ujeté km nad definovaný limit, podle které se budou dofakturovávat nadlimitní km
•	Sazba za km nad limit s DPH (Price Per Km Over Limit Incl. VAT)
o	V poli se dopočte hodnota Sazby za km nad limit s DPH podle zadané sazby v poli Sazba za km nad limit 
o	Pokud Uživatel změní hodnotu v tomto poli přepočte se také hodnota v poli Sazba za km nad limit 
•	Sazba [výjezd] (Tariff (Trip))
o	 v tomto poli může uživatel definovat sazbu za přistavení vozidla mimo provozovnu, podle které se budou dofakturovávat poplatky za výjezdy podle pole Počet výjezdů * Sazba [výjezd]
•	Sazba s DPH [výjezd] (Tariff Incl. VAT (Trip)) 
o	 V poli se dopočte hodnota Sazby s DPH [výjezd] podle zadané sazby v poli Sazba [výjezd]
o	Pokud Uživatel změní hodnotu v tomto poli přepočte se také hodnota v poli Sazba [výjezd]

2.1.6	PARKOVIŠTE (API PARKING PLACE (4027401))
V této části jsou nastaveny informace o domovském parkovišti / nákladovém středisku vozidla autopůjčovny. Tuto hodnotu lze vybrat na kartu vozu v záložce Autopůjčovna do pole Parkoviště
 
Pole:
•	Číslo (No.) 
o	Kód pro daný řádek, zadává Uživatel, může být také text
o	10 znaků
•	Umístění (Place)
o	Textová informace, kde je vozidlo defaultne umístěno
o	Text 30 
•	Popis (Description) 
o	Uživatelsky popis k umístnění vozidla. V případě doplňující informace
o	Text 30
•	Nákladové středisko (Cost Centre) 
o	Pokud je vozidlo přirazené v rámci autopůjčovně pod samostatné středisko může pro informaci zadat uživatel název střediska 
o	10 znaků

