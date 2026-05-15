# Robottinen hiustenleikkaus

Kielet: [English](README.md) | [中文](README.zh.md) | Suomi | [Deutsch](README.de.md) | [Français](README.fr.md)

Tama arkisto toimii ensisijaisesti robottista hiustenleikkausta kasittelevana tietosanakirjamaisena yleiskatsauksena. Se kokoaa yhteen taustaa, historiaa, turvallisuutta, haasteita, tutkimussuuntia ja viitteita. Arkistoon kootut asiaankuuluvat julkaisut on listattu sivun lopussa.

## Yleiskuva

Robottinen hiustenleikkaus tarkoittaa robottijarjestelmien kayttoa hiustenleikkaustoimintojen avustamiseen tai kokonaan suorittamiseen. Ala voi kattaa leikkaamisen, trimmaamisen, parranajon, hiusten muotoilun ja muita vastaavia hoitotehtavia. Naiden tehtavien toteuttamiseen suunniteltuja robottialustoja kutsutaan tavallisesti hiustenleikkausroboteiksi.

Ala sijoittuu robotiikan, tietokonenakemisen, liikesuunnittelun, robottimanipulaation, ihmisen ja robotin vuorovaikutuksen, viestinnan, tietokonegrafiikan, virtuaalitodellisuuden, tekoalyn ja haptiikan risteyskohtaan.

Toisin kuin tavalliset sahkoiset hiustenleikkuukoneet tai kasin kaytettavat hiustyokalut, robottiset hiustenleikkausjarjestelmat vaativat havainnointi-, suunnittelu- ja ohjauskykyja, joiden avulla robotti voi asemoida leikkaus- tai hoitotyokalun suhteessa ihmisen paahan ja hiuksiin. Tehtava on teknisesti vaikea, koska hiukset ovat muodonmuutoksille alttiita, vaihtelevat suuresti yksiloiden valilla ja niita kasitellaan lahella herkki anatomisia alueita, kuten korvia, silmia, hiuspohjaa ja kasvoja.

Jarjestelmat vaihtelevat teleoperoinnista autonomisempiin konsepteihin. Vuonna 2025 laajasti kaytossa olevaa taysin kaupallista hiustenleikkausrobottia ei ollut, mutta tutkimusprototyypit ja katsausartikkelit viittaavat mahdolliseen kaupallistumispolkuun.

## Historia

### Varhaiset automaattiset hiustenleikkauslaitteet

