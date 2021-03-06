# ORC club certificate scoring

Van http://orc.org/index.asp?id=44 zijn lijsten te downloaden met daarin gegevens over de zeilboten met een geldig ORC-certificaat.

Omdat de VPP ook wel zinnig is voor anderen, heb ik dit tooltje gemaakt.





## Columns in `.rms` file:

for `<tws>`:  [6, 8, 10, 12, 14, 16, 20]

for `<twa>`:  [52, 60, 75, 90, 110, 120, 135, 150]

 - `NATCERTN.FILE_ID`
 - `SAILNUMB` sail number
 - `NAME` boat name
 - `TYPE` boat type
 - `BUILDER` boat builder
 - `DESIGNER` boat designer
 - `YEAR`
 - `CLUB`
 - `OWNER` name of owner
 - `ADRS1`
 - `ADRS2`
 - `C_Type` Club or international
 - `D` One of 'C', 'S' or 'R'
 - `CREW` Crew weight (kilograms)
 - `DD_MM_yyYY HH:MM:SS`
 - `LOA` Length over all (meters)
 - `IMSL`
 - `DRAFT` Draft (meters)
 - `BMAX` Maximum beam (meters)
 - `DSPL` Displacement (kg)
 - `INDEX`
 - `DA`
 - `GPH` General purpose handicap
 - `TMF`
 - `ILCGA`
 - `PLT-O`
 - `PLD-O`
 - `WL<tws>` Windward / Leeward @tws
 - `OL<tws>` ?? @tws
 - `CR<tws>` Circular random @tws
 - `NSP<tws>` Non spinnaker circular random @tws
 - `OC<tws>`
 - `UA<tws>` optimal beat angle @tws (true wind angle)
 - `DA<tws>` optimal gybe angle @tws (true wind angle)
 - `UP<tws>` Beat VMG @tws (kts)
 - `R<twa><tws>` Time allowance @twa/@tws (s/Nautical mile)
 - `D<tws>` Run VMG @tws (kts)
 - `OTNLOW` Offshore triple number low
 - `OTNMED` Offshore triple number mid
 - `OTNHIG` Offshore triple number high
 - `ITNLOW` Inshore triple number low
 - `ITNMED` Inshore triple number mid
 - `ITNHIG` Inshore triple number high
 - `DH_TOD`
 - `DH_TOT`
 - `PLT-I`
 - `PLD-I`
 - `TMF-OF`
 - `PLT2H`
 - `PLD2H`
 - `OSN`
 - `ReferenceNo`
 - `CDL`
 - `DSPS`
 - `WSS` Wetted surface (m²)
 - `MAIN` Maximum main sail area (m²)
 - `GENOA` Maximum genoa area (m²)
 - `SYM` Maximum symmetrical spinnaker area (m²)
 - `ASYM` Maximum asymmetrical spinnaker area (m²)

## Links
 - [Uitleg over certificaat op orc.org](http://orc.org/index.asp?id=23)
 - OpenCPN book: [weather routing plugin](http://opencpn.org/ocpn/book/export/html/267)
 - Collapse sidebar (http://www.bootply.com/mL7j0aOINa)
 - Bootstrap toggle switch (interpolation on/off) http://www.bootstraptoggle.com/

## update site

- (Pas het jaar aan in `Makefile`)
- download de nieuwe RMS-files met `make rms`
- Converteer naar de juiste site-jsons met `make site`
- Update jaartal en site, update bundle (`npm run bundle`) en commit.
