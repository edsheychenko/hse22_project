# hse22_project

Ссылка на колаб: https://colab.research.google.com/drive/1VyeeO2h6eESkAdjlt2Lr9xXiFKn470X5#scrollTo=pQn197KlgYKc

* `data` - геномы 5 выбранных организмов
* `predictions` - предсказания участков Z-DNA для 5 выбранных геномов. Формат файлов: 1 столбец - начало участка, 2 - конец, 3 - zh-score; столбцы разделяются табуляцией  
* `alignments` - все белковые выравнивания для выбранных кластеров  


## 1. Таблица аннотированных генов
|Название организма             |Кол-во хромосом|Длина генома|Кол-во генов |Процент генов в геноме |Кол-во участков Z-ДНК|Кол-во участков Z-ДНК с zh-score > 500 |Общая длина участков Z-ДНК с zh-score > 500  |
|:-----------------------------:|:-------------:|:----------:|:-----------:|:---------------------:|:---------------------:|:---------------------:|:---------------------------:|
|Candidatus Viadribacter manganicus       |1              |3732719     |3848         |74.78                  |3732719                |94607                    |923130                        |
|Candidatus Puniceispirillum marinum IMCC1322|1              |2753527     |2599         |74.88                  |2753527               |14488                   |140582                        |
|Candidatus Phycorickettsia trachydisci |1              |1472411     |1265        |70.56                  |1472411                |560                   |5382                        |
|Candidatus Pelagibacter ubique HTCC1062      |1              |1308759     |1380        |74.58                  |1308759                |119                   |1196                        |
|Candidatus Nucleicultrix amoebiphila FS5|1              |1838212     |1806         |71.17                  |1838212                |3073                   |29734      

## 2. Распределение участков с Z-ДНК

<img width="605" alt="Снимок экрана 2022-06-13 в 20 09 26" src="https://user-images.githubusercontent.com/93148512/173407760-d0935d89-f96b-4a6a-8389-e2c6131274d8.png">

## 3. Гистограмма значений zh-score

<img width="381" alt="Снимок экрана 2022-06-13 в 20 11 40" src="https://user-images.githubusercontent.com/93148512/173408203-a44b5536-1ad5-428b-aedb-c2e10217d158.png">  | <img width="393" alt="Снимок экрана 2022-06-13 в 20 11 53" src="https://user-images.githubusercontent.com/93148512/173408257-9dbf1f5d-f8da-45bb-9374-e7eae1d4a311.png"> 
<img width="399" alt="Снимок экрана 2022-06-13 в 20 11 11" src="https://user-images.githubusercontent.com/93148512/173408320-781035a3-b9ef-44d2-a3f1-b40fa4a74a6e.png"> | <img width="391" alt="Снимок экрана 2022-06-13 в 20 11 25" src="https://user-images.githubusercontent.com/93148512/173408486-de6fd2be-ba70-4bb8-8be9-f113cc4105ff.png">
<img width="401" alt="Снимок экрана 2022-06-13 в 20 10 55" src="https://user-images.githubusercontent.com/93148512/173408502-a0af1c6a-c5ec-4532-8075-2918976895d7.png">

## Z-ДНК и гомологичные гены разных организмов
# Информация по полученным гомологичным кластерам

<img width="415" alt="Снимок экрана 2022-06-13 в 20 35 13" src="https://user-images.githubusercontent.com/93148512/173411735-b05b98ae-e12b-4de7-b5ae-42877336113c.png">

Всего кластеров - 1622

## Множественное белковое выравнивание

