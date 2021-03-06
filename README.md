# Webbutveckling III

### av Gianluca Incandela giin1900@student.miun.se

## Moment 5 - REST-webbtjänst:

Den här REST-webbtjänsten är skapad med PHP och hanterar information om de kurser jag läst tidigare i programmet.
Den läser in data från en databas och hämtas ut i JSON-format som komsumerar med full CRUD-funktionalitet via Fetch API anrop. 
Webbtjänsten är skapad med objektorienterad PHP-programmering med anslutning mot MySQL-databasserver.

### 1.1 Sätt upp databasen via SQL-fråga:

CREATE TABLE `courses` (
  `id` int(11) NOT NULL,
  `code` varchar(64) NOT NULL,
  `name` varchar(64) NOT NULL,
  `progression` varchar(64) NOT NULL,
  `syllabus` varchar(128) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

INSERT INTO `courses` (`id`, `code`, `name`, `progression`, `syllabus`) VALUES
(1, 'DT057G', 'Webbutveckling I', 'A', 'https://www.miun.se//utbildning//kursplaner-och-utbildningsplaner//Sok-kursplan//kursplan//?kursplanid=17948'),
(3, 'DT084G', 'Introduktion till programmering med JavaScript', 'A', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21877'),
(4, 'DT163G', 'Digital bildbehandling webb', 'A', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21898'),
(5, 'DT003G', 'Databaser', 'A', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21595'),
(6, 'GD008G', 'Typografi och form', 'A', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21669'),
(7, 'DT093G', 'Webbutveckling II', 'B', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21874'),
(8, 'DT068G', 'Webbanvandbarhet', 'B', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=19699'),
(9, 'DT152G', 'Webbdesign CMS', 'B', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21872'),
(10, 'DT173G', 'Webbutveckling III', 'B', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=21873'),
(11, 'IK060G', 'Projektledning', 'A', 'https://www.miun.se\\/utbildning\\/kursplaner-och-utbildningsplaner\\/Sok-kursplan\\/kursplan\\/?kursplanid=18594');


### 1.2 Skapa databas användernamn:
   HOST: localhost
   USER: dbtest
   PAASWORD: password
   DATABASE: dbtest

### 2. Klona projekt:

git clone https://github.com/jbbreil/moment5Steg1.git

### 3. XAMPP installation:

Installera xampp-application för att hämta JSON-datakälla ur databasen i lokalt.

### 4. Initialisering konsol kommando:

npm install --save --dev

