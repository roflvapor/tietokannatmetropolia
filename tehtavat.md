Relaatiotietokannan peruskäsitteiden harjoitukset:

![image](https://github.com/user-attachments/assets/f47fda4d-5346-4ae0-98df-46a556412db6)  
![image](https://github.com/user-attachments/assets/7dee9049-7a3d-4394-8cb9-3e0b95e6b234)
![image](https://github.com/user-attachments/assets/473a3f4d-0731-42c1-98cc-a01afe3659fc)
![image](https://github.com/user-attachments/assets/205c0d41-7166-4653-99fa-ecd583b4d8f6)
![image](https://github.com/user-attachments/assets/69958bdb-f560-4dc6-a999-676652029534)
![image](https://github.com/user-attachments/assets/386d40c9-f31b-46be-9e18-d9fe058fa5b7)
![image](https://github.com/user-attachments/assets/cb41ed04-469e-458f-aa60-d1eae828098e)
![image](https://github.com/user-attachments/assets/817492a5-2c76-4d89-b07c-4ccaa90dd258)
![image](https://github.com/user-attachments/assets/9815694f-370c-452c-9e05-a7e82a344818)
![image](https://github.com/user-attachments/assets/47bbd369-02d0-450a-ad6d-df1cc945cac2)
![image](https://github.com/user-attachments/assets/5d62a2ef-041a-494b-a3e3-9ad8f18b8cb8)
![image](https://github.com/user-attachments/assets/3fc47793-911e-4e05-937d-0107209c61a5)
![image](https://github.com/user-attachments/assets/19be4666-f319-434f-82eb-bc952620bc8b)
![image](https://github.com/user-attachments/assets/bba6484a-2f0d-419f-9c97-9bb55fc2e72a)
![image](https://github.com/user-attachments/assets/40601c0d-c6dc-46b9-bbb7-0b10140c8bc1)
![image](https://github.com/user-attachments/assets/34d36500-650d-49e7-a8ca-17a8e581aad0)
![image](https://github.com/user-attachments/assets/1c6878cb-38e3-406d-adff-2f02aee979ed)
![image](https://github.com/user-attachments/assets/7a08241d-5c2e-4885-a0ec-200f39b3c159)
![image](https://github.com/user-attachments/assets/c679a585-130f-43aa-9817-f630a1fe8d0e)
![image](https://github.com/user-attachments/assets/98c3660b-0774-4922-aa21-916f2e1173cc)
![image](https://github.com/user-attachments/assets/57b0b81e-f824-42f7-a163-0de858f039b1)
![image](https://github.com/user-attachments/assets/d9721225-f130-40c2-8f6d-824f80f45c7a)
![image](https://github.com/user-attachments/assets/2d5acce8-7a0b-48f3-a891-0dcdc38f2763)
![image](https://github.com/user-attachments/assets/2a5d7869-8324-479e-8b0c-0b74417aaae6)
![image](https://github.com/user-attachments/assets/033846bc-1d77-4218-9eb6-e4e33adbed69)
![image](https://github.com/user-attachments/assets/b18ef81b-11a6-4805-b6a9-3399355e1d93)


Yhteen tauluun kohdistuvien kyselyiden harjoitukset:  

![image](https://github.com/user-attachments/assets/266e1eb7-f28e-4b6c-b320-c4c6d4789048)  
Kysymykset joita järjestelmä ei hyväksyny:  
Kysymys 2: SELECT name, airport_type FROM airport WHERE iso_country = "FI";  
Ihan sama palautus, pitäisi olla täydet pisteet.  

Where-osan liitosehto harjoitukset:  

![image](https://github.com/user-attachments/assets/866c3ef8-f835-418f-be42-5289038703f9)\
Kysymykset joita järjestelmä ei hyväksyny:  \
Kysymys 3: select country.name as "country_name", airport.name as "airport_name" from country, airport where country.iso_country = airport.iso_country and airport.continent ="AN" order by country.name ASC;  
Melko sama palautus, en ole varmaa miten voi saada paremman tuloksen.  

Join harjoitukset  
![image](https://github.com/user-attachments/assets/69554717-3300-4b04-8ff9-9b84239ccbaf)\

Kysymykset joita järjestelmä ei hyväksyny:  
Kysymys 4: select airport.name, screen_name from game right join airport on airport.ident = game.location where airport.name LIKE "%Hels%";  
![image](https://github.com/user-attachments/assets/2166583e-e1c9-4bd7-af91-57d865842e1c)  
Yksi linja ero, ei voi tehdä paremmin  

Sisäkysely harjoitukset:  
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


![image](https://github.com/user-attachments/assets/b933980d-afc8-4dc2-b176-e25294731420)  

![image](https://github.com/user-attachments/assets/2725f803-268f-4a93-a27b-02e7358ff957)