Результаты выравнивания находятся в директории `alignments`.
<details>
  <summary>Выравнивание для кластера №1</summary>
  
  ```
>WP_106874893.1_Candidatus_Phycorickettsia_trachydisci
MPFK------------SARRINRIAAVQCIYYYHSTSFDINKVQQDIKSLY-PNQALESDHEIFTSNLQHDHFEELINNF
LGNADIIDKRISANLKEGWTIDNLHLTLLSIIRIGIGELL-YTNNTPFQVIISEFADIAGLMLQKNEVAFVNSIMQKVHN
DRE----LFF
>WP_013045040.1_Candidatus_Puniceispirillum_marinum_IMCC1322
MAKE---NAELKPVPVRRRSASRVSSIQILYQSQITDRASVDFAPDYLTHYAPDVS----KSFRVKDLDHEHLNALYTGV
EKEMVLLDEDIADSLASGWSIKRLPLIELTLLRCGAYELR-FMPHIPARAVVSEYAAISDAC--GCEVAFVNAVLDRLSR
IVRTVEMGTA
>WP_011282132.1_Candidatus_Pelagibacter_ubique_HTCC1062
MRTP-----------YNPNQSPRVIIIQKLYGNFFNDDTDLTFPK---------------------HRFKKFIKDVVLGT
IERDEVIKEEVKKYLSEDLELTNLDQVFQVIVKSAIFEFL-YKPKVSSKIIIKEYLDASNFFLEDGQTKYLNAILDKIAK
KIRT---TNA
>WP_066767018.1_Candidatus_Viadribacter_manganicus
MSAH---N-------NLSRSIARLGTVQALYQMEVSGATTAEVIADFADGKLPRQT-E--ASYTDSEGDLDLFKLLVEKA
VDRQATYDRTIARHLGKGWRLERIDAVARAILRAGAAELE-QRTDIPVAVVIDEYVEVAKAFFEGPEPGFINAALDAAAR
DLRPTE-QGA
>WP_085783692.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MEVMGDRPSKMRPGKFEAARVARVAAVQAMFQIFHQSLSKDEVIEQFLRYRLSSKD------Y-PCVANKSLFADLVNAT
LNRLEEIDHIIEESLTDEYTLDRLDPVLKAILRVGAAELLNQQTKIPPPVVISEYVDITKGFYEGTEPAFVNSLLDSLAK
KLGLSLTPHK
  ```
</details>

<details>
  <summary>Выравнивание для кластера №2</summary>
  
  ```
  >WP_013045233.1_Candidatus_Puniceispirillum_marinum_IMCC1322
----MKVTMLGCGTSVGVPALGN--AGWGACDPTDPRNRRQRCAMLIQK---------DDTTILVDAGPDIRNQLLPHML
KKIDAVLITHTHSDHVAGLDDLRAFY-WPDRNIIPLYATASSRTDIVNRFPYLFTK-NPKSPSYFVPP-----MDVTEIK
AGQTLNF--GSINIDVLHQEHGNISSLGFVFNGKFGYSTDVIDMPEESFAKLRDLDLWIVEALRPE-PHSSHSHYENTFA
WIEAMKPKHAVLTHLGLEADYAELAELCPAHVEPGVDGLSFTL-D
>WP_085783546.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MQ--SKAIILGCGGSGGVPSLGPNGGYWGACDPKNPRNIRSRTSSYIEM---------SGVRILIDTSTDLRQQFLKNNL
TDFDAVLYTHAHADHTHGIDELRALFFVRNEKSIPVYGTAECMKDIERRFNYLITPTSDVYPKV---------LIPNVIQ
CD-TFYV--QNLEILAFQQGHGNQPSTGYRFG-TMAYSTDFNYLSEESIEKLKGLKIWIVDCLSKEPPRRTHNHLDLTLH
WIERVRPERAILTHMNATLDYDWLQSVLPQNVEPAFDGMIIE--F
>WP_106874031.1_Candidatus_Phycorickettsia_trachydisci
M---LQITVLGCGSSLGTPVIG---CKCETCSSSDPKNKRLRSAILITKFHPN----DSKTNILIDSGFDVRTQLLRAGV
SKLDATIITHDHADHISGLDELRVFSPLGSNKILPIYFTSATGARIIPRYQYLFDN-KN--------------LNANTIE
YDSSINI--CDVSISFFKQNHIVMDSLGIRIN-NFVYANDVAFFYDESLRYLDNIDTFVIDCCDYQ-STRVHAGLDRVLS
WINQFKPKVTYLTNLSHKIDYYKIKNMLPVNVYPAYDGLVFK--I
>WP_066766633.1_Candidatus_Viadribacter_manganicus
MSGTLRVTVLGCGSSGGVPRAT---GDWGVCDPNEPKNRRTRCGIMLQKWNGQATSASEATTVLIDTPPELRQQLADAAP
SHLDAVLISHDHADQIHGFDDIRAFF-IKQRSQIPTFIDAKTRLSFMQRFGYAFMS-EGGYPAIARDAGHMTPLIPVEI-
-D--GPG--GKLEVLPLDQDHGFSRSLGFRIG-PIAYSNDLVDMPEATLAQLGGLQLWIVDALRDT-PHPTHAHVAKALE
WILELKPQRAVLTNMHIDLDYQALKARLPLGVEPAYDGWAGEYPV
>WP_011282101.1_Candidatus_Pelagibacter_ubique_HTCC1062
MS--LKFVILGSGSSMGVPRAD---GYSGDCDLKNKKNFRTRCSALIKF---------NDQNILIDTSPDLRSQLLKNKI
KSISKVFYTHLHADQTHGINDLRPFF-LINKKQIPVYADINTKKYLLSTFKYCFKS-SFGYPST---------LNINSLK
KKHEFIIKDKKIKIESIPVQHGKIKSICYLINNKLAYASDISLFFKKDYKKLKNLEYLIIDCLWYR-NHSAHFNLDQVLE
IVKILTPKKTILTNMHSDLDYAKLKKKLPKNIIPGFDGLTVSLKN
  ```
