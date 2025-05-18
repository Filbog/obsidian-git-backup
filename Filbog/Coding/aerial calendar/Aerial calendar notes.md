25-10-2024

### inspo
 - FEDEC site Fedec.eu/en/agenda/

### edge cases
 - in a year view, what if there are events spanning two diff months? Just show them on both months. For example, if the event is 30th Oct - 2nd Nov: it’ll be 
    - November: 
    - 30-2nd Nov - Event Title
    - October:
    - 30 Nov-2 - Event Title
 - that way it’ll be clean, and even if event is for 3 months, it’ll be readable.


### models and fields
##### event
 - beginning day
 - end day
 - location (particular city/virtual)
 - type
 - aerials/other circus arts
 - Main link
 - additional external links for the event - like website, FB page, code of points
 - author - but I'm thinking about edge cases. What if someone changes a company or studio? Then we have to change his alias, but leave the old one on the already-created events
 - title

### filters
 - location - by city. My idea for now: find an existing list of Polish cities and somehow implement it in the app for an autocomplete. So that there isn't Poznan, poznań etc. Or if I don't want to do this challenge, I can just let users type shit in.
 - festival/competition/convention/retreat/workshops/other
 - aerials/other circus arts
### verification of organizers
 - how to tackle it? Taking into consideration both admin's comfort, and UX
 - Idea of how it should function: users can register and ask for verification. They can add events anyway, and those events show up when the organizer gets verified. When they get verified thru some social methods, we add them thru django admin to the "organizer" group or sth.
 - Albo moze: jak ktos jest verified to moze dodawac eventy od razu. Jak nie, to moze dodawac wydarzenia do jakiejs „poczekalnil” czy czegos takiego

### views

### functionality
 - report the event - sth changed? no longer happening? violates our policy? Mb max 3 per day so that they can't spam.
 - Banning users :D
 - add to calendar
 - na pewno dodaj jakis disclaimer ze to jest passion project i ze maja sie 3 razy upewniac co do dat, etc U ORGANIZATORA
 - footer xd
 - Disclaimer na dole
 - FAQ:
	 - jak dodac event
	 - nie widac mojego eventu
	 - mam pomysl na usprawnienie, gdzie napisac
	 - jak zostac przyklepanym do dodawania eventow
- zasady - ale czy ta strone dodam to nwm
	- tylko wydarzenia, ktore są jakkolwiek związane ze swiatem aerial
	- znowu disclaimer - ze jako pkt odniesienia; kontaktowac sie z organizatorem


### postgres db data for dev testing on fly.io
Username:    postgres
  Password:    Xl1RMR6ltb2gvCf
  Hostname:    kalendarium-aerial-db.internal
  Flycast:     fdaa:2:c180:0:1::19
  Proxy port:  5432
  Postgres port:  5433
  Connection string: postgres://postgres:Xl1RMR6ltb2gvCf@kalendarium-aerial-db.flycast:5432
## Hashtags:


### References (source material, similar notes):
