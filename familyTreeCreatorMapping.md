This file shows the mapping between **Mindscape Family Tree Creator Deluxe** and the Gedcom files exported from the same program.

Color Legend
- ![direct](https://placehold.it/10/00ff00?text=+) - mapped directly
- ![multiple](https://placehold.it/10/ccff11?text=+) - split across multiple Gedcom fields
- ![derived](https://placehold.it/10/ccff11?text=+) - derived from other Gedcom fields and linked references
- ![generic](https://placehold.it/10/ffff00?text=+) - part of more generic Gedcom field
- ![partial](https://placehold.it/10/ffaa00?text=+) - mapped partially
- ![unmapped](https://placehold.it/10/ff0000?text=+) - unmapped
- ![unknown](https://placehold.it/10/00ffff?text=+) - unknown

### Individual

- Name --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > NAME*
- Date of Birth --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > BIRT > DATE*
- Place of Birth --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > BIRT > PLAC*
- Sex --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > SEX*
- Date of Death --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > DEAT > DATE*
- Place of Death --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > DEAT > PLAC*
- Also Known As --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > NAME > NICK*
- Occupation --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > OCCU*
- Title --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > TITL*
- Reference Number --> *![direct](https://placehold.it/10/00ff00?text=+) INDI*
- Spouses[] : **Spouse** --> *![derived](https://placehold.it/10/ccff11?text=+) - FAMS (FAM) > HUSB|WIFE*
- Children[] : **Child**
  - multiple:
  - --> *![derived](https://placehold.it/10/ccff11?text=+) - FAMS (FAM) > CHIL*
  - --> *![derived](https://placehold.it/10/ccff11?text=+) - INDI > ASSO*
- Events[] : **Event**
- Medical --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Height --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Weight --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Eyes --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Hair --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Blood Type --> *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Cause of Death *![generic](https://placehold.it/10/ffff00?text=+) - INDI > DSCR*
  - Age --> *![direct](https://placehold.it/10/00ff00?text=+) - calculated, not needed*
  - Additional Medical Information --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > DSCR > NOTE*
  - Sources[] : **Source**
- Address
  - Street & Number --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > ADDR*
  - City/Town --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > CITY*
  - County/Region --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > ADDR2*
  - State/Province --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > STAE*
  - Country --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > CTRY*
  - Zip/Postal Code --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > POST*
  - Phone --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > PHON*
  - E-mail --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > EVEN > _EMAIL*
  - Details
  - Sources[] : **Source**
- Album
  - ...
- Notes --> *![direct](https://placehold.it/10/00ff00?text=+) - INDI > NOTE*
- (Siblings[]) --> *![derived](https://placehold.it/10/ccff11?text=+) - FAMC (FAM) > CHIL*
- (Mother) --> *![derived](https://placehold.it/10/ccff11?text=+) - FAMC (FAM) > CHIL*
- (Father) --> *![derived](https://placehold.it/10/ccff11?text=+) - FAMC (FAM) > CHIL*

### Spouse

- Name of Spouse
- Start
  - Status
  - Date
  - Place
  - Details
  - Sources[] : **Source**
- End
  - Status
  - Date
  - Place
  - Details
  - Sources[] : **Source**

### Child

- Name
- Sex
- Status of Father
- Other Parent

### Source

- Source --> *![direct](https://placehold.it/10/00ff00?text=+) - SOUR > TITLE*
- Reliability --> *![derived](https://placehold.it/10/ccff11?text=+) - [object > SOUR > QUAY](http://homepages.rootsweb.ancestry.com/~pmcbride/gedcom/55gcch2.htm#SOURCE_CITATION)*
- Type --> *![direct](https://placehold.it/10/00ff00?text=+) - SOUR > REFN > TYPE*
- Details --> *![derived](https://placehold.it/10/ccff11?text=+) - object > SOUR > NOTE*
- (Source Info) --> *![generic](https://placehold.it/10/ffff00?text=+) - SOUR > TEXT*

### Event

- Event
- Date of Event
- Place of Event
- Details
- Sources[] : **Source**
