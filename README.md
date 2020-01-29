from random import shuffle                      # ZufallsBibliothek

superlatives = "amazing gorgeous blazing stunning tremendous greatest best fantastic \
               phenomenal delightful ambitious outstanding incredible spectacular \
               super cool magical revolutionary beautiful jaw-dropping lovely".upper().split() #upper großschreibung
shuffle(superlatives)                           # Zufall aus der Liste

for strophe in range(5):                        # 5 Strophen erzeugen
    for zeile in range(2):                      # 2 Zeilen
        for word in range(4):                   # 4 mal
            print("SPAM ", end='')              # nebeneinander
        print()
    el1 = superlatives.pop()                    # pop. damit die Variablen nicht wiederholt werden
    el2 = superlatives.pop()

    print("{} SPAM, {} SPAM".format(el1, el2))  # Ausgabe      
    print()

