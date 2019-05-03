Στο φάκελο αυτό θα βρείτε:

  α) το αρχείο του τελικού κώδικα (.hex) του micro:bit
  
  β) την τεκμηρίωση του κώδικα

## Βασικές συναρτήσεις και Περιγραφή λειτουργίας

**Κατά την έναρξη**
To μπλόκ αυτό εκτελείται μόνο μια φορά κατά την έναρξη του προγράμματος

![OnStart](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/OnStart.JPG)

**Για Πάντα**
To μπλόκ αυτό εκτελείται για πάντα

![ForEver](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/ForEver.JPG)


**TurnOnlyLeftLightOn**:
Ανάβει μόνο το αριστερό φανάρι της διάβασης (ελέγχεται από τον ακροδέκτη P8)
![TurnOnlyLeftLightOn](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/TurnOnlyLeftLightOn.JPG)


**TurnOnlyRightLightOn**:
Ανάβει μόνο το δεξιό φανάρι της διάβασης(ελέγχεται από τον ακροδέκτη P12)

![TurnOnlyLeftLightOn](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/TurnOnlyRightLightOn.JPG)


**TurnLightsOff**:
Σβήνει και τα 2 φανάρια

![TurnLightsOff](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/TurnLightsOff.JPG)


**TurnLightsOn**:
Ανάβει και τα 2 φανάρια

![TurnLightsOn](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/TurnLightsOn.JPG)


**OpenBar**:
Γυρίζει τον άξονα του servo σε 0 μοίρες, ώστε η μπάρα να ανέβει, ελευθερώνοντας τη διάβαση.
![OpenBar](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/OpenBar.JPG)


**CloseBar**:
Γυρίζει τον άξονα του servo κατά 90 μοίρες, ώστε η μπάρα να κατέβει, κλείνοντας τη διάβαση.
![CloseBar](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/CloseBar.JPG)


**BeepAndBlinkLights**:
Παράγει ηχητικούς τόνους και θα αναβοσβήνει τα φανάρια της διάβασης ώστε να ειδοποιούνται οι οδηγοί που περιμένουν στη διάβαση

![BeepAndBlinkLights](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/BeepAndBlinkLights.JPG)


**trainPass**:
Βασική συνάρτηση που καθορίζει όσα πρέπει να γίνονται όταν ο αισθητήρας στη γραμμή ανιχνεύσει τρένο
![trainPass](https://github.com/jomihal/Automatic-Rail-way-crossing/blob/master/Code/trainPass.JPG)

Η βασική της λειτουργία είναι:


    • Θα ανάβει και τα 2 φανάρια της διάβαση για 1 δευτερόλεπτο (ειδοποίηση οδηγών)

    •	Θα κατεβάζει τη μπάρα (κλήση συνάρτησης CloseBar)

    •	Θα περιμένει 0.5 δευτερόλεπτα

    •	Θα παράγει οπτική και ηχητική ειδοποίηση για τη διέλευση του τρένου (κλήση συνάρτησης BeepAndBlinkLights)

    •	Θα σβήνει τα φανάρια της διάβασης (κλήση συνάρτησης turnLightsOff)

    •	Θα ανεβάζει τη μπάρα της διάβασης (κλήση συνάρτησης OpenBar)

