# Proof_of_Concept
See if it's possible to automaticly recognize an object in a picture, translate it en have the translation being voiced at the same time


### 15/12
* Bekijken object herkennen in foto. 
* [Google image recognition](https://cloud.google.com/vision/?utm_source=google&utm_medium=cpc&utm_campaign=emea-emea-all-en-dr-skws-all-all-trial-e-gcp-1002258&utm_content=text-ad-none-any-DEV_c-CRE_175901543514-ADGP_SKWS+%7C+EXA+~+1%3A1_EMEA_EN_ML_Vision+API_TOP_image+recognition+api-KWID_43700016288634079-kwd-40564249699-userloc_1001021&utm_term=KW_image%20recognition%20api-ST_image+recognition+api&ds_rl=1245734&gclid=Cj0KCQiAgs7RBRDoARIsANOo-Hjca0GTNetIZh_Qz1FOPFtBN5nGcOwnIpCY1y9E7PQG_8s3xP8hr9QaAj3DEALw_wcB&dclid=CNTphKGAjNgCFQU-4AodVrkJkg) api ontdekt.

* Bekijken hoe te gebruiken via de Google [documentatie](https://cloud.google.com/vision/docs/quickstart)
* Cloud Platform Console nodig. Kan free trial doen maar moet credit card gegevens invullen. Moet nog vragen aan ouders.
* Aantal stappen ook nodig vooraleer de api kunnen gebruiken. Zou normaal gezien niet lang mogen duren (5-10min)



### 16/12
* Google Cloud Platform 12 maanden trial gestart.
* Eerste image geprocessed via de [Quickstart](https://cloud.google.com/vision/docs/quickstart)
* API key gegenereerd voor gebruik op web - [Use google vision api](https://code.tutsplus.com/tutorials/how-to-use-the-google-cloud-vision-api-in-android-apps--cms-29009), [Credentials](https://console.cloud.google.com/apis/credentials?project=double-genius-189210)


### 21/12
* Bekijken integratie API voor web - [credentials](https://support.google.com/cloud/answer/6158857?hl=en), [video tutorial](https://www.youtube.com/watch?v=nMY0qDg16y4) - [Speech API](https://www.youtube.com/watch?v=wzp9dfVpeeg)


### 23/12
* Bekijken hoe API gebruiken überhaupt - [Google demo Java](https://www.youtube.com/watch?v=tVIIgcIqoPw), [Google demo Python](https://www.youtube.com/watch?v=IVjZMIWhz3Y)
* Bekijken tutorials Google API's - [Tutorial overzicht](https://cloud.google.com/vision/docs/tutorials), [Tutorial label detection](https://console.cloud.google.com/getting-started), [label detection](https://cloud.google.com/vision/docs/detecting-labels)
* Veranderen van onderwerp naar:



# Proof of concept
Zien of het mogelijk is om een scanner een afbeelding te laten omzetten in tekst die op de afbeelding lijkt.

### 23/12
* Opzoeken of er een manier is om een scanner geprinte tekst te laten herkennen.
* OCR ontdekt, optical character recognition. Herkent patronen in handgeschreven teksten en kan ze vertalen naar "geprinte tekst" zodat de computer het kan verstaan. Wordt o.a. gebruikt bij het ordenen van mail. OCR herkent de patronen van donker en licht, waaruit de letters bestaan. We kunnen een foto (meestal jpg) dan omzetten naar een doc of txt file. De geschreven tekst wordt vergeleken met allerlei bestaande fonts om eraan uit te geraken om welke letters het gaat. Er wordt wel nog altijd aangeraden de teksten na te lezen aangezien het niet error proof is. Sheet feed scanners worden vaker gebruikt dan flatbed scanners omdat er meerdere pagina's na elkaar kunnen worden verwerkt. Bij flatbed scanners moet het verwerken per pagina gebeuren. Er zijn ook programma's die de tekst kunnen nakijken en opvallende schrijffouten kunnen verbeteren. Soms kijken de programma's zelfs naar de woorden nabij het woord dat wordt gecheckt. Zoals "de blaffende bond" wordt verbeterd naar "de blaffende hond" omdat er "de" en "blaffende" bij het woord "hond" stonden. - [info OCR hp printers](http://h71036.www7.hp.com/hho/cache/608037-0-0-39-121.html), [uitleg OCR](http://www.explainthatstuff.com/how-ocr-works.html)
* Zaken die kunnen helpen bij het beter lezen van letters (en eventueel later van een image): extra contrast tussen de lichte en donkere stukken.
* Sommige programma's veranderen gescande afbeeldingen meteen naar graphics dus het zou kunnen dat enkel twijfelachtige afbeeldingen zoals koffievlekken kunnen omgezet worden naar tekst. Zullen we moeten testen.
* Beslissen test runs. Gewone image scannen, image met enkel een duidelijk object en witte achtergrond scannen, een zwart-wit image scannen



### 24/12
* Inspiratie opdoen voor "kunstwerken" met tekst, die we hopen te creëren.
* Kunst met typografie: [interview Yves Velter](https://vimeo.com/86238888), [Blanck, beeld en typografie](https://www.youtube.com/watch?v=--h0FXVoOVU&feature=youtu.be), [Einaudi, typografie bij muziek](https://www.youtube.com/watch?v=k9NM-yK1C2I), [Pietrella, foto's omzetten in tekst via stamp](https://www.youtube.com/watch?time_continue=16&v=pd-edgSDVo4)



### 26/12
* Bekijken welke programma's er zijn om OCR mee te doen. Eventueel een ouder programma / minder advanced om de beeldherkenning eigenschap nog niet in het programma te hebben zitten.
* [Microsoft OCR programma](https://www.microsoft.com/nl-be/store/p/a9t9-free-ocr-software/9nblgggz5nsn#) - Test failed, kon geen tekst van afbeelding maken, [app OCR](https://www.microsoft.com/nl-be/store/p/photo-to-text-ocr/9nblggh6hrzh), [app fast OCR](https://www.microsoft.com/nl-be/store/p/fast-ocr/9nblggh52svj#), [Online OCR](https://www.onlineocr.net/) - Foto appel proberen inladen, "Kan tekst niet lezen". 

* Proberen met vagere foto's, waar tekst in verwerk zit?
* Voorbereiden 3 testen: tekening zonder schaduwen, simpele lijnen, met stempel woord tekening, met stempel reeks woorden simpele vorm maken, morgen checken: herkent hij hier iets uit?


### 8/01
* Maken tekeningen + met stempels waar tekst in zit
* Tekeningen inscannen


### 9/01
* Test: Kan hij hier iets uit maken?
* Test 1: gewone tekening kan hij niks uit maken
* Test 2: Tekening met stempels waar de tekst schuin of over elkaar staat. Herkent geen tekst doordat er geen duidelijke letters in voorkomen.
* Test 3: Ster vorm gemaakt uit stempels met tekst: herkent een aantal woorden maar niet veel.. komen ook niet op de juiste plaats

* Programma's zijn misschien te geavanceerd geworden om dit met OCR te kunnen doen? Herkennen enkel cleane tekst en zien non-tekst dus niet meer als mogelijke tekst..