</details>

<details>
  <summary>Выравнивание для кластера №3</summary>
  
  ```
>WP_085784875.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MPTINQLIRKPRESSPPRNKVPALKSCPQRRGVCTRVSTTTPKKPNSALRKIARVRLTSGFEVTGYIPGEGHNLQEHSVV
LIRGGRVRDLPGVRYHVIRGALDTQGVQNRKKSRSKYGTKRP-K
>WP_106874161.1_Candidatus_Phycorickettsia_trachydisci
MPRINQLVKQGRVLKTKKSTAPALQKCPFKAGVCMSVMTKSPKKPNSALRAVARVRLSNGFEVISYIPGEGHNLQEHSKV
LIRGGRVKDLPGVRYHIVRGSFDTQGVKNRKQSRSLYGAKKPKQ
>WP_066775133.1_Candidatus_Viadribacter_manganicus
MPTINQLIRKPRHPKPTRNKSPALKASPQRRGVCTRVYTTTPKKPNSALRKVAKVRLTTGIEAVCYIPGEGHNLQEHSVV
LIRGGRVKDLPGVRYHILRGVLDTQGVKDRKKRRSLYGAKRP-K
>WP_013047256.1_Candidatus_Puniceispirillum_marinum_IMCC1322
MPTINQLIRHGRKRPVERTKVPAMEACPQKRGVCTRVYTTTPKKPNSALRKVARVRLTNGFEVSSYIPGEGHNLQEHSVV
LIRGGRVKDLPGVRYHIIRGTLDTQGVSDRRQRRSKYGAKRP-K
>WP_006996807.1_Candidatus_Pelagibacter_ubique_HTCC1062
MPTINQLLRKKRIKPVARNKVPALQKQPLKRGVCVKVYTTTPKKPNSALRKVARVRLSNGFEVTAYIGGEGHNLQEHSVV
LIRGGRVKDLPGVRYHILRGNLDTQGVANRKKRRSLYGTKKG-K
  ```
</details>

