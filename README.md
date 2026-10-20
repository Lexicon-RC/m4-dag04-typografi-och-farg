# Dag 4 · Typografi och färg i kod

*Modul 4, UI/UX & Frontendutveckling, Lexicon IT-Proffs*

## Vad du ska göra idag

Du översätter en typskala och en färgpalett till CSS, med kontrast som håller och tydliga tillstånd (hover och fokus).

## Bakgrund

Typografi och färg är det som mest direkt ger en sida karaktär, och det som oftast går fel i tillgängligheten. Idag arbetar du efter specifikationen i `design.md` (samma sorts dokument som en designöverlämning från Figma).

## Så arbetar du (samma som alltid)

1. **Forka** dagens repo på GitHub (*Fork → Create fork*).
2. **Klona din fork:** *Code → HTTPS → kopiera adressen*. I terminalen (Ctrl+ö i VS Code): `git clone <adressen>`. Öppna den nya mappen i VS Code och starta *Live Server*.
3. **Gör uppgiften.** Spara och kontrollera i webbläsaren efter varje steg. Gör en commit efter varje avslutat steg: `git add .` och `git commit -m "Beskriv vad du gjorde"`.
4. **Skicka upp** när du är klar: `git push`.
5. **Lämna in i Microsoft Forms.**

Fastnar du: skriv ner exakt var och vad du försökt, och ta det först i nästa handledda pass.

## Uppgiften steg för steg

### Steg 1. Läs design.md

Där står typsnitt, storlekar, radavstånd och färgkoder. Du ska följa dem exakt, inte "ungefär".

### Steg 2. Ställ in grundtypografin

På `body`: `font-family`, `font-size: 1rem`, `line-height: 1.6`. Förklara i en kommentar varför `rem` är bättre än `px` för textstorlek.

### Steg 3. Rubrikskalan

Sätt `font-family` (Georgia) och `font-size` för `h1`, `h2`, `h3` enligt skalan. Rubriker har kortare radavstånd (1.2) än brödtext.

### Steg 4. Färger på text och länkar

Sätt textfärg, rubrikfärg och priset i kaféets röda. Länkar får en egen färg och en tydlig `:hover`.

### Steg 5. Kontrollera kontrasten

Öppna kontrastkontrollen från modul 3. Testa brödtext mot bakgrund, vit text mot den röda knappen och länkfärg mot bakgrunden. Skriv resultaten som kommentarer i CSS. Kravet är minst 4,5:1 för vanlig text.

### Steg 6. Fokusmarkering

Lägg till en tydlig `:focus-visible`-stil för länkar, knappar och formulärfält. Tabba genom sidan och kontrollera att du alltid ser var du är. Ta aldrig bort `outline` utan att ersätta den.

### Steg 7. Styla hero och formulär

Hero-sektionen får bakgrund, `padding` och större text. Formulärfälten får `padding`, kantlinje och `font: inherit`. Etiketterna blir fetstilta.

## Kontrollista: så vet du att du är klar

- [ ] Typsnitt, storlekar och radavstånd matchar `design.md`.
- [ ] All brödtext och alla knappar klarar kontrastkravet 4,5:1, och du har dokumenterat det.
- [ ] Länkar och knappar har hover-läge.
- [ ] Det finns en tydlig fokusmarkering, och du har testat med Tab.
- [ ] Formuläret är läsbart och fälten är lätta att träffa.
- [ ] Du har pushat till din fork och skickat in länken.

## Tips om du fastnar

- Texten ser för liten ut? Du har kanske satt `font-size` på fel element. Kolla i DevTools.
- Kontrasten blir för låg? Mörka färgen lite, inte hela designen.
- Georgia syns inte? Kontrollera stavningen på `font-family` och att du har en reservlista.

## Inlämning

**Deadline: imorgon klockan 09.00.** Allt lämnas in i Microsoft Forms. Du behöver inte redovisa något muntligt.

I formuläret fyller du i:

1. Länk till din fork av det här repot.
2. Reflektion: Vilket kontrastvärde överraskade dig mest, och vad ändrade du för att klara kravet?

## Vill du mer? (frivilligt)

- Skapa en `.sr-only`-klass som döljer text visuellt men inte för skärmläsare.
- Testa sidan i mörkt läge med `@media (prefers-color-scheme: dark)`.
