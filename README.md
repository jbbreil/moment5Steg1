# Webbutveckling III

### av Gianluca Incandela giin1900@student.miun.se

## Moment 5 - REST api PHP - Steg 1

Den här wbbtjänsten är skapad med PHP och hanterar information om de kurser jag läser på Mittuniveristet.
Den läser in data från en databas och hämtas ut i JSON-format och är impementerad med CRUD.

1. Sätt upp databasen:
   CREATE TABLE IF NOT EXISTS `courses` (
   `id` int(11) NOT NULL,
   `code` text NOT NULL,
   `name` text NOT NULL,
   `progression` text NOT NULL,
   `syllabus` text NOT NULL,
   PRIMARY KEY (id)
   ) ENGINE=InnoDB DEFAULT CHARSET=latin1;


### Klona projekt:

git clone https://github.com/jbbreil/moment5Steg1.git