<details>
  <summary>Выравнивание для кластера №4</summary>
  
  ```
 >WP_066768774.1_Candidatus_Viadribacter_manganicus
MKI-AVLKESAPGETRVAATPETVKKIVGLGHSVTVEAGAGARASFPDEQFKAAGAEISADG--GIGAADLVVKVRRP-S
D--A-----EIGKIKAGSGFVSLLEPYGDKATIDALAKAKIEALAMEFIPRISRAQSMDALSSQANLAGYRAVIEASALY
GRAFPMMMTAAGTIAAAKVFIMGVGVAGLQAIATARRLGAVVSATDVRPATKEQVASLGGKFIAVEDEEFKQAETTAGYA
KAMSGEY-QAKQAALVTEHIAKQDIVITTALIPGRAAPVLVTEAQAKSMRPGSIIIDLAVAQGGNCPLSKPDELVEVGGV
KIMGFTNLPARLASDASSLYAKNFLALLPLLADKESKAFAPAWDDEIIKGAMLSKGGALVHPHFAPKTAA
>WP_106874551.1_Candidatus_Phycorickettsia_trachydisci
MKI-AALKERHPNETRVAITPDIVKLFIRSKFDICIETKAGLAAGFSDEDYIAAGAKVSKVPLEVIGDADIILKVQPTPI
D--EK--INELSFAKKGALIIGLLLN-SEKNLFEAYADKKINAMSLELMPRISKVQHMDVLSSQSNLAGYRAVIEAAYHC
LGIFPMLMTSAGTILAKKTLVIGAGVAGLQAIATAKRLGGIVQAYDVRQATKEQVESLGAKFINTHLQ---DCETKSGYA
KAKLDSASVKAQNEILTNAAKNNDIIITTAQIPGKKAPILISKEMIAQMKPGSIIIDLAAGTGGNTELTKADKIVDINGV
KIIGYTNFAGLVPNDASRLYAKNLYNVITYAFND----GVLNASDDVIKSMLVTFEGKVVYG-------L
>WP_085784706.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MKI-AVLRERRPGEKRVAATPETVKKMIGLGASVVIEKGAGLASSYLDEAYKDSGAKIAADAASALDGADIILKVQRP-V
LKGEQTGTDQLEKAKKGAFILALFSPYNNTKDLKVYAKQGLTTLALELVPRITRAQTMDVLSSQTNLAGYRAVIEAAYVY
DRAFPMMMTAAGTIPPAKILILGAGVAGLQAVATAKRMGAVVSAFDVRAAAREQVESLGGTFISVESDE--KGEGTGGYA
KEMSADY-QKRQADKIKATLEKSDIAITTALIPGKTAPRLITEDMIAVMKPGSVILDMAVESGGNCALSEPGKIVEKNGV
QIIGYINLPSRIARDASALYARNVLNYLTLLIDKDSKKINLNFEDEIIAATTLTHGGEVVHPNF----KA
>WP_013046211.1_Candidatus_Puniceispirillum_marinum_IMCC1322
MPTLFVPAEIASGETRCAVVPETISKLVAQGLDVTVQSGAGASSSYDDAAFTEAGAKIIKTAKDGYAKADLIFKVRPP-Q
I--E-----ETALIQKNTIILSLFEGYVDAKRNAAIAKTGATVFGLELVPRISRAQSMDVLSSQSNLAGYRAVIEGAYEF
GRAFPMMMTAAGTIPPTKVLVMGAGVAGLQAIATAKRLGAIVSATDVRPAAKEQVESLGGKFVAVEDEEFKQAETDGGYA
KAMSAEY-QAKQQVLIAETIRVMDIVITTALIPGRPAPELVSAEMVASMKSGSVIVDMAVEQGGNCALSKPDEIVKANDV
TIIGHCNMPGRLPKDASSLYARNLMNFVGLLWDKEAGALTINKDDEIIAGSLVAEAGQLVHPSV----TS
>WP_006997330.1_Candidatus_Pelagibacter_ubique_HTCC1062
MRI-VSILENQNIDKRIAITPEIAKKYIALGFQITLVEKYGEHLGFKDSDYKELGVEISTDETQILSKANIIIQLGLL-S
D--E-----NLSNLKENQTLIGVFNPYNNKEKIENLSKKNINVFSLEMLPRITRAQSMDILSSQANLAGYKTVIESFANF
EKAIPMMMTAAGTIPAAKVLVVGAGVAGLQAIATAKRMGAIVFATDVRMASKEQVESLGGKFLTVEGSE--NLETEGGYA
KEASEEF-KKKQEDLLAETLKKIDIVICTALIPGKKAPLIIKGSMIDNMQSGSVIYDLAAVQGGNAEFTEVDKVVVKNGV
KIMGETNILNKLPVSASNLYSKNVFNFVSNLYDKENNKININLEDEIIEKTLIK----------------
  ```
