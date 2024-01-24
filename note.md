FRAGEN:

BEOBACHTUNG:
- Mit gefixter bigscape.py funktioniert das nutzen der Metadata option plötzlich
- Mit ungefixter .py kommt ein fehler ->  error beim Biom erstllen -> siehe error.log
- Ohne .py wird auch Metadata genommen auch ohne Fehler
    => komisch aber interssant

TODO:
- Herausfindne wie man über das package auf die .py kommt -> wahrscheinlich nur möglich wenn man entweder den path als argument einfügt oder gesagt bekommt wo alles gespeichert wird (oder das recipe ändern?). Falls es andere möglichkeiten gibt hab ich diese nicht gefunden.
- Local alles option durchtesten -> WICHTIG!
- Mit dem Wrapper rasufinden ob der Fehler wie oben beschrieben auch auftaucht
- Wenn es ein Release recipe fertig schreiben -> WICHTIG
- Mithilfe von [__foobar@0.0.1] den Wrapper testen -> läuft mit localen Datein
    - Schauen ob man beide tools direkt mit planemo bekommen kann dann kann man volle funktionalität prüfen (nicht vergessen die bigscape.py fix version zu nehmen)
- Outputs erstellen
- Test erstellen
- help text für jeden param aktualisieren
- Help section schreiben

ERRORS:

DONE:
- Did create a new issue where i ask if its possible to make release for makeing the recipe -> NO ANSWER YET (24.01)
- it seem the error only happen if the [.family.py] didn't run correct
