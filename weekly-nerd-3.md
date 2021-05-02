# Weekly nerd 3

# Vraag: Welke onderwerpen die zijn behandeld tijdens de minor hebben de meeste indruk op je gemaakt, per vak?

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
