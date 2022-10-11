## Llenguatge compilat ( C++ ) 
Hem escollit C++ com a llenguatge compilat.


### Compilant amb C++
He creat l'arxiu de codi font .cpp amb nano i he afegit el codi per al dau de 6 cares amb c++.

![image](https://user-images.githubusercontent.com/96839905/195153331-2d83afa3-ec06-4213-a096-2e51c3172a2f.png)

Per compilar c++ desde la terminal farem servir g++ com a compilador. Un cop realitzada la comanda del g++ tindrem l'arxiu de codi objecte compilat i llest per executar-se.

![image](https://user-images.githubusercontent.com/96839905/195157756-d2481770-480c-4dc4-8e26-6221b8d1090c.png)

Per executar el codi compilat simplement tindrem que fer servir la comanda ./ a la terminal.

![image](https://user-images.githubusercontent.com/96839905/195168548-e968e04c-5808-499e-81d7-fe043666343b.png)

### Avantatges i desventatges de fer servir un llenguatge compilat.

**Avantatges**:

El codi executable obtingut es el mes eficient i rápid.

S'utilitza principalment per a desenvolupament d'aplicacions d'escriptori.

**Desventatges**:

 Normalment requereixen més recursos del sistema i consumeixen mes capacitat de hardware.
 
 Requereix finalitzar el programa per a poder executar-lo.
 
 La compilació s'ha de fer cada cop que el codi font es modifica.
 
 El tipat de dades es mes restrictiu, en molts casos rígid.
 
 Els arxius executables solen ocupar mes espai.
 
 Poc portable.
 
### Webgrafía:

https://hetpro-store.com/TUTORIALES/compilar-cpp-g-linux-en-terminal-leccion-1/

https://es.stackoverflow.com/questions/156709/lanzamiento-de-dados-en-c

https://ehack.info/lenguajes-compilados-vs-lenguajes-interpretados/

### IDE's per al desenvolupament amb C++
VSCode, C++ Builder, CodeLite

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

A la hora de l'execució del programa, quan compilem el transformem a codi màquina i això fa que baixi la velocitat d'execució

Aunque sigui multiplataforma, si la màquina no te l'interpret no funcionara

### IDE de desenvolupament

Visual Studio code, RStudio i Geany

## Llenguatge de VM ( Java ) 
Hem escollit Java com a llenguatge de Maquina virtual.

### Compilant Java amb javac
He instalat javac, un compilador bastant senzill que s'utilitza de la següent forma:
![image](https://user-images.githubusercontent.com/96839905/194018723-727b5315-681f-4b9d-bc60-ef6baf647cd7.png)

Per a passar el codi font a ByteCode només tindrem que executar l'arxiu amb javac, cosa que creará l'arxiu class a partir del codi font.

Extensions dels fitxers de codi font i ByteCode:

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
### Avantatges i desventatges de fer servir un llenguatge de MV
**Avantatges**:

Son l'opció mes versàtil del les 3 ja que la propia màquina virtual fa d'interpret i compilador així no t'has de preocupar de si la maquina tindra la capacitat de llegir o no el codi.

**Desventatges**:

Agregan gran complexitat al sistema en temps d'execució, el que implica treball extra per a la maquina.

Son més lents que els llenguatges completament compilats, a causa de la sobrecàrrega que genera tenir una capa de programari intermèdia entre l'aplicació i la màquina.

### IDE's per al desenvolupament amb java

IntelliJ, VisualStudio Code, Eclipse.

### Webgrafía
https://ehack.info/lenguajes-compilados-vs-lenguajes-interpretados/