</details>

<details>
  <summary>Выравнивание для кластера №5</summary>
  
  ```
>WP_106874598.1_Candidatus_Phycorickettsia_trachydisci
MAKL----INDLHLAAKALQQGQVVAFPTETVCGLGASALSFDACNRIYQLKGRPSFNPLIVHVADLNQAKLIGEFSDIA
IKLAEKFWPGPLTLVVKLKQTANIASNVTAGLDTIAIRVSAHPITSELLKLANIPIAAPSANLSGYVTSTSPQHVLNDFT
DK--DLYVLSSDEASQYCGLESTIIDTT--GK-LTILRSGVILPPDIQEVCGIW------PETCCQDNDAPKAPGMLLAH
YSPVSKLRLNAAKLKNDEVGLDFNNHFT----SNFSLSKSGNLEEAAHNLYALLREADRQVIQKGLKGIAVAKIPYVGIG
IAINDRLFKAASKK
>WP_066767745.1_Candidatus_Viadribacter_manganicus
---------MNVARGAEVLRAGGLVVFPTETVYGVGADATNPRAVARIFAAKGRPQFNPLISHVLGLSDAEGHGVLHPTA
RALIEKFWPGPLTIVVPRRADSPVAELACAGLATIALRSPSHPLARDLLAAFGGPVVAPSANRSGHVSATTAAHAAADLA
DA--VDLI--LDGGASEVGLESTIVAIDAEGR-ATLLRPGAIGRAELEAVCGPL------ATP---ASETIAAPGMMESH
YAPRARIILDAATPPVGAAYLAFGAEAPA---GGLTLSASGDLTEAAANLYAHLRALDAT----GADTIAIAPIPGGGLA
EAIRDRLARAAAPR
>WP_013045563.1_Candidatus_Puniceispirillum_marinum_IMCC1322
MTECLSISENSVARAVDLLRAGQLVAFPTETVYGLGGDACNDHAVAGIFKTKGRPSFNPLISHVATIDMAFTLGKKTAIA
EILAYNFWPGAMTMILDRTKDCKVSMLTTAGLDKIAVRVPSHEAATQLLSSFGGPLAAPSANPSGRISPSTVSHVIDGLG
GQ--IDLI--LDGGACESGLESTIIDCS--ANIPVILRPGGITRDAVNDVLNQAGHRLLEQTIAGNDDKRPVSPGQLASH
YAPQLGVRMNATNAEDTEIAIGFGSQMHE---APLNLSLSGNLTEAAANLFALLHKADKLGAKQNATHIAIAPIPDHELG
EAINDRLRRASAPR
>WP_011281810.1_Candidatus_Pelagibacter_ubique_HTCC1062
MKSN----QSNIKKAKKYLDKNYCIGVPTETVYGLAANAYKNSAVKKIYNLKKRPKNNPLIVHYHDIDSLKKDCLINDNF
IKLYKKFSPGPITYVLQLKKNSKISKYVTNNKKSLAVRFPKHTIFKNLLKQLDYPLAAPSANITTKVSAVKAKDVKEEFG
NK--IKYI--LDGGTCAIGIESTIVNLT--AK-PTILRLGGLDISKIQKALGFK------MNIST-NPKKKIAPGQSRLH
YSPGIPLRMNVTKPKNNEAFILIKKKKTKLK-SYFYLTSKSNLDEAAKNLYSCLRKIKNK----GYKSIAVEKIPNIGLG
KTINDRLRRA-SKY
>WP_085783836.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MPEI----STDLDLAVHYLKDGALVALPTETVYGVAGDATNDKAVANIFALKKRPEFNPLIIHYPHITFMNQDVEITELA
KKLANAFWPGPLTLVLPRRQESKISFLASAGLDTLAVRIPSHPMTLQILRNFGKPVAAPSANPSSKVSPTSAQHVFDSFK
NNPLLPLI--IDGGACHVGIESTIIDLT--VPIPKLLRPGKITAEEIKNLTGIV------LENQSHSKSNPKAPGQLKVH
YAPHIPLYLNCTAPKKDQALLAFGPHIPKGAAYSLNLSPSGNLNEAATNLFAMIRLLDND----RYASIAVMPIPKEGLG
HAINDRLKRA-AQE
  ```
