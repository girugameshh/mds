"description" je odradjen u HTML formatu. Koristio sam Google-supported tagove, u ovom slucaju p, li i um. ![ggtags](https://github.com/girugameshh/mds/assets/40721125/942f4182-ae91-4e2c-8aaf-2506558edbce)

U "identifier" objektu sam ubacio unikatnu vrednost za "value" kljuc na svakoj stranici, lako prepoznatljivu (CompanyDriverSolo, OwnerOperator88, etc. , videces/skontaces)

Proverio sam moguce opcije za vrednosti koje mogu da se zalepe za employmentType key, CONTRACTOR je savrsen za OwnerOpove dok je FULL_TIME odgovarajuca vrednost za Company vozace
Takodje, link u logo kljucu je samo za tebe da mozes da skines sliku pa ces posle ti to podici na server i prepraviti link u lokal (skywayholdings.com/img/logo.png ili kako god bude isao path)
Datume postavi kako zelis, slobodno stavi validThrough tipa za godinu dana ili tako nesto nenormalno (prakticno perma)

Primetices da "baseSalary" objekat ne postoji na OwnerOp stranicama. Razlog je sto ne postoji schema-friendly property za JobPosting tip koji precizno opisuje model placanja za OwnerOpove koji mi koristimo (procenat od load revenue).
Najbliza stvar je "value" : 0 i "unitText" : "JOB_APPLICATION" sto je u prevodu "Pitajte nas za platu tokom apliciranja", sto nam iskreno nije od neke pomoci. Na srecu, u svakom "description" za owner operatore sam stavio prvi bullet point da bude "Compensation Model" sto je najbitnija informacija za owner operatora sto se love i placanja tice.
Takodje, baseSalary je optional field, prema tome - mozemo bez toga kad su ownerops u pitanju.

Provukao sam svaku stranicu kroz preporucene validatore https://search.google.com/test/rich-results i https://validator.schema.org/ i sve su prosle test.
