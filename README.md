I detta repository har jag skapat en webbplats som kommunicerar med en enkel REST API med Express.

Webbplatsen använder html, css och javascript. Anropen till apiet sker med Fetch api

Information om APIet:
Jag har använt Sqlite3 som databas. 
Funktionalitet för CRUD finns

Länk till webbsida
https://studenter.miun.se/~mifr2204/writeable/azure_backend-mom2-sida/add.html

länk till app
https://backendm2.azurewebsites.net/

länk till git webbtjänst
https://github.com/mifr2204/backend-mom2-webbtj.git

länk till git webbsida
https://github.com/mifr2204/backend-mom2-sida.git

Installation, databas
Sqlite3 används som databas av APIet. Klona ner källkodsfilerna, kör kommandot: npm install 
Andvänd kommandot: npm run install för att installera Installations-skriptet skapar följande databastabeller:

Tabell   	Fält
workplaces	id (INTEGER), companyname (TEXT), location (TEXT), startdate(DATE), enddate (DATE), title (TEXT), description (TEXT), timestamp (TIMESTAMP)

Användning
Hur man nå APIet:

Metod	Ändpunkt	    Beskrivning
GET	    /workplaces	    Hämtar alla tillgängliga arbetsplatser.
POST	/workplaces	    Lagrar en ny arbetsplats.
PUT	    /workplaces/:ID	Uppdaterar en arbetsplats. 
DELETE	/workplaces/:ID	Raderar en arbetsplats.


Ett arbetsplats-objekt returneras/skickas som JSON med följande struktur:

{
   "companyname": "Frösunda",
   "location": "Nässjö",
   "startdate": "2010-01-01",
   "enddate": "2016-02-01",
   "title": "Personlig assistent/teamleader",
   "description": "Vara hos olika kunder och hjälpa dom i vardagen, planera schema med mera"
}