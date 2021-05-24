# Weekly nerd 2

# Vraag: De tech-industrie bestaat voor een groot deel uit dezelfde type personen en testen vervolgens hun websites bij weer dezelfde types, met stereotypering, vooroordelen en biased uitkomsten tot gevolg. Herken je dit als probleem? Moet dit veranderen? In wat voor team zie jij jezelf graag werken?

Ik herken dit zeker als probleem. Je ziet bij veel bedrijven in het CMD vakgebied dat er nog een best groot onderscheid is tussen de rollen die mannen veelal op zich nemen en de rollen die vrouwen veelal op zich nemen. We lopen wel wat vooruit als je kijkt naar onze zuidelijke continentgenoten, maar dat neemt niet weg dat er nog genoeg te doen is. Wat ik persoonlijk ook nog best veel zie is dat mensen met een etnische of allochtone achtergrond ook wel wat meer gerepresenteerd worden, maar dat kan ook schijn zijn. Misschien kijk ik wel naar de verkeerde bedrijven en neem ik daarom deze aanname.

Bij de bedrijven die ik veelal langs zie komen zie ik graag dat ze het gebrek aan diversiteit harder aanpakken. Het is lastig om je aannames in kwestie te stellen, maar je bouwt er wel betere producten mee. Vooral als het producten zijn die een zo'n breed mogelijk publiek moeten bereiken. Ik test graag mijn aannames, en ik zou dit graag willen doen in een divers team die dit fasiliteert en hier grote stappen in maakt.

# Aantekeningen

## Mammut case: Build in amsterdam

Webshop voor meest extreme collectie.

Conversie wordt gedreven door emotie, dus iemand emotioneel meenemen in een verhaal verkoopt.

### Stap 1: Strategie

We willen dat de gebruiker onderdeel werd van de expeditie, en daarbij geïnformeerd worden over de gebruikte producten.

### Stap 2: Wireframes

### Stap 3: Ontwerp

### Challenges

- 6 weken voor 4 pagina's.
- Terugbrengen van design om project haalbaar te maken.

### De stack

- Next.js framework + SSG
- Contentful CMS
- Vercel voor hosting

### Animaties: Key principles

**1. Gebruik transform of opacity**

Stappen die browser doorloopt voor animaties:
1. JavaScript verandert CSS van een element.
2. Styling wordt opnieuw berekend.
3. Layout berekend.
4. Pixels worden ingevuld; paint.
5. Compositie van de verschillende lagen.

**2. Vermijd layout-trashing**

Treedt op wanneer JS herhaaldelijk schrijft, en dan leest, van de DOM, wat een document reflow veroorzaakt. Dit voorkom je door styling apart op te halen en apart te setten.

Vraag waardes alleen bij eerste render en bij window resizes

**3. Animeer in rAFloop**

`window.requestAnimationFrame()`

Voordelen:
- een enkele reflow- en repaint- cyclus
- Animatie-veranderingen zijn te bundelen in 1 callback die alle geregistreerde callbacks afhandeld

**4. Stop alles buiten view**

Intersection Observer API: Neemt asynchroon veranderingen waar, en geeft een melding wanneer een element in beeld is.

- Lazy loaden van media
- Pauzeren van video's
- Pauzeren van animaties
- Verberg fixed elementen met `visibility: hidden`

### Wat er gebeurd als je dit niet toepast

Constante layout thrashing met een hoge performance impact.

## Triple: Ajax & NLZIET

### Kern van Triple

- Technology Operations
- Concept & Creation
- Development

### Webteam

- Next.js + TypeScript
- Sass
- Contentful CMS
- Standardisatie van projectstructuur
- Boilerplates
- Code cannon
- Chromecast 

### Hoe los je een complexe situatie op die je nog niet eerder bent tegengekomen?

#### Methode 1 RTFM

- Documentatie lezen.
- Error messages zoeken in de repository van de library
- Niet gelijk naar stackoverflow antwoorden zoeken

#### Methode 2: Code aan/uitzetten

1. Alle code uitcommenten
2. Stap voor stap code aanzetten totdat oorsprong van bug duidelijk is

#### Methode 3: Devtools

- Netwerk tab om te kijken of falende netwerk requests aan front-end of back-end liggen
- Georganiseerde console log: `console.log('debug:::var',var)`

#### Methode 4: Artikelen lezen

- Kan helpen met het oplossen van problemen
- Sowieso handig voor het uitbreiden van je kennis

#### Methode 5: Stackoverflow

- Goed letten op bronvermelding
- Letten op juiste antwoorden

#### Methode 6: Collega vragen

Soms zie je door de bomen het bos niet meer

#### Methode 7: Dagje pauze nemen

Frisse blik doet wonderen, vooral als je je dag niet hebt.
