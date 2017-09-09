This file shows the mapping between **Mindscape Family Tree Creator Deluxe** and the Gedcom files exported from the same program.

Color Legend
- ![direct](https://placehold.it/10/00ff00?text=+) - mapped directly
- ![multiple](https://placehold.it/10/ccff11?text=+) - split across multiple Gedcom fields
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
- Spouses[] : **Spouse**
- Children[] : **Child**
- Events[] : **Event**
- Medical --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Height --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Weight --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Eyes --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Hair --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Blood Type --> *![unknown](https://placehold.it/10/00ffff?text=+) - unknown*
  - Cause of Death *![unknown](https://placehold.it/10/00ffff?text=+) - unknown*
  - Age --> *![direct](https://placehold.it/10/00ff00?text=+) - calculated, not needed*
  - Additional Medical Information --> *![unmapped](https://placehold.it/10/ff0000?text=+) unmapped*
  - Sources[] : **Source**
- Address
  - Street & Number
  - City/Town
  - County/Region
  - State/Province
  - Country
  - Zip/Postal Code
  - Phone
  - E-mail
  - Details
  - Sources[] : **Source**
- Album
  - ...
- Notes --> *![multiple](https://placehold.it/10/ccff11?text=+) INDI > NOTE [ > CONC,CONT]*
- (Siblings[])
- (Mother)
- (Father)

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

- Source
- Reliability
- Details

### Event

- Event
- Date of Event
- Place of Event
- Details
- Sources[] : **Source**
