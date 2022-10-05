## Llenguatge Compilat ( Java ) 
Hem escollit Java com a llenguatge compilat ja que es un llenguatge amb el que no estem familiaritzats i ens serà útil saber quant més millor sobre el seu funcionament/sintaxi.

### Compilant Java amb javac
He instalat javac, un compilador bastant senzill que s'utilitza de la següent forma:
![image](https://user-images.githubusercontent.com/96839905/194018723-727b5315-681f-4b9d-bc60-ef6baf647cd7.png)

Per a passar el codi font a codi d'objecte només tindrem que executar l'arxiu amb javac, cosa que creará l'arxiu class a partir del codi font.

Extensions dels fitxers de codi font i objecte:

![image](https://user-images.githubusercontent.com/96839905/194020406-b906b9cf-c92c-49b1-8572-a18c51b65d4f.png)

### Exemple de codi

Programa de dau de 6 cares amb Java (he fet servir nano per escriure el codi desde la terminal)

```// Inici del programa, logica y declaració de variables:

public class java6 {
  public static void main(String[] args) {
      
     int dau = (int) Math.floor(Math.random()*6 + 1); 
 // math random genera un número entre 0 i 6 aquest no inclós ( per això el +1 final) i desprès math floor s'arrodoneix els decimals del resultat a la baixa (de forma que no podem obtenir un 7 si surt mes de 6.5).
    
 // Output de dades
 
     System.out.println("Resultat de la cara obtinguda: ");
     ;
     
// Switch per al resultat del math random/floor (resultat del dau)

    switch (dau) {
    case 1:
      System.out.println("T'ha tocat el número \"un\".");
      break;
    case 2:
      System.out.println("T'ha tocat el número  \"dos\".");
      break;
    case 3:
      System.out.println("T'ha tocat el número \"tres\".");
      break;
    case 4:
      System.out.println("T'ha tocat el número \"quatre\".");
      break;
    case 5:
      System.out.println("T'ha tocat el número \"cinc\".");
      break;
    case 6:
      System.out.println("T'ha tocat el número\"sis\".");
      break;
    default:
      System.out.println("Número no disponible al dau >:(");
    }
  }
}
```
### Avantatges de fer servir un llenguatge compilat

### IDE's per al desenvolupament amb java

IntelliJ, VisualStudio Code, Eclipse.


## Llenguatge Interpretat
Com a llenguatge interpretat ens ha tocat realitzar un dau de 6 cares utilitzant R desde la línia de comandes.

### Descripció de l'intèrpret
A l'interior del fitxer ens trobem aixó

![image](https://user-images.githubusercontent.com/96839905/194037664-044efcdd-c084-4029-b400-95266d033a58.png)


 #### El sample(1:6, 1):
 El 1:6 es el rang de nombres que surtiran aletoriament
 
 El 1 es la quantitat de nombres aleatoris que sortiran cada vegada que executem el programa,en aquest cas 1.
 
 ### L'executable
 
 En primer lloc hem de instalar el paquet
 
![image](https://user-images.githubusercontent.com/96839905/194037819-bd0a378f-b0aa-42fb-9ce5-0c2be9948762.png)

El Rscript es l'executable del llenguatge R per a que fagi corre els programas

![image](https://user-images.githubusercontent.com/96839905/194037893-7191267e-e6bb-4ed0-b8b9-4cc11824b9a6.png)


### Extensions del codi font

La extensio .R es la que s'utiltza en aquest cas

![image](https://user-images.githubusercontent.com/96839905/194038114-6dbdac56-540c-427a-866b-f84db56e854d.png)


### Avantatges i desaventatges dels llenguatges interpretats

#### Avantatges

Es multiplataforma, ja que, l'interpet sol estar en varis sistemes operatius

Es pot portar a diferents plataformes

Al poder executarse en el navegador client, disminueix la carga de treball del servidor web aumentant aixiques el seu rendiment

#### Desaventatges

A la hora de l'execució del programa, quan compilam el transformam a codi màquina i això fa que baixa la velocitat de l'execució

Aunque sigui multiplataforma, si la màquina no te l'interpret no funcionara

### IDE de desenvolupament

Visual Studio code, RStudio i Geany


