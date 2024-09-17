Relaatiotietokannan peruskäsitteiden harjoitukset:

![image](https://github.com/user-attachments/assets/4a65f5a6-96a6-463b-b262-95139b9fb99f)
Kysymykset joita järjestelmä ei hyväksyny:
Kysymys 8: char
Kysymys 11: char
Kysymys 13: description
Kysymys 22: goal_id
Kysymys 24: goal,game

Yhteen tauluun kohdistuvien kyselyiden harjoitukset:  
![image](https://github.com/user-attachments/assets/266e1eb7-f28e-4b6c-b320-c4c6d4789048)  
Kysymykset joita järjestelmä ei hyväksyny:  
Kysymys 2: SELECT name, airport_type FROM airport WHERE iso_country = "FI";  
Ihan sama palautus, pitäisi olla täydet pisteet.  

Where-osan liitosehto harjoitukset:  

![image](https://github.com/user-attachments/assets/866c3ef8-f835-418f-be42-5289038703f9)  
Kysymykset joita järjestelmä ei hyväksyny:  
Kysymys 3: select country.name as "country_name", airport.name as "airport_name" from country, airport where country.iso_country = airport.iso_country and airport.continent ="AN" order by country.name ASC;  
Melko sama palautus, en ole varmaa miten voi saada paremman tuloksen.  

Join harjoitukset  
![image](https://github.com/user-attachments/assets/69554717-3300-4b04-8ff9-9b84239ccbaf)  

Kysymykset joita järjestelmä ei hyväksyny:  
Kysymys 4: select airport.name, screen_name from game right join airport on airport.ident = game.location where airport.name LIKE "%Hels%";  
![image](https://github.com/user-attachments/assets/2166583e-e1c9-4bd7-af91-57d865842e1c)  
Yksi linja ero, ei voi tehdä paremmin
Sisäkysely harjoitukset
![image](https://github.com/user-attachments/assets/b23df9ea-5ab0-42ef-a40c-29abea74e427)   
Kysymys 1: select country.name from country where name in( select name from airport where name like '%Satsuma%');   
![image](https://github.com/user-attachments/assets/5852a106-fb56-41e6-b8fb-a0bbb66004c0)    
Kysymys 2: select airport.name from airport where name in( select name from country where name like 'Monaco');   
![image](https://github.com/user-attachments/assets/24c600d7-0627-4b08-83ee-9c0dfc4e4d5b)   
Kysymys 3: select screen_name from game where id in( select game_id from goal_reached where id in ( select goal.description from goal where goal.description = "Clouds"));   
![image](https://github.com/user-attachments/assets/7f3fb7be-ddae-471c-8ff1-3be5f4fc3a78)   
Kysymys 5: select game.screen_name from game where id not in( select goal.id from goal where goal.name not in(select description from goal));    
![image](https://github.com/user-attachments/assets/76886558-bf53-4d68-93bb-ced44342106a)   
Samat koodit mutta ei hyväksy.    


