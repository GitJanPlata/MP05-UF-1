# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

  - **Resultat 1: 16-14+2= 4**
  - **Resultat 2: 16-14+2 = 4**
  - **Resultat 3: 8-6+2 = 4**


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)

  - **Diagrama:**
![image](https://user-images.githubusercontent.com/96839905/204739663-a0362549-afce-4fe2-b95d-c07520203434.png)

  - **Resultat CC: 2 + 1 = 3**

3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama: ![image](https://user-images.githubusercontent.com/96839905/204747661-ac9a1110-65c5-43d1-ba61-da61cd77d61b.png)
**
  - **Resultat CC: 8-6+2 = 4**

4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama: ![image](https://user-images.githubusercontent.com/96839905/204747067-befadecf-8293-488a-9308-0bfd4f7ce879.png)
**
  - **Resultat CC:9-9+2 = 2**
  - **Resultat proves camins: if hora <= 8 ( 6 = True, 9 = false)  if hora >=20 ( 15 = false, 23 = true)**

5. Investiga sobre les proves de caixa negra:

  - **Què són?**
  -Son probes de programari com les de caixa blanca, pero mes senzilles i amb altres propòsits que les de caixa blanca de forma que poden ser executades per algu sense ple coneixement al contrari de les de caixa blanca.
  - **Quina diferència principal tenen sobre les de caixa blanca?**
  - Les probes de caixa negra son proves en les que només es te en compte els valors de l'entrada i la sortida del programa, sense parar a tenir en compte l'estructura i funcionament d'aquest, contrari al que fan les de caixa blanca.
