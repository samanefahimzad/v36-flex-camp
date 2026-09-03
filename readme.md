.kort-rad är hyllan och mina fyra .kort är böckerna.

.kort-rad är föräldern till alla mina kort. Därför sätter jag display: flex på .kort-rad och inte på .kort.

.kort-rad {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

display: flex gör att korten ligger bredvid varandra. Mina .kort blir flex-items eftersom de ligger inuti .kort-rad.

Jag behöver inte använda manuella procentbredder som width: 25%.

gap: 1rem ger mellanrum mellan korten.

flex-wrap: wrap gör att korten kan gå ner på nästa rad om skärmen är liten.

Jag använder Flexbox eftersom jag vill ordna korten i en riktning.

Grid passar bättre när man vill ordna saker i både rader och kolumner. Därför behövs Grid inte i min kod.
Flexbox passar bra för mina aktivitetskort eftersom jag vill lägga korten bredvid varandra. I min kod använder jag .kort-rad { display: flex; }, vilket gör att mina fyra .kort blir flex-items och hamnar bredvid varandra. gap: 1rem ger mellanrum och flex-wrap: wrap gör att korten kan gå ner på nästa rad på en liten skärm.

Grid används för att ordna saker i rader och kolumner. Jag använde inte Grid eftersom jag bara behövde ordna korten i en riktning.
FEEDBACK: display: flex sitter som inline style , flytta till en class på containern i CSS-filen.
FEEDBACK: display: flex på ett enskilt .card 
flex hör hemma på hyllan, inte på varje bok.
FEEDBACK: Korten är gjorda med div och avståndet skapas med margin. använd article för korten och gap på föräldern för mellanrummet.


