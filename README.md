# recalbox-gamelists
Emulationstation gamelists and images for recalbox.

This repository regroups gamelists and images for emulationstation systems in recalbox.

Rom names are based on "NO-INTRO" sets, that are very clean sets for many systems.

From the website of no-intro : 
>What "No-Intro" does is fill some .dat files, to be used with ROM-Managers, with information about the known ROMS released. Often there are more versions of the same ROM dump, but most of them are garbage, some examples may include: bad dumps, hacks, fakes, overdumps, underdumps, and so on. "No-Intro" lists only the best available ROM; it must be a full dump with no faults and no changes to the file, basically just the ROMS that are the closest as possible to the original licensed cartridges. 

See http://www.no-intro.org/ for more informations on their game database.


**If you want to contribute, here is the procedure :**
- Only use No-Intro data files.
- First, use the special scrapper at https://github.com/digitalLumberjack/ES-scraper, it bases the scrape on games checksums, so you'll have no errors in scraped games.
- Then use babou's https://github.com/bbouko/Recalbox-scraper to scrape remaining games basing search on file names.
- If you add custom image, the maximum width should be 375px and the maximum height should be 350px.
- Create a pull request with the modified gamelists and images.

The special scrapper automatically resize scrapped image to the good size. It also add the *region* tag with corresponding region in xml data. A *romtype* tag is added too, with a default value set to *Official* if the title do not contains the string *(Proto)*.
