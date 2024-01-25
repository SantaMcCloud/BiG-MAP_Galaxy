FRAGEN:

BEOBACHTUNG:
- Mit gefixter bigscape.py funktioniert das nutzen der Metadata option plötzlich
- Mit ungefixter .py kommt ein fehler ->  error beim Biom erstllen -> siehe error.log
- Ohne .py wird auch Metadata genommen auch ohne Fehler
    => komisch aber interssant

TODO:
- Herausfindne wie man über das package auf die .py kommt -> wahrscheinlich nur möglich wenn man entweder den path als argument einfügt oder gesagt bekommt wo alles gespeichert wird (oder das recipe ändern?). Falls es andere möglichkeiten gibt hab ich diese nicht gefunden.
- Local alles option durchtesten -> WICHTIG!
    - zum schluss ein lauf für nur metatranscriptomic machen und schaune ob die optionen gehen
- Mit dem Wrapper rasufinden ob der Fehler wie oben beschrieben auch auftaucht
- Wenn es ein Release recipe fertig schreiben -> WICHTIG
- Mithilfe von [__foobar@0.0.1] den Wrapper testen -> läuft mit localen Dateien
- Outputs erstellen
- Test erstellen
- help text für jeden param aktualisieren
- parameter überprüfen ob alle grenzen richtig sind und alle eingetragen sind was es an parameter gibt
    - Man muss entwerder bei .analyse [BiG-MAP.map.meta.dec.biom] oder [BiG-MAP.mapcore.metacore.dec.biom] nehmen
        - [.map.] = alles und [.mapcore.] = nur core!!!!!!
        - sind in den order von output welcher map nutzt und dann noch /biom-results/ !!!!
    - Man muss entwerder [--explore] oder [--compare] nehmen oder beide!!
        - Für [--explore] muss auch [-t] angeben werden sowie [-fe] !!!!!
        - Wenn man [--compare] nutzt muss man auch [-g] nutzen => WICHTIG!!!!
        - auch hier muss man dann [-af] und [-ak] und [-fc]einstellen können!!!!!
        - [-fc] man gibt erst an wie die KW file heißt dann wie die FIZ file heißt
        - so einstellen das!!!!!!
        - explore + t + fe
        - compare + -af + ak + fc
- Help section schreiben

ERRORS:

GETESTETE OPTIONS:
- .downlaod.py => fertig getestet
    - [-A] 
        - getestet
    - [-O] 
- .family.py
    - [-D] 
        - getestet
    - [-O] 
        - getestet
    - [-b] 
        - getestet
    - [-pf]
        - getestet
    - [-tg]
        - getestet
    - [-th]
        - getestet
    - [-c]
        - getestet
    - [-f]
        - getestet -> gibt sogar aus wenn die nummer für gewisse files zu größ ist
    - [-g] 
        - getestet
    - [-s]
        - getestet
    - [-k]
        - getestet
    - [-p]
        - kann ignoriert werden
    - [--metatranscriptomes]

- .map.py
    -
- .analyse.py => fertig getestet
    - [--explore]
        - gestetet
    - [-B]
        - getestet, nimmt beide Files
    - [-T]
        - getestet -> gibt error wenn metatranscriptomic data nicht gibt (teseten zum schluss noch)
    - [-g]
        - getestet
    - [--compare]
        - getestet
    - [-O]
        - getestet
    - [-M]
        - gestetet -> gibt ein Error falls die Metagroup nicht vorhanden ist
    - [-ak]
        - getestet
    - [-af]
        - getestet
    - [-co]
        - getestet
    - [-fe]
        - getestet 
    - [-fc]
        - getestet
    - [-t]
        - getestet
    
    

DONE:
- Did create a new issue where i ask if its possible to make release for makeing the recipe -> NO ANSWER YET (24.01)
- it seem the error only happen if the [.family.py] didn't run correct
