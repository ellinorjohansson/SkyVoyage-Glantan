# Generell information

## Prototyp

Vår prototyp har till största delen ingen funktionalitet inlagd, utan vi har istället exempel som visar på hur sidan ska fungera.

Ni kan se vår [Figma Prototyp](https://www.figma.com/design/HeVlmmxQgbXIfMEeCxn0BB/Mandarinfiskarna?node-id=5-50&t=Cc5cge2QwUTRjPGO-1) här.

## Kontakt

Vid frågor så vänligen skriv till Lenita Dahlin eller Malin Rosenquist i grupp "Mandarinfiskarna" på Teams.

**Vi finns tillgängliga dessa tider:**

- Mån-Fre
- 10-15 (Lunchpaus 12-13 då vi inte är tillgängliga)
- Vi svarar så snabbt vi kan, men som senast 2h senare (under kontorstid).

## Filer

Ni finner alla filer ni behöver i "components" i vår Figma.

För att ladda ner bilderna antingen som PNG eller SVG så gör ni såhär:

1. Klicka på (select) den grafik ni vill ha (t.ex flygplanet eller luftballongen)
2. I inspector panel (på höger sida av skärmen, där alla redigeringsalternativ finns) gå längst ner till "Export"
3. Klicka på "Export" och välj det filmformat ni behöver i dropdown menyn, sedan klicka "Export" knappen för att spara den till din dator.
4. Klart!

## 📝 Specifika noteringar för styling - Alla versioner

### Formulär - knappar

- "Skicka in" knappen ska vara disabled tills hela formuläret har blivit ifyllt.
- När knappen är disabled så bör opaciteten vara lägre och den ska inte gå att klicka på.
- När formuläret är helt ifyllt så blir knappen aktiverad.

### Rundade hörn

Alla cards, knappar, och inputfält har rundade hörn, och de ska vara rundade till samma grad. I Figma så har vi rundat dem med corner radius 8.

### H1/Logo

Vår logotyp är baserad på idéen av ett akrobatflyg som har skrivit hemsidans namn med rök. Se _alltid_ till att planet är vinklat och positionerat så att bakdelen matchar vinkeln av "svansen" på den sista bokstaven.

## Cookiebar/ popup

- Cookie-popupen bör vara synlig på varje enhet (mobil, tablet, desktop).
- Den ska placeras mitt på sidan och sitta fast där, vilket innebär att den ska vara synlig även när användaren scrollar.
- Resten av sidan bör vara någorlunda mindre synlig så länge denna popup är kvar (tänk som en overlay med ca 50% opacity).
- Cookie-popupen ska förbli synlig tills användaren har gjort ett aktivt val, genom att antingen acceptera eller avböja cookies.
- Denna popup ska _inte_ ha rundade hörn.

- Bakgrundsfärg: #F57E4B
- Textfärg: #000000
- "Acceptera" Knapp: #0077B6
- "Avböj" knapp: #595959
- Textfärg knappar: #FFFFFF

## 🎨 Färger

### Primär - Prussian Blue - #0A374F

Bakgrundsfärg på sidan

### Sekundär - Charcoal - #224B60

Används som bakgrundsfärg på alla cards, både text och bilder.

### Accent - Payne’s Gray - #385D70

Används för fälten i boknings-formuläret på sidan “Bokning”

### Accent - Coral - #F57E4B

- Alla knappar utom de i cookie bar.
- Alla ikoner, både för sociala medier samt de i menyn på mobilversionen.
- Används för att markera vilken sida man är på i deskopversionen genom att lägga till ett streck under den texten i navbar.

### Accent - Honolulu Blue - #0077B6

Används till “Acceptera” knappen i cookie bar

### Text - White - #FFFFFF

- H1/ Logo
- All text utom den på “Läs mer” & "boka" knapparna
- Text på cookie bar knappar

### Text - Black - #000000

- Text på alla orangea knappar
- Text på Cookie-bar/ cookie-popup

## 🖊️ Typsnitt

[Over the Rainbow](https://fonts.google.com/specimen/Over+the+Rainbow) - Calligraphy

[Jura](https://fonts.google.com/specimen/Jura) - Sans-serif

[Inter](https://fonts.google.com/specimen/Inter) - Sans-serif

# 🖥️ Desktop

Bredden utgår från 1440 px.

### H1

Over the Rainbow, 90px

### H2

Jura, 45px

### H3

Jura, 22.5px

### Paragraf/ brödtext

Inter, 20px

### Knapptext - "Acceptera" & "Avböj" i cookie bar, samt alla "Läs mer" & "boka" knappar

Inter, 20px

## Specifika noteringar för styling - Desktop

### Margin i textrutor

Texten bör alltid ligga 45px ifrån alla sidor på textrutorna.
Med andra ord, margin på 45px på alla sidor.

### Navbar

Vår navbar är en vit ruta som sträcker sig över hela skärmen.

**Opacity:** 38%

**Storlek:**

- Bredd: 100%vw
- Höjd: 70px

**Länktext:**

- H2
- Bör aldrig ligga närmare än 60px från högerkanten på sidan (i desktop)
- Bör alltid ha lika mycket plats ovanför och under i navbar rutan.

### Recenssioner

- **Hem:** Blandade recenssioner från både luftballong & akrobatflyg
- **Luftballong:** Endast recenssioner från turer med luftballong
- **Akrobatflyg:** Endast recenssioner från turer med Akrobatflyg
- **Bokning:** Inga recenssioner

### Footer

Sidan/"Företagets" namn samt dess slogan ska ligga centrerat.
Storlek & typsnitt:
Logo: Over the Rainbow, 41px
Slogan: Inter, 18px
Alla element bör ha lika mycket utrymme mellan varandra och från sidorna.

## Marginaler på sidan

Vi har inkluderat alla relevanta margins i Figma filen, så om något är oklart så rekommenderar vi att ni tittar där först.

Om ni har frågor efter det så vänligen hör av er till antingen Lenita Dahlin eller Malin Rosenquist i grupp "Mandarinfiskarna" på Teams, våra arbetstider finner ni ovan under "Kontakt".

### "Hem"

**Horizontala Marginaler:**

- 20px på höger och vänster sida av textrutorna
- 76px minimum mellan cards med information ang de olika flygningarna. De bör ligga nära nog att de ser ut att höra ihop, men det är okej att låta dem ligga lite längre isär på större skärmar.

**Vertikala Marginaler:**

- 45px mellan "header" bilden och den första textrutan
- 90px mellan den första textrutan och våra cards (luftballong och akrobatflyg)
- 90px mellan cards & textrutan för recenssioner
- 60px mellan recenssioner och footer.

## "Luftballong" & "Akrobatflyg" (dessa sidor har samma marginaler)

**Horizontala Marginaler:**

- 20px på höger och vänster sida av textrutorna
- 76px minimum mellan cards med information ang de olika flygningarna. De bör ligga nära nog att de ser ut att höra ihop, men det är okej att låta dem ligga lite längre isär på större skärmar.

**Vertikala Marginaler:**

- 45px mellan "header" bilden och den första textrutan
- 45px mellan den första och andra textrutan ("Turer med Akrobatflyg" och "Vanliga Frågor")
- 90px mellan den andra textrutan ("Vanliga Frågor") och våra cards (val av turer för luftballong och akrobatflyg)
- 83px mellan cards med de olika valen för flygturer.
- 90px mellan cards & textrutan för recenssioner
- 60px mellan recenssioner och footer.

## "Boka"

**Horizontala Marginaler:**

- 20px på höger och vänster sida av textrutorna
- 20px på höger och vänster sida av formuläret. På större skärm är det okej att ha större marginal.

**Vertikala Marginaler:**

- 45px mellan "header" bilden och den första textrutan
- 45px mellan den första textrutan ("Bokning") och bokningsformuläret
- 90px mellan bokningsformuläret och textrutan "Vanliga Frågor"
- 90px mellan textrutan "Vanliga Frågor" och footer

# 💻 Tablet

Bredden utgår från 768 px.

### H1

Over the Rainbow, 64px

### H2

Jura, 32px

### H3

Jura, 25px

### Paragraf/ brödtext

Inter, 18px

### Knapptext - "Acceptera" & "Avböj" i cookie bar, samt alla "Läs mer" & "boka" knappar

Inter, 18px

## Specifika noteringar för styling - Tablet

### Margin i textrutor

Texten bör alltid ligga en liten bit ifrån alla sidor på textrutorna så att det inte ser ut att vara och känns ihopträngt.

Med andra ord, samma margin på alla sidor.

### Navbar

Vår navbar är en ruta som sträcker sig över hela skärmen (100% skärmbredd), och ligger på toppen av sidan även i tablet versionen.

Denna ut på samma sätt som i Desktop.

### Recenssioner

- De ska vara animerade så att det "scrollas" igenom dem (Från höger till vänster)
- Endast en i taget ska visas på skärmen.
- Det ska finnas vita pilar för att bläddra genom recenssionerna

## Marginaler på sidan

### "Hem", "Luftballong", "Akrobatflyg" & "Boka" (Alla sidor har samma marginaler)

**Horizontala Marginaler:**

- 10px minst på höger och vänster sida av textrutorna
- 25px minimum mellan cards med information ang de olika flygningarna. De bör ligga nära nog att de ser ut att höra ihop, men det är okej att låta dem ligga lite längre isär på större skärmar.

**Vertikala Marginaler:**

- 25px mellan alla element på sidan

# 📱 Mobile

Bredden utgår från 320 px.

### H1

Over the Rainbow, 40px

### H2

Jura, 25px

### H3

Jura, 20px

### Paragraf/ brödtext

Inter, 16px

### Knapptext - "Acceptera" & "Avböj" i cookie bar, samt alla "Läs mer" & "boka" knappar

Inter, 16px

## Specifika noteringar för styling - Mobile

### Margin i textrutor

Texten bör alltid ligga en liten bit ifrån alla sidor på textrutorna så att det inte ser ut att vara och känns ihopträngt.

Med andra ord, samma margin på alla sidor.

### Navbar

Vår navbar är en ruta som sträcker sig över hela skärmen (100% skärmbredd), och ligger på botten av sidan i mobile versionen.

**storlek:**

- Bredd: 100%vw
- Höjd: 76px

**Basdesign:**

- Prussian Blue - #0A374F
- Ett streck på toppen med en tjocklek på 3px (ljusare ton än resten av knappen)
- Ett streck på botten med en tjocklek på 3px (ljusare ton än resten av knappen)

**Knappar:**

- Knappfärg: White - #FFFFFF
- Med Opacity 15%
- Placering:
  - Jämnt fördelade med 4px mellan varje knapp.
  - Knapparna ska sträcka sig hela vägen till sidorna av skärmen.
- När man är inne på en sida (T.ex "Luftballong") så ska knappbakgrunden på motsvarande ikon bli samma färg som basfärgen(#0A374F).
  _Se Figma för exempel. Sida: Prototype Mobile_

**Ikoner:**

- Coral - #F57E4B
- Storlek:
  - Höjd: 50px
  - Bredd: varierar beroende på ikon
- Alla ikoner har en "Drop shadow" effekt
- Finns att hitta i "components" i vår Figma fil

**Länktext:**

- H2
- Bör ha samma spacing mellan varje val samt på sidorna av dem.
- Bör alltid ha lika mycket plats ovanför och under i navbar rutan.

### Recenssioner

- **Hem:** Blandade recenssioner från både luftballong & akrobatflyg
- **Luftballong:** Endast recenssioner från turer med luftballong
- **Akrobatflyg:** Endast recenssioner från turer med Akrobatflyg
- **Bokning:** Inga recenssioner

### Footer

Sidan/"Företagets" namn samt dess slogan ska ligga centrerat. All information i footern ska vara "staplade" på varandra i följande ordning:

1. Logo & Slogan
2. Kontaktinformation
3. Sociala medier

**Storlek & typsnitt:**

- Logo: Over the Rainbow, 41px
- Slogan: Inter, 18px

Alla element bör ha lika mycket utrymme mellan varandra, samt en god marginal från sidorna.

## Marginaler på sidan

### "Hem", "Luftballong" & "Akrobatflyg" (dessa sidor har samma marginaler)

**Horizontala Marginaler:**

- 10px minst på höger och vänster sida av textrutorna

**Vertikala Marginaler:**

- 20px mellan alla element på sidan

### "Boka"

**Horizontala Marginaler:**

- 10px på höger och vänster sida av textrutorna

**Vertikala Marginaler:**

- 20px mellan "header" bilden och den första textrutan
- 25px mellan den första textrutan ("Bokning") och bokningsformuläret
- 25px mellan bokningsformuläret och textrutan "Vanliga Frågor"
- 20px mellan textrutan "Vanliga Frågor" och footer

## Authors

[Lenita Dahlin](https://github.com/LDMI-24)

[Malin Rosenquist](https://github.com/MalinRosenquist)

## Design

Designen på sidan, samt prototypen, skapades av:

[Lenita Dahlin](https://github.com/LDMI-24)

[Malin Rosenquist](https://github.com/MalinRosenquist)

Ikonerna för Flygplan och Luftballong skapades av:

[Lenita Dahlin](https://github.com/LDMI-24)
