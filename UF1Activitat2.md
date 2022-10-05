Programa de dau 6 cares amb Java.

```// Inici del programa, logica y declaració de variables:
public class java6 {
  public static void main(String[] args) {
      
     int dau =(int) Math.floor(Math.random()*6 + 1);
    
// Output de dades
     System.out.println("Resultat de la cara obtinguda: ");
     ;
// Switch per al resultat
    switch (dau) {
    case 1:
      System.out.println("T'ha tocat el número \"un\".");
      break;
    case 2:
      System.out.println("T'ha tocat el numero  \"dos\".");
      break;
    case 3:
      System.out.println("T'ha tocat el numero \"tres\".");
      break;
    case 4:
      System.out.println("T'ha tocat el numero \"quatre\".");
      break;
    case 5:
      System.out.println("T'ha tocat el numero \"cinc\".");
      break;
    case 6:
      System.out.println("T'ha tocat el numero\"sis\".");
      break;
    default:
      System.out.println("Numero incorrecte >:(");
    }
  }
}´´´