</details>

<details>
  <summary>Выравнивание для кластера №6</summary>
  
  ```
>WP_066774291.1_Candidatus_Viadribacter_manganicus
MMQPKKTKFRRAHKGRIKGNTKGGSALNFGQFGLKALEPNRVNAREIEAARRAITREMKRQGRVWIRIFPDVPVSQKPVE
VRMGKGKGAVEFWAARVAPGRIMFEIDGVPETVARESLRLGAAKLSVRTKIVARIE-GL
>WP_013047267.1_Candidatus_Puniceispirillum_marinum_IMCC1322
MLSPKRTKFRKAHKGRIHGNAKGGTQLNFGSYGLKAMSPERVTARQIEAARRAITRHLRRTGRVWIRIFPDVPVSSKPAE
VRMGKGKGSPEFWVARVKPGRIMFEIDGVPWELAQEAFRLAAAKLPLDTKIVRRLGDSD
>WP_085784886.1_Candidatus_Nucleicultrix_amoebiphila_FS59
MLAPKKTKYRKAHKGRIHGMSKGGTRLNFGSFGLKALEPTRVTARQIEAARRAITRHIKRSGRVWIRIFPDVPVSTKPAE
VRMGSGKGNPEFWVCRVAPGRILFELEGVPADLAKEAFLLAAAKLPIKTKFVTRLASGV
>WP_106874576.1_Candidatus_Phycorickettsia_trachydisci
MLVPKKQKFRKAHKGRIAAKVKRGDQISFGSFGLKALELERINSRQIEAARRAATRVMKREGKLWIRIFPDIPVSKKPSE
VRMGKGKGSVEFYVARISPGRVLFEVDGVSDDACLEALRLAAAKLPLKTKVVKRY---E
>WP_006996818.1_Candidatus_Pelagibacter_ubique_HTCC1062
MLQPVRTKYRKAHKGRIHGTATRASKINYGSFALKAMAPERIIGKQIEAARVALTRHMKRQGRVWTRIFPNIPVSKKPVE
VRMGKGKGAPEYWACRVKPGRILFEIDGVSETIAKEALYKASAKLPIKTKFIKRF---A
  ```
</details>