Ajatuksia automaattisesta hiustenleikkauksesta esitettiin jo ennen nykyaikaisia robottijarjestelmia. [Jean Gronierin](#ref-gronier-1966) vuonna 1966 saama yhdysvaltalainen patentti kuvasi automaattista hiustenleikkauskonetta, joka tuotti ennalta maaritetyn kampauksen ohjelmoidun ohjauksen avulla. Sita on kuitenkin tarkoituksenmukaisempaa pitaa esirobottisena automaationa kuin modernina robottisena hiustenleikkausjarjestelmana, koska se perustui mekaaniseen rakenteeseen ja ennalta maaritettyihin ohjelmiin eika reaaliaikaiseen havainnointiin tai adaptiiviseen palautteeseen.

Myohemmat patentit esittivat integroidumpia jarjestelmia, joissa yhdistyivat havainnointi, robottimekanismit ja kayttajaliittymat. Tama osoittaa siirtymaa kohti selkeammin robotillisia toteutuksia, mukaan lukien myohempi [Mubarak Aldabbahin](#ref-aldabbah-2023) patentti.

### Kameralla avustetut itseleikkausjarjestelmat

Toinen lahestymistapa keskittyi siihen, miten ihmisia voitaisiin auttaa leikkaamaan omat hiuksensa sen sijaan, etta robotti suorittaisi leikkauksen itsenaisesti. Vuonna 2014 [Futami, Terada ja Tsukamoto](#ref-futami-2014) esittivat liikkuvalla kameralla varustetun robottijarjestelman, jonka avulla kayttaja pystyi tarkastelemaan paataan eri kuvakulmista itseleikkauksen aikana.

### Robottiset hiustenleikkausprototyypit

2020-luvulla useat julkiset demonstraatiot ja tee-se-itse-prototyypit toivat robottisen hiustenleikkauksen laajemman huomion kohteeksi. Nissa projekteissa yhdistyivat mekaaninen toimilaite, anturointi ja kayttajan valvonta, mutta ne olivat yleensa kokeellisia esittelyja eivatka validoituja tai kaupallisesti kaytossa olevia jarjestelmia; sama ero tehdään myos [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) -teoksessa.

### Lahialueen hiustenhoito- ja muotoilurobotit

Useat akateemiset jarjestelmat ovat tarkastelleet hiustenleikkauksen lahitehtavia, kuten shampoopesua, hiuspohjan hierontaa, harjausta, kampausta, takutuksen poistoa ja otsahiusten muotoilua. Namat jarjestelmat eivat valttamatta leikkaa hiuksia, mutta ne kasittelevat monia samoja teknisia kysymyksia, kuten muodonmuutoksille alttiiden hiusten havainnointia, kontaktirikkaita manipulointitehtavia, polkusuunnittelua, kayttajamukavuutta ja turvallisuutta paan lahella ([Ando ym., 2013](#ref-ando-2013); [Hughes ym., 2021](#ref-hughes-2021); [Dennler ym., 2021](#ref-dennler-2021); [Yoo ym., 2024](#ref-yoo-2024); [Kim ym., 2025](#ref-kim-2025)).

Esimerkkeja ovat hiustenpesu- ja paanhoitorobotit, palautteeseen perustuvat takutuksenpoistojarjestelmat, robottikampausalustat, MOE-Hairin kaltaiset pehmeat hiustenkasittelyjarjestelmat seka otsahiusten muotoilurobotit, jotka perustuvat hiussuortuvien juurikeskeiseen saatoon.

### Akateeminen kehitys

2020-luvulla robottinen hiustenleikkaus alkoi hahmottua omaksi tutkimusaiheekseen palvelurobotiikassa ja henkilokohtaisen hoivan automaatiossa. Varhaiset monografiat ja katsausartikkelit kuvasivat hiustenleikkausta monitieteisena insinooriongelmana, johon sisaltyvat havainnointi, muodonmuutoksille alttiiden kohteiden mallinnus, liikesuunnittelu, ohjaus, teleoperointi, ihmisen ja robotin vuorovaikutus seka turvallisuus. Samat tyot korostivat paan lahella toimimisen vaikeutta, mukaan lukien hiusgeometrian epavarmuus, kayttajien valinen vaihtelu ja tarve tiiviisti integroiduille havainnointi-suunnittelu-ohjausputkille, ja ne esittivat laajempia kasitteellisia kehyksia, joissa robottista hiustenleikkausta tarkastellaan esimerkiksi CNC-tyyppisena prosessina tai liikkuvan robotin peittotehtavana, johon liittyy turvarajoitteita kriittisten alueiden ymparilla ([Li, 2025](publications/2025/LiHaircutting%20Robots.pdf); [Shuai Li, 2025](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf); [Khan ja Li, 2026a](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf); [Khan ja Li, 2026b](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)).

Uudempi tutkimus on lisaksi yhdistanut robottisen hiustenleikkauksen visio-kieli-toiminta-arkkitehtuureihin ja kayttanyt sita konkreettisena tapausesimerkkina korkeamman tason jarjestelmaalykkyyden, arvioinnin ja kayttoonoton tarkasteluun ([2026 position paper](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)).

### Tekoalyn tuottamat robottihiustenleikkausvideot

Vuoden 2025 lopulta alkaen generatiiviset AI-videotyokalut lisasivat kuvitteellisten robottihiustenleikkausvideoiden maarää verkossa. Videoissa esiintyi humanoidikampaajia, monivarsisia tyopisteita ja kypärämäisiä automaattisia hiustenleikkauslaitteita. Vaikka sisalto oli fiktiivista, se lisasi julkista tietoisuutta ja heijasti kasvavaa kiinnostusta automatisoitua henkilokohtaista hoivaa kohtaan.

## Turvallisuus

Turvallisuus on robottisessa hiustenleikkauksessa keskeinen kysymys, koska robotti toimii ihmisen paan lahella kayttaen tyokaluja, kuten leikkureita, saksia, partakoneita, kuivauslaitteita tai lampenevia muotoilutyokaluja. Keskeisia vaaratekijoita ovat havainnointivirheet, paan odottamaton liike, liian suuri kontaktivoima, tyokalun ylikuumeneminen, leikkaustyokalun virheellinen kohdistus, kalibrointivirheet, viive teleoperoinnissa seka ohjelmisto- tai ohjausviat.

Ehdotettuja turvallisuustoimenpiteita ovat tyotilan rajaukset, nopeus- ja kiihtyvyysrajoitteet, voima- tai painerajat, joustavat mekanismit, pehmeat suojukset tai paate-efektorit, hatasammaytys, laheisyysvalvonta, redundantti anturointi seka toiminnan automaattinen keskeyttaminen vaaratilanteissa.

Robottiselle hiustenleikkaukselle ei ole olemassa omaa kansainvalista turvallisuusstandardia. Useat olemassa olevat standardit ovat kuitenkin merkityksellisia riskianalyysin ja jarjestelmasuunnittelun kannalta, erityisesti [ISO 13482](#ref-iso-13482), [ISO/TS 15066](#ref-iso-ts-15066), [ISO 10218-1](#ref-iso-10218-1) ja [ISO 14971](#ref-iso-14971). Hiustenleikkaukseen liittyvia vaaraluokkia, lieventamisstrategioita ja naiden standardien merkitysta tarkemmalle riskianalyysille kasitellaan [Shuai Li (2025)](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf) -julkaisussa seka [vuoden 2025 turvallisuuskatsauksessa](publications/2025/Safety_in_Robotic_Haircutting.pdf).

## Haasteet ja tutkimussuunnat

Keskeisiin haasteisiin kuuluvat hiusten ja hiuspohjan luotettava havainnointi, erilaisten hiustyyppien mallintaminen, kayttajan liikkeen kompensointi, turvallisten tyokaluratojen suunnittelu, sopivan etaisyyden ja kontaktivoiman yllapitaminen seka toimiminen herkkien alueiden, kuten korvien, silmien, kasvojen ja hiuspohjan lahella.

Hiuksia on erityisen vaikea kasitella, koska ne ovat muodonmuutoksille alttiita, suortuvapohjaisia ja hyvin vaihtelevia pituuden, tiheyden, kiharuuden, jaakkyyden ja kosteuden suhteen. Vaikka geometrinen tarkkuus olisi korkea, esteettinen arviointi on edelleen vaikeaa, koska hiustenleikkauksen laatu riippuu myos tyylitoiveista, symmetriasta, mukavuudesta ja kayttajan odotuksista.

Muita haasteita ovat pitkaaikainen toiminta, kustannusten kohtuullisuus, sertifiointi, vastuuasiat, kayttajien hyvaksynta, yksityisyys ja datan kasittely. Kameraan tai kolmiulotteiseen skannaukseen perustuvat jarjestelmat voivat kerata kasvo-, hiuspohja- tai kampausdataa, mika aiheuttaa yleisten turvallisuuskysymysten lisaksi yksityisyyshaasteita.

Namat haasteet osoittavat useita lupaavia tutkimussuuntia robottisessa hiustenleikkauksessa:

- Autonominen hiustenleikkaus
- Teleoperointiin perustuva hiustenleikkaus etavalvotulle asiantuntijaohjaukselle
- Jaetun autonomian jarjestelmat, joissa yhdistyvat ihmisen valvonta ja robotin suoritus
- Hiustenleikkauksen suunnittelu tavoitekampausten, geometristen maaritysten tai kayttajaohjeiden perusteella
- Hiusten, hiuspohjan ja paan asennon reaaliaikainen havainnointi leikkauksen aikana
- Kayttajan liikkeen ja muiden hairioiden kompensointi toiminnan aikana
- Turvallisuustietoinen ohjaus herkilla anatomisilla alueilla toimimiseen
- Arviointiprotokollat, benchmark-menetelmat ja sertifiointiin suuntautunut jarjestelmasuunnittelu
- Kayttoonottoon suuntautunut jarjestelmaintegraatio luotettavaa tosielaman kayttoa varten

## Viitteet

- <a id="ref-gronier-1966"></a>Jean Gronier. *Automatic hair-cutting machine having programmed control means for cutting hair in a predetermined style*. US Patent 3241562A, 1966.
- <a id="ref-aldabbah-2023"></a>Mubarak Aldabbah. *Automatic hair cutter robot*. WO Patent 2023080812A1, 2023.
- <a id="ref-futami-2014"></a>Kyosuke Futami, Tsutomu Terada, and Masahiko Tsukamoto. *A System for Supporting Self-Haircuts Using Camera Equipped Robot*. MoMM, 2014.
- <a id="ref-ando-2013"></a>Takeshi Ando et al. *Biosignal-based relaxation evaluation of head-care robot*. EMBC, 2013.
- <a id="ref-hughes-2021"></a>Josie Hughes et al. *Detangling hair using feedback-driven robotic brushing*. RoboSoft, 2021.
- <a id="ref-dennler-2021"></a>Nathaniel Dennler, Eura Shin, Maja Mataric, and Stefanos Nikolaidis. *Design and Evaluation of a Hair Combing System Using a General-Purpose Robotic Arm*. IROS, 2021.
- <a id="ref-yoo-2024"></a>Uksang Yoo et al. *MOE-Hair: Toward Soft and Compliant Contact-rich Hair Manipulation and Care*. HRI Companion, 2024.
- <a id="ref-kim-2025"></a>Soonhyo Kim et al. *Front Hair Styling Robot System Using Path Planning for Root-Centric Strand Adjustment*. SII, 2025.
- <a id="ref-iso-13482"></a>ISO 13482. *Robots and robotic devices - Safety requirements for personal care robots*.
- <a id="ref-iso-ts-15066"></a>ISO/TS 15066. *Robots and robotic devices - Collaborative robots*.
- <a id="ref-iso-10218-1"></a>ISO 10218-1. *Robotics - Safety requirements for industrial robots - Part 1: Robots*.
- <a id="ref-iso-14971"></a>ISO 14971. *Medical devices - Application of risk management to medical devices*.

## Tiimin julkaisut

Seuraavat julkaisut on mainittu ylla asiaankuuluvissa kohdissa ja koottu tahan arkistoon.

### 2025

- [Haircutting Robots](publications/2025/LiHaircutting%20Robots.pdf)
- [Haircutting Robots from Theory to Practice](publications/2025/Haircutting_Robots_from__Theory_to_Practice.pdf)
- [Safety in Robotic Haircutting](publications/2025/Safety_in_Robotic_Haircutting.pdf)

### 2026

- [CNC-Inspired Robotic Hair Cutting: A Comprehensive Survey on Precision Personal Care Automation](publications/2026/CNC_Inspired_Robotic_Hair_Cutting_A_Comprehensive_Survey_on_Precision_Personal_Care_Automation.pdf)
- [Robotic Haircutting Systems: A Survey of Methods, Challenges and Hair Modeling Insights](publications/2026/Robotic_Haircutting_Systems_A_Survey_of_Methods_Challenges_and_Hair_Modeling_Insights.pdf)
- [Vision-Language-Action Modules for Intelligent Haircutting Robots: A Position Paper on Architectures, Evaluation and Future Direction](publications/2026/Vision_Language_Action_Modules_for_Intelligent_Haircutting_Robots__A_Position_Paper_on_Architectures_Evaluation_and_Future_Direction.pdf)
