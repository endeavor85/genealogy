This file shows the mapping between **Mindscape Family Tree Creator Deluxe** and the Gedcom files exported from the same program.

Color Legend
- ![direct](https://placehold.it/10/00ff00?text=+) mapped directly
- ![multiple](https://placehold.it/10/ccff11?text=+) split across multiple Gedcom fields
- ![derived](https://placehold.it/10/ccff11?text=+) derived from other Gedcom fields and linked references
- ![generic](https://placehold.it/10/ffff00?text=+) part of more generic Gedcom field
- ![partial](https://placehold.it/10/ffaa00?text=+) mapped partially
- ![unmapped](https://placehold.it/10/ff0000?text=+) unmapped
- ![unknown](https://placehold.it/10/00ffff?text=+) unknown

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
- Spouses[] : **Spouse** --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > HUSB|WIFE : @INDI*
- Children[] : **Child**
  - multiple:
    - --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > CHIL*
    - --> *![derived](https://placehold.it/10/ccff11?text=+) INDI > ASSO*
- Events[] : **Event** --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN*
- Medical --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Height --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Weight --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Eyes --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Hair --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Blood Type --> *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Cause of Death *![generic](https://placehold.it/10/ffff00?text=+) INDI > DSCR*
  - Age --> *![direct](https://placehold.it/10/00ff00?text=+) calculated, not needed*
  - Additional Medical Information --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > DSCR > NOTE*
  - Sources[] : **Source** --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > DSCR > SOUR*
- Address - *INDI > EVEN (TYPE="Current Address")*
  - Street & Number --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR*
  - City/Town --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR > CITY*
  - County/Region --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR > ADR2*
  - State/Province --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR > STAE*
  - Country --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR > CTRY*
  - Zip/Postal Code --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > ADDR > POST*
  - Phone --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > PHON*
  - E-mail --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > _EMAIL*
  - Details --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > NOTE*
  - Sources[] : **Source** --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > EVEN > SOUR*
- Album - *![unmapped](https://placehold.it/10/ff0000?text=+) not using, don't care*
- Notes --> *![direct](https://placehold.it/10/00ff00?text=+) INDI > NOTE*
- (Siblings[]) --> *![derived](https://placehold.it/10/ccff11?text=+) FAMC (FAM) > CHIL*
- (Mother) --> *![derived](https://placehold.it/10/ccff11?text=+) FAMC : @FAM > CHIL*
- (Father) --> *![derived](https://placehold.it/10/ccff11?text=+) FAMC : @FAM > CHIL*

### Spouse

- Name of Spouse --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > HUSB|WIFE : @INDI > NAME*
- Start --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > MARR*
  - Status --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > (type)*
  - Date --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > MARR > DATE*
  - Place --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > MARR > PLAC*
  - Details --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > MARR > NOTE*
  - Sources[] : **Source** --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > MARR > SOUR*
- End --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > DIV,others?*
  - Status --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > (type)*
  - Date --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > DIV > DATE*
  - Place --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > DIV > PLAC*
  - Details --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > DIV > NOTE*
  - Sources[] : **Source** --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > DIV > SOUR*

### Child

- Name --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > CHIL : @INDI > NAME*
- Sex --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > CHIL : @INDI > SEX*
- Status of Father|Mother --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > CHIL : @INDI > ASSO > RELA*
- Other Parent --> *![derived](https://placehold.it/10/ccff11?text=+) FAMS : @FAM > HUSB|WIFE : @INDI*

### Source

- Source --> *![direct](https://placehold.it/10/00ff00?text=+) SOUR > TITLE*
- Reliability --> *![derived](https://placehold.it/10/ccff11?text=+) [object > SOUR > QUAY](http://homepages.rootsweb.ancestry.com/~pmcbride/gedcom/55gcch2.htm#SOURCE_CITATION)*
- Type --> *![direct](https://placehold.it/10/00ff00?text=+) SOUR > REFN > TYPE*
- Details --> *![derived](https://placehold.it/10/ccff11?text=+) object > SOUR > NOTE*
- (Source Info) --> *![generic](https://placehold.it/10/ffff00?text=+) SOUR > TEXT*

### Event

- Event --> *![direct](https://placehold.it/10/00ff00?text=+) object > EVEN > TYPE*
- Date of Event --> *![direct](https://placehold.it/10/00ff00?text=+) object > EVEN > DATE*
- Place of Event --> *![direct](https://placehold.it/10/00ff00?text=+) object > EVEN > PLAC*
- Details --> *![direct](https://placehold.it/10/00ff00?text=+) object > EVEN > NOTE*
- Sources[] : **Source** --> *![derived](https://placehold.it/10/ccff11?text=+) object > EVEN > SOUR*
