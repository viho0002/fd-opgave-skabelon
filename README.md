# Opgaveskabelon til Frontend Design tema på Frontend-valgfaget

Se opgavebeskrivelsen på Fronter.

## Medfølgende API

Der medfølger en simpel API, som du kan bruge til at hente data til din opgave. Det er ikke et krav til opgaven, men det kan gøre det nemmere og hurtigere at få tekst og billeder ind i dit projekt.

Dokumentationen til API'et finder du på: [https://frontend-design-theme.netlify.app/](https://frontend-design-theme.netlify.app/).

Her er et eksempel på, hvordan du kan hente data fra API'et:

```astro
const employeesData = await fetch(
  "https://frontend-design-theme.netlify.app/api/employees"
).then((response) => response.json());

console.log(employeesData);
```

# Reflection

## Udfordringer

### Overblik

Den største udfordring i starten var at få et overblik, der var en del sider og jeg lavede fejlen ved at bare begynde at kode med det samme før jeg virkelig forstod hvad der var på siden. Jeg valgte at kigge på de få farver og text størelser før jeg hurgtigt smed dem ind i global.css og startede med på siden. Jeg tror det ville havde været meget bedre at tjekke gennem alle sider og notere hvor mange farver og font størelser der faktisk blev brugt så jeg ikke senere skulde ind i og lave flere størelser og farver samt ændre kode jeg allerede havde skrevet.

Jeg tror også at have et godt overblik ville have gjort det bedre at finde ud af hvad der skulde laves til componenter og hvad der nok bare skulde være noget der skulde bruges 1 gang

### Componenter

Hvad skal være et component? det var et spørgsmål jeg stillede mig selv gennem hele opgaven fordi jeg virkelig ikke kunne tage et valg, med nogle ting. Nogle ting opdagede jeg også meget sent og derfor viste ikke om jeg havde tid til at gå tilbage for at ændre vær gang til et component. en af de ting jeg er mest sur over jeg ikke gjorde componenter er headeren på de fleste containerer der har en roundtext titel og random text.

Senere læerte jeg at det nok er klogt at gøre noget til et component hvis det bliver brugt mere en 2 gange så kan man ligeså godt gøre det for at spare kode

### Card/Container

Meget af det her går tilbage til overblik og gennemlæsning af siden, jeg kunne godt mærke at i slutningen det var svært at finde ud af hvad der skulde være hvad, fordi jeg ikke havde det samme opsætning på alle containerne.

### Navngivning

navngivningen går som mange af de andre udfordinger tilbage til starten, fordi når jeg kom til en ting og navngav det så ente jeg med at skulde komme op med noget på det tidspunkt som ente med at gå galt

## Successerne

Bruge astro props til at lave gode dynamiske components

### Props

Det var super fedt at bruge props rigtigt for den første gang, jeg vil sige det jeg lavede som jeg var mest glad for var mine knapper og value siden, de kunne godt stadig havde været mere idyptende med måske nogle størelses queries men jeg syntes de var fede og var en af de ting jeg fik lavet meget tidligt.

Når man har props gør det det meget lettere at gå videre til de næste sider da du har noget af opsættningen allerede så hver gang jeg skulde have en knap var det allerede skrevet jeg skulde bare fylde hvad der skulde ind og så var den der.

Hvis jeg havde lavet flere mere dynamiske components med props kunne jeg nok have haft "færdigjort" siden hurtigere.

## Fremhævspecifikke kode dele der laver forskellige teknikker

knap kode for at snakke om astro props og alt de kan for at gøre siden bedre

side med meget text for at snakke om hvordan man kan lave gode maps af data

## Organisation på css

Jeg prøvede til startede med at fylde alt jeg tænkte vil gennemkomme på flere sider ind på global cssen.

Jeg prøvede at holde meget af koden inden på vert component, i starten for at give mig selv et bedre overblik over hvad der rammer hvad

Når jeg bruger data startede jeg med at tage det fra det første
hvor data bliver lagt
Globalt når det er noget der kommer med på mere
