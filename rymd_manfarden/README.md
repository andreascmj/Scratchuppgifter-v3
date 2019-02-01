# Månfärden

Nu är det dags för uppskjutning till månen! Tur att vi har förberett oss genom att sätta ut saker i rymden i vårt koordinatsystem. Det kommer vi få användning av här.

Vi ska bygga en avfyrning där vi skriver in vilka koordinater vi vill åka till och sedan så åker vi dit.

![](./0_1.gif)

##  1 – Lägg ut planeter, asteroider och satelliter

Vi ska börja med att lägga ut alla våra sprajtar så att de får rätt koordinater.

Tryck på en sprajt i biblioteket för att välja den. Vi kan se att den är vald för att den får en blå ram runt sig.

Vi ska sätta ut våra sprajtar så exakt vi bara kan. För att göra det så kan vi programmera dem genom att använda blocken **När grön flagga klickas på** och **gå till x: ` ` y: ` `**.

![](./1_1.png)

Skriv in de exakta koordinaterna från ditt koordinatsystem på papper. Hamnar alla sprajtar där du trodde att de skulle hamna? Är det någon som inte stämmer?

## 2 – Använda frågor och svar

Välj sprajten ”Raket”.

Vi kan berätta för vår raket vart den ska åka genom att använda blocket **fråga `     ` och vänta**. Då öppnas en textruta där vi kan skriva in exempelvis en x-koordinat. Det vi svarar hamnar sedan i variabeln **svar**.

Koda raketen så att den frågar vilken x-koordinat den ska gå till och att den sedan sätter x till svaret.

![](./2_1.png)

## 3 – Fråga efter y-koordinat

Fortsätt koda på sprajten ”raket”. 

För att kunna åka till månen behöver vi veta både en x-koordinat och en y-koordinat.

Så vi behöver en fråga till. Men denna gång frågar vi ”Vilken y-koordinat ska vi gå till?”. Lägg frågan under vårt block där vi går till x.

![](./3_1.png) 

Frågar vår raket nu först vilken x-koordinat den ska gå till? Och sedan vilken y-koordinat den ska gå till?

## 4 – Spara x och y i variabler

I stället för att hoppa till x- och y-koordinaten så skulle vi vilja använda blocket **glid 1 sek till x: ` ` y: ` `**. Då kommer vår raket att glida till koordinaten i stället för att hoppa. Det kommer se roligare ut.

Men för att kunna glida så behöver vi veta både x och y. Och variabeln **svar** vet bara svaret på den senaste frågan. Den håller inte reda på tidigare svar. Det betyder att vi inte vet vilken x-koordinat vi ska åka till efter att vi har svarat på frågan om y-koordinat.

Vad vi kan göra är att spara svaret i en egen variabel. Som vi själva kan hålla reda på.

Skapa en ny variabel som heter ”ny x”. 

Använd blocket **sätt ”ny x” till `svar`** i stället för att använda blocket ”sätt x till `svar`”. Då sparar vi svaret på frågan i vår variabel ”ny x”.

Gör samma sak med y. Skapa en ny variabel som heter ”ny y” och sätt den till ”svar”.

![](./4_2.gif)

Nu kommer vår raket inte att flytta på sig längre för vi har tagit bort blocken som flyttar den. Men kan du se att värdena för variablerna ändras när du skriver in svar på frågan?

## 5 – Glid till variabler

Ser din kod för raketen ut ungefär så här?

![](./5_1.png)

Nu ska vi använda blocket **`4` sek till x: ` ` y: ` `**. 

![](./5_2.png)

När du har satt ihop de här blocken med de andra så kommer vår raket glida till koordinaten vi skriver in.

![](./5_3.gif)

## 6 – Berätta hur det har gått

Efter att vår raket har glidit så vill vi att den säger ”Jippie! En perfekt uppskjutning” om den rör vid månen. Och annars så vill vi att den säger ”Ajdå. Inte så bra som vi hoppades”.

Det gör vi med blocket **om `    ` då**:

![](./6_2.png)

Om vi rör vid månen då ska vi säga ”Jippie! En perfekt uppskjutning!”:

![](./6_3.png)

Annars så ska vi säga ”Ajdå. Inte så bra som vi hoppades.”.

![](./6_4.png)

![](./6_5.gif)

## 7 – Slumpmässig position

Nu ska vi ändra så att månen får en *slumpmässig* position i den högra och övre delen av scenen. Det ska vi göra med blocket **slumptal**. 

![](./7_2.png)

Anledningen är att vi vill att månen skall byta plats varje gång vi spelar så att vi inte bara kan komma ihåg vilken koordinat den har. 

Blocket **slumptal** fungerar lite som en tärning. Precis som att vi får olika svar när vi slår en tärning så får vi olika tal varje gång vi trycker på den gröna flaggan.

Till skillnad från en vanlig tärning (där det minsta talet vi kan slå är 1 och det högsta är 6) så kan vi i scratch välja vad det minsta- och högsta talet ska vara.

Markera sprajten ”Månen” och ersätt x-koordinaten med **slumptal**.

![](./7_4.gif)

Om vi vill att vår måne ska hamna på högersidan av vår scen – **vilken är den lägsta x-koordinaten som månen kan få?**

**Och vilken är den högsta x-koordinaten som månen kan få?**

Skriv in den lägsta i det vänstra fältet och den högsta i det högra fältet.

Hamnar månen på olika positioner nu varje gång du trycker på den gröna flaggan?

## 8 – Slumpmässig y-koordinat

På samma vis som vi slumpade fram en x-koordinat så ska vi nu slumpa fram en y-koordinat. Det är för att månen också ska kunna röra sig upp och ned.

Om vi vill att vår måne ska hamna på den övre delen av vår scen – **vilken är den lägsta y-koordinaten som månen kan få?**

**Och vilken är den högsta y-koordinaten som månen kan få?**.

Lägg till ett fält för slumptal även på y-koordinaten. Skriv in den lägsta i det vänstra fältet och den högsta i det högra fältet.

Hamnar vår måne på olika positioner även i höjdled varje gång du trycker på den gröna flaggan?

## 9 – 

