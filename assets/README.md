# assets/

Sem odloži svoje slike (in po potrebi video datoteke) za spletno stran.

- `assets/images/` — fotografije (hero ozadje, tvoja fotka pri "Your Guide", slike za galerijo …)
- `assets/videos/` — video datoteke, če jih ne linkaš samo na YouTube

## Kako poteka

1. Datoteke naloži v ustrezno mapo — preko GitHuba (Add file → Upload files na branchu
   `claude/norway-trip-webpage-hr4rym`, v mapo `assets/images` ali `assets/videos`) ali
   pošlji datoteke meni v pogovoru.
2. Sporoči mi, katera slika gre kam (npr. "hero.jpg = ozadje na vrhu", "guide.jpg = moja fotka",
   "gallery-1.jpg … gallery-8.jpg = galerija").
3. Jaz posodobim `index.html`, da namesto trenutnih CSS/SVG placeholderjev uporabi te slike,
   ter spremembe commitam in pusham.

## Priporočila za slike

- Format: `.jpg`/`.webp` za fotografije (manjša velikost datotek), `.png` samo če potrebuješ prosojnost.
- Hero ozadje: širok format (vsaj 1920×1080), ne pretemno, ker čez njega leži besedilo.
- Fotka vodiča: pokončni format (npr. 4:5), obraz naj bo dobro viden.
- Galerija: kvadratni format (1:1) je najbolj berljiv v trenutni postavitvi.