<details>
  <summary>Выравнивание для кластера №7</summary>
  
  ```
 >WP_066767064.1_Candidatus_Viadribacter_manganicus
M-IIGIGSDIIDIRRVEKTLSRFGERFTNRIYTEKERARAE---RRPEQRAATYAKRFAAKEATSKALGTGIRRGVFWRD
MGVANLPSGQPTMVLTGGAARRLEQLTPPGHVAHIHVSLTDDYPLAVGFVIISAELAPIQPGPGE
>WP_106874021.1_Candidatus_Phycorickettsia_trachydisci
M-ILGIGTDIVNIDRIGKIYNKFPHRFAHRILSTQEEVIYGQFQNNE-QKIRYLAKRFAAKEAFVKALGIGMG-DISFRD
ISILNDARGKPYIKFAKTI------------EFNMELSISDEHDYAVAFVVLWA-----------
>WP_006996870.1_Candidatus_Pelagibacter_ubique_HTCC1062
MKILGIGVDIVENIRIHKSLKNV--NFIKRVFSSSEILLAK---KIT-NKKSFYSKRFAAKEAFSKAIGTGFRENLNFKD
ITVINDKLGKPSFVVTDKIKKIVKKRFK-ISSFNFFLSISDEKKYSVAYVILQK----------K
>WP_013045405.1_Candidatus_Puniceispirillum_marinum_IMCC1322
M-ILGIGTDLVDSRRIANSLDRFGARFETRIFTEKEIETAR---NRP-DPSLFYAKRFAVKEAVYKALSAAEVAGLGWRE
AETLNDPNGAPRLHLSGGCKTALERLTPEGYKASIHISLSDELPYAQAFVVISASM--IQ--TGI
>WP_085784762.1_Candidatus_Nucleicultrix_amoebiphila_FS59
M-ILGIGSDIVEIERIAKLQERFGERFLEKVFTPDERRRAL---DSI-NGAASLAKRFAAKEAFLKALGSGFSQGVSWHE
IMVTNDPQGAPYITLTGQALSLAENKVPSGHQLAIFLSLSDSQTVAHAVVVLEAR--------PE
  ```
</details>

<table>
    <thead>
        <tr>
            <th>Название кластера</th>
            <th>Кол-во генов</th>
            <th>Гены</th>
            <th>Функции генов</th>
            <th>Расположение Z-ДНК</th>
            <th>Z-Hunt score</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #1</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066767018.1</td>
            <td rowspan=1>transcription antitermination factor NusB</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>884, 38833, 3428</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013045040.1</td>
            <td rowspan=1>transcription antitermination protein NusB</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>752, 8922, 784, 2752</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874893.1</td>
            <td rowspan=1>transcription antitermination protein NusB</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011282132.1</td>
            <td rowspan=1>transcription antitermination protein NusB</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085783692.1</td>
            <td rowspan=1>transcription antitermination protein NusB</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>784</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #2</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066766633.1</td>
            <td rowspan=1>MBL fold metallo-hydrolase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>907, 980, 27872, 1515</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013045233.1</td>
            <td rowspan=1>MBL fold metallo-hydrolase </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>948</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874031.1</td>
            <td rowspan=1>MBL fold metallo-hydrolase </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>583</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011282101.1</td>
            <td rowspan=1>MBL fold metallo-hydrolase </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085783546.1</td>
            <td rowspan=1>MBL fold metallo-hydrolase </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>2752, 4914</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #3</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066775133.1</td>
            <td rowspan=1>30S ribosomal protein S12</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013047256.1</td>
            <td rowspan=1>30S ribosomal protein S12</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>12723</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874161.1</td>
            <td rowspan=1>30S ribosomal protein S12</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_006996807.1</td>
            <td rowspan=1>30S ribosomal protein S12</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085784875.1</td>
            <td rowspan=1>30S ribosomal protein S12</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>1820, 16770, 948, 783</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #4</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066768774.1</td>
            <td rowspan=1>Re/Si-specific NAD(P)(+) transhydrogenase subunit alpha</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>980, 883, 38833</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013046211.1</td>
            <td rowspan=1>Re/Si-specific NAD(P)(+) transhydrogenase subunit alpha</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>38833, 1430, 762</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874551.1</td>
            <td rowspan=1>Re/Si-specific NAD(P)(+) transhydrogenase subunit alpha</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>980</td>
        </tr>
        <tr>
            <td rowspan=1>WP_006997330.1</td>
            <td rowspan=1>Re/Si-specific NAD(P)(+) transhydrogenase subunit alpha</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085784706.1</td>
            <td rowspan=1>Re/Si-specific NAD(P)(+) transhydrogenase subunit alpha</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>3428, </td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #5</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066767745.1</td>
            <td rowspan=1>L-threonylcarbamoyladenylate synthase </td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>650, 752, 980, 3428...</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013045563.1</td>
            <td rowspan=1>L-threonylcarbamoyladenylate synthase </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>13713, 883, 698</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874598.1</td>
            <td rowspan=1>L-threonylcarbamoyladenylate synthase </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_011281810.1</td>
            <td rowspan=1>L-threonylcarbamoyladenylate synthase</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085783836.1</td>
            <td rowspan=1>L-threonylcarbamoyladenylate synthase </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #6</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066774291.1</td>
            <td rowspan=1>50S ribosomal protein L16 </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>980, 783, 3428, 13713</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013047267.1</td>
            <td rowspan=1>50S ribosomal protein L16 </td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>883, 908</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874576.1</td>
            <td rowspan=1>50S ribosomal protein L16 </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_006996818.1</td>
            <td rowspan=1>50S ribosomal protein L16 </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085784886.1</td>
            <td rowspan=1>50S ribosomal protein L16 </td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
    </tbody>
    <tbody>
        <tr>
            <td rowspan=5>Cluster #7</td>
            <td rowspan=5>5</td>
            <td rowspan=1>WP_066767064.1</td>
            <td rowspan=1>holo-ACP synthase</td>
            <td rowspan=1>Нет</td>
            <td rowspan=1>783, 3403, 3428</td>
        </tr>
        <tr>
            <td rowspan=1>WP_013045405.1</td>
            <td rowspan=1>holo-ACP synthase</td>
            <td rowspan=1>Промотор</td>
            <td rowspan=1>908, 848, 705</td>
        </tr>
        <tr>
            <td rowspan=1>WP_106874021.1</td>
            <td rowspan=1>holo-ACP synthase</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_006996870.1</td>
            <td rowspan=1>holo-ACP synthase</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
        <tr>
            <td rowspan=1>WP_085784762.1</td>
            <td rowspan=1>holo-ACP synthase</td>
            <td rowspan=1>нет</td>
            <td rowspan=1>-</td>
        </tr>
    </tbody>
