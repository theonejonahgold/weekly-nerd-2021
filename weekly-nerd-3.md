# Weekly nerd 3

# Vraag: Welke onderwerpen die zijn behandeld tijdens de minor hebben de meeste indruk op je gemaakt, per vak?

## Web apps from scratch

Wat mij het meeste indruk heeft gemaakt is wat de tekortkomingen zijn van een SPA. Het omzeilt een paar Browser-technlogieën, zoals routing en SEO, en geeft er niets of een hacky oplossing voor terug. Hash routing sprint daar naar boven, wat misbruik maakt van navigeren naar elementen met een id om routing zonder van pagina te veranderen toe te staan.

## CSS to the recue

De ruwe kracht die CSS bezit, en hoeveel je ermee voor elkaar kan krijgen. Vooral op het gebied van 3D. Ik had altijd wel het idee dat je wat coole dingen kon doen met CSS in 3D, maar zo ver heb ik het nog nooit gepusht. Ik denk dat ik zeker het theoretische limiet van wat mogelijk is met CSS heb bereikt met mijn Rubik's Cube experimenten.

## Progressive web app

Caches, en de features die je eromheen kan bouwen. Ik heb voor mijn opdracht een HackerNews kloon gebouwd, wat een nieuwssite is waar je artikelen kan delen en reacties kan achterlaten. Ik heb met caches een bookmark-systeem gebouwd, die ook offline werkt.

## Browser technologies

Hoe makkelijk wij als developers het maken om de gebruiker te benadelen. Het kost veel moeite om een Kahoot kloon te bouwen die te gebruiken is zonder CSS en JavaScript, maar het resultaat is wel zeer bevredigend, en bruikbaar voor veel meer mensen.

## Real-time web

Dat real-time eigenlijk niet 100% real-time is. Er worden nog steeds requests verzonden en responses ontvangen, het gebeurt alleen over een verbinding die nooit afsluit, maar altijd open staat voor verkeer vanaf beide kanten van de lijn. De benaming is dus eigenlijk niet helemaal oprecht. Ook ervoor zorgen dat dataverkeer je "response buffer" niet overbelast, waardoor je applicatie volledig kan crashen.

## Human-centered design

Hoe je testen soms niet zo serieus moet aanpakken, en gewoon wat op moet gooien en kijken wat er blijft hangen. Testscenario's schrijven volgens het boekje en testpersonen deze door laten lopen maken je blind voor wat er daaromheen fout zou kunnen gaan. Je gebruikers lopen niet als een robot telkens dezelfde stappen door, en dat moet ook terug te vinden zijn in hoe je je tests opzet.

# Aantekeningen

## Introductie

**Dave**:

- Senior front-end
  - Interactive web paplications
  - Full-stack front-end
- Contactpersoon CMD X Mirabeau

**Alex**:

- Senior Designer & Art Director
  - Visual design, Branding, brand strategy, animation & 3D (een beetje)
- Zelf-aangeleerd motion designer tot 3D illustrator en beetje developer.
- Excited en bang voor de opkomende mix van de digitale en fysieke wereld.

Mirabeau:

- Full-service digital-design agency gefocust op HCD
- Interacteive applicaties en websites
- Image Recognition/AI
- MakerSpace: Garage met 3D printers en andere fysieke maakapparaten

## Topics

1. De kracht van T-shaped Front-end developers.
2. Het grootste probleem met SPA frameworks oplossen.

## De kracht van T-shaped Front-end developers

**Hoe zijn wij/CMD front-end developers van anderen?**: We zijn front-end experience developers.

### Het profiel

- Expertise in front-end development
  - T-shaped T-shaped front-end developer (accessibility, creative/visual, technical)
- Kennis in visual design
- Kennis in interaction design

### The interactive department

1. Front-end experience development guild
2. Visual design guild
3. Interaction design guild

Front-end developers zitten bij de designers, niet bij de andere soorten developers.

#### De impact op het design proces

De verschillende guilds werken gesilood samen. Wannneer samenwerking nodig is, komen ze samen om te overleggen. Voor de rest werken visual designers, interaction designers en front-end developers apart van de andere disciplines aan hun doelstellingen.

##### De stappen waarbij FXD samenwerkt met design

- Concepting
- Design production
- Design review
- Browser handoff
- Development review
- Documentatie

#### Tegenwoordig

De silo's zijn de laatste tijd steeds verder open gebroken, waardoor de verschillende gildes soepeler samen kunnen werken in een gestroomlijnd proces.

### From MiraBlog to Lely Used

MiraBlog geheel in de browser ontworpen, op basis van de geüpdate Mirabeau website. Door de samenwerking tussen FXD en VD kon zonder design tools de blog ontworpen worden op deze manier.

#### Lely Used project

- Lely Builds autonomous robots for farming.
- They want to own the second hand market through a new refurbishment platform.
- Just a couple of waves (aantal sprints van 1/2 weken) to realise an MVP.
- The project called for a high-paced an multidisciplinary approach.

Het uiteindelijke ontwerp was in de browser ontworpen samen met front-end developers om de oneindige hoeveelheid states en variaties niet te hoeven ontwerpen.

## Solving the biggest problem we had with SPA frameworks

Nadelen frameworks:

**Oplossing**: Progressive enhancement

### Progressive enhancement

- HTML
  - Accessibility
  - SEO
  - Stop reinventing the wheel
- CSS
  - Enhance UX with visual
  - Mobile first
- JS
  - Enhance UX with interaction
  - Always Vanilla, unless framework is necessary

### Tools used

Server-side rendered website/application: Sitecore

Client-side rendered website/application: React

React is not good enough. It costs too much

Next.js lost deze problemen op voor React.js:

- Geen SSR
- Trage initial page load (pagina en data wordt gecached)
- SEO
- Non-JS gebruikers die je app niet kunnen gebruiken

Dus CSR en SSR **samen**!

## Next.js stappen

1. Render pagina op de server (SSG of SSR)
2. "Hydrate" de pagina op de front-end  
   Vergelijkbaar met hoe React.js de DOM inlaadt, maar met een volle DOM (slim inladen)
3. Gebruik website als SPA met CSR na hydratatie

## Andere features

- SSR (serverless), SSG of mix van beide
- Automatische code splitting
- Integreerde (serverless) API
- Critical CSS (binnenkort, op de roadmap)
- Automatische image optimalisatie
- En veel meer!

## Takeaways

- Bouw altijd progressively enhanced
- SPA frameworks gebruiken is niet verkeerd, zolang je SSR/SSG kan toepassen
  - Gebruik wanneer het logisch is
  - Onderzoek hoe je dan alsnog alle PA lagen kan ondersteunen
  - Leer de basis voordat je het gaat weg-abstraheren.
- Onderscheid de hype van de bewezen en wel-ondersteunde frameworks.
