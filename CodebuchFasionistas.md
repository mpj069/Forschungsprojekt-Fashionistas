##Codebuch Modedesigner*inen und Luxusmarken##
Codebuch Stand 2023-06, aktualisiert 2023-06
erstellt von Fashionistas (mj069@hdm-stuttgart.de)


## Inhalt
- Edges.csv (Edgelist)
- Nodes.csv (Nodelist)
- CodebuchFashionistas.md (Codierung der Datensätze)



## Ursprung und Datenerhebung
Wir haben den Datensatz unter den Modedesigner*innen in der Luxusmarkenbranche erhoben.

Das Netzwerk ist ein *gerichtetes Akteursnetzwerk*. Es wurden vier getrennte Fragen erhoben:

**Projektnetzwerk Modemarken collaborations**

1a) Wie sind bekannte Modedesigner*innen mit Fashion Brands verbunden?

1b)  Gab es einen Wechsel ? Arbeiten sie exklusiv für eine renomierte Marke?

1c) Welchen Rang hat der/die Designer*in ?

Für das Modemarkennetzwerk *collaborations* wurde den Rängen des Designers ein Gewicht von 1-3 vergeben,  3 steht für Founder, 2 für Creative Director, und 1 für Design assistant


**Projektnetwerk Designerfakten**

1)Gibt es ausschlaggebende Fakten über die Designer*innen?

Für dieses Netzwerk recherchierten wir Attribute wie Ausbildungsgrad, Sexualität, Alter, Land der Tätigkeiten, Mentoren und Musen der Designer*innen. 



**Umgang mit fehlgenden Werten**
Fehlende Werte werden nicht erfasst.


# EDGE-Attribute

**id**  
(eindeutige Codierung des Knoten)   
codiert von 1 bis 50 ( 10 Knoten pro Gruppenmitglied), jede ID entspricht einem Designer. Knoten für die Musen (Models) werden noch erhoben. Hierbei untersuchen wir, ob die Musen zu der neuen Modemarke mit gewechselt sid.

**from**
initiierender Knoten, in diesem Fall: Designer/in wechselte von einer zur anderen Marke.

**to**
erhaltender Knoten, in diesem Fall: Marke , für die ein/e Designer*in arbeitet.

**weight**  
Designerrang   
3 = Founder
2 = Creative Director
1 = Design Assistant

**scholar**
Abschlussart des Designers 
1 = *talent* : Der/Die Designer*in hat bis auf seine kreative Ader keinen Abschluss.
2 = *internship* : Der/Die Designer*in hatte eine Art Ausbildung bei einem Mentor.
3 = *degree* Der/Die Designer*in hat einen akademischen Abschluss.

**sexuality**  
1 = straight: Der/Die Designer*in ist heterosexuell
2 = notstraight: Der/Die Designer*in ist nicht heterosexuell     
3 = NA: Die Sexualität ist nicht bekannt


**transfer**

1 = Der/Die Designer*in hat die Marke ein mal gewechselt
2 = Der/Die Designer*in hat die Marke zwei mal gewechselt
3 = Die Marke wurde drei oder mehrmals gewechselt


# NODE-Attribute  
  
**id**  
Identische ID wie aus der edgelist zur Identifikation der Knoten.

**name**
numerische ID

**name_first**
Vorname abgekürzt, z.B. für Visualisierung, falls der Name zu lange ist

**sex**    
Bitte geben Sie ihr Geschlecht an:  
1 = weiblich  
2 = männlich  
3 = divers
  

**age_real**   
Alter in natürlichen Zahlen.  

**birthyear**   
Die Generation des Knoten:  
1 =    
2 =     
3 =   
4 =   


**location** 
Wohnort, als string/characters codiert  

**workplace**  
Einsatzland, als string/characters codiert  

##