</table>

## Визуализация расположения участков Z-DNA
Для демонстрации было выбрано 7 кластеров. В некоторых из них во всех гомологичных белках сохраняются участки Z-ДНК, в некоторых - нет (такие кластеры были выбраны специально для иллюстрации). 

<img width="949" alt="Снимок экрана 2022-06-13 в 20 50 55" src="https://user-images.githubusercontent.com/93148512/173414698-14243d4a-b232-4575-8922-31023b3c3b4b.png">

<img width="937" alt="Снимок экрана 2022-06-13 в 20 52 13" src="https://user-images.githubusercontent.com/93148512/173414743-5bb6b83f-40aa-4c05-9851-1d0e185ac223.png">

<img width="871" alt="Снимок экрана 2022-06-13 в 20 52 31" src="https://user-images.githubusercontent.com/93148512/173414772-d5c7458c-6c5e-4881-8670-7afbb4abfa61.png">

<img width="898" alt="Снимок экрана 2022-06-13 в 20 52 46" src="https://user-images.githubusercontent.com/93148512/173414796-c194801a-7b71-4d8c-9197-46383282f593.png">

<img width="837" alt="Снимок экрана 2022-06-13 в 20 53 02" src="https://user-images.githubusercontent.com/93148512/173414823-f7dc545e-8175-4ea6-a673-ab257423207b.png">

<img width="903" alt="Снимок экрана 2022-06-13 в 20 53 13" src="https://user-images.githubusercontent.com/93148512/173414844-425bb55a-cf31-4ec1-b21b-03195c056d8d.png">

<img width="846" alt="Снимок экрана 2022-06-13 в 20 53 25" src="https://user-images.githubusercontent.com/93148512/173414884-8bfa1ae0-646b-4f16-8c16-adb0dd4c6d35.png">
