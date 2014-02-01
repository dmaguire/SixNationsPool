SixNationsPool
==============

Simple script for managing an in office Six Nations pool.

Usage is relatively straightforward, using git style commands.

### Add:

snpool add help displays help text for the add commands.

**add player** \<forename\> \<surname\> \<email\> \<paid\>  
**add match**  \<hometeam\> \<awayteam\> \<venue\> \<date\> \<time\>  
**add result** \<match-id\> \<homescore\> \<awayscore\>  
**add guess**  \<player-id\> \<match-id\> \<homescore\> \<awayscore\>  

### Print/Display:

snpool print help displays help text for the print commands.
Note: \'print\' can be replaced with \'display\' in all the below commands.

**print players**       - Displays details of the players signed up for the Pool.  
**print player \<id\>** - Displays details of a specific player, by ID.  
**print matches**       - Displays details of the Six Nations championship matches.  
**print match \<id\>**  - Displays details of individual matches, including player guesses and statistics.  
**print results**       - Displays short form details of the Six Nations results.  
**print sn-table**      - Displays the current Six Nations results table.  
**print pool**          - Displays the current Pool results table.  
**print short**         - Displays a short list of players.
**print debug**         - Displays the pool table, but with debug information displaying calculations.

NOTE: Current sn-table remains unwired, because I haven't gotten round to implementing it yet. Which obviously leads to...

### Update:

snpool update updates various player information points

**update name \<id\> \<name\>**           - Updates players forename.
**update surname \<id\> \<surname\>**     - Updates players surname.
**update email \<id\> \<email\>**         - Updates players email.
**update paid \<id\> \<paid\>**           - Updates players paid status.
**update guess \<id\> \<match-id\> \<homescore\> \<awayscore\>** - Updates players guess for specified match.

### TODO:
* Work out a way of calculating the SN Table
    * This may require some reworking of the Matches structure to allow it to be 'team aware' or something like that. 
* ~~Add the ability to edit data (should be relatively straight forward, using IDs).~~
* ~~Add alternative printing mechanisms (short form player and match lists would be useful).~~
