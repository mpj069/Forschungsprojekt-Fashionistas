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

1a) Wie sind bekannte Modedesigner*innen der 90er Jahre mit Fashion Brands verbunden?

1b) Gab es einen Wechsel zu einem anderen Label? Arbeiten sie exklusiv für eine renomierte Marke?

1c) Welchen Rang hat der/die Designer*in ?

Für das Modemarkennetzwerk *collaborations* wurde den Rängen des Designers ein Gewicht von 1-3 vergeben,  3 steht für Founder, 2 für Creative Director, und 1 für Design assistant


**Projektnetwerk Designerfakten**

1)Gibt es ausschlaggebende Fakten über die Designer*innen?

Für dieses Netzwerk recherchierten wir Attribute wie Ausbildungsgrad, Sexualität, Alter, Herkunftsland, und Musen der Designer*innen. 



**N.A**
Fehlende Werte werden nicht erfasst, und als N.A angegeben.



# EDGE-Attribute


**from**

initiierender Knoten, in diesem Fall: Designer/in wechselte von einer zur anderen Marke.

**to**

erhaltender Knoten, in diesem Fall: Marke , für die ein/e Designer*in arbeitet.

**weight**  
Designerrang innerhalb des Modelabels 
3 = Founder
2 = Creative Director or other Designer Role
1 = Design Assistant


**position**

Designer*innen Rang innerhalb einer Brand

1 = Design Assistant
2 = Creative Director
3 = Founder

**year**

Jahr, in dem der Wechsel stattfand.






# NODE-Attribute  
  
**id**  

(eindeutige Codierung des Knoten )
klare Codierung durch Abkürzung der Namen der Knoten, jede ID entspricht einem Designer. Knoten für die Musen (Models) werden noch erhoben. Hierbei untersuchen wir, ob die Musen zu der neuen Modemarke mit gewechselt sid.

**name**

voller Name


**sex** 

1 = weiblich  
2 = männlich  
3 = divers
  

**birthyear**   

Geburtsjahr des Knotens  


**main workplace**
	
D = Deutschland
USA = Amerika
IT = Italien
F = Frankreich 
GB = England
JAP = Japan
DR = Dominikanische Republik
VEN = Venezuela
BRA = Brasilien


**type**

1 = designer
2 = brand
3 =  muse



**scholar**

Abschlussart des Designers 

1 = *talent* : Der/Die Designer*in hat bis auf seine kreative Ader keinen Abschluss.
2 = *internship/work experience* : Der/Die Designer*in hatte eine Art Ausbildung bei einem Mentor.
3 = *degree* Der/Die Designer*in hat einen akademischen Abschluss.


**sexuality**  

1 = heterosexual: Der/Die Designer*in ist heterosexuell
2 = homosexual: Der/Die Designer*in ist homosexuell   
3 = bisexual : Der/Die Designer*in ist bisexuell
4 = pansexual: Der/Die Designer*in ist pansexuell
5 = asexual : Der/Die Desdigner*in ist asexuell


**transfer**

0 = Der/Die Designer*in hat von Anfang an ein eigenes Label gegründet.
1 = Der/Die Designer*in hat die Marke ein mal gewechselt
2 = Der/Die Designer*in hat die Marke zwei mal gewechselt
3 = Die Marke wurde drei oder mehrmals gewechselt


**value**

Designervermögen/ Markenwert

1 = unter 2 Mrd. Dollar
2 = 2-10 Mrd. Dollar
3 = 10-50 Mrd. Dollar
4 = 50-100 Mrd. Dollar


##

