# Actividad3
Actividad 3 sobre cartas de poker 

import java.util.ArrayList;
import java.util.Collections;
import java.util.Random;
/**
 *
 * @author FTD
 */
public class Deck {
    
    public ArrayList<Card> Cards = new ArrayList<>();
    
    public Deck(){
        Cards.add(new Card("Trebol","Rojo","A"));
        Cards.add(new Card("Trebol","Rojo","J"));
        Cards.add(new Card("Trebol","Rojo","Q"));
        Cards.add(new Card("Trebol","Rojo","K"));
        Cards.add(new Card("Trebol","Rojo","2"));
        Cards.add(new Card("Trebol","Rojo","3"));
        Cards.add(new Card("Trebol","Rojo","4"));
        Cards.add(new Card("Trebol","Rojo","5"));
        Cards.add(new Card("Trebol","Rojo","6"));
        Cards.add(new Card("Trebol","Rojo","7"));
        Cards.add(new Card("Trebol","Rojo","8"));
        Cards.add(new Card("Trebol","Rojo","9"));
        Cards.add(new Card("Trebol","Rojo","10"));
        Cards.add(new Card("Corazones","Rojo","A"));
        Cards.add(new Card("Corazones","Rojo","J"));
        Cards.add(new Card("Corazones","Rojo","Q"));
        Cards.add(new Card("Corazones","Rojo","K"));
        Cards.add(new Card("Corazones","Rojo","2"));
        Cards.add(new Card("Corazones","Rojo","3"));
        Cards.add(new Card("Corazones","Rojo","4"));
        Cards.add(new Card("Corazones","Rojo","5"));
        Cards.add(new Card("Corazones","Rojo","6"));
        Cards.add(new Card("Corazones","Rojo","7"));
        Cards.add(new Card("Corazones","Rojo","8"));
        Cards.add(new Card("Corazones","Rojo","9"));
        Cards.add(new Card("Corazones","Rojo","10"));
        Cards.add(new Card("Picas","Rojo","A"));
        Cards.add(new Card("Picas","Rojo","J"));
        Cards.add(new Card("Picas","Rojo","Q"));
        Cards.add(new Card("Picas","Rojo","K"));
        Cards.add(new Card("Picas","Rojo","2"));
        Cards.add(new Card("Picas","Rojo","3"));
        Cards.add(new Card("Picas","Rojo","4"));
        Cards.add(new Card("Picas","Rojo","5"));
        Cards.add(new Card("Picas","Rojo","6"));
        Cards.add(new Card("Picas","Rojo","7"));
        Cards.add(new Card("Picas","Rojo","8"));
        Cards.add(new Card("Picas","Rojo","9"));
        Cards.add(new Card("Picas","Rojo","10"));
        Cards.add(new Card("Diamantes","Rojo","A"));
        Cards.add(new Card("Diamantes","Rojo","J"));
        Cards.add(new Card("Diamantes","Rojo","Q"));
        Cards.add(new Card("Diamantes","Rojo","K"));
        Cards.add(new Card("Diamantes","Rojo","2"));
        Cards.add(new Card("Diamantes","Rojo","3"));
        Cards.add(new Card("Diamantes","Rojo","4"));
        Cards.add(new Card("Diamantes","Rojo","5"));
        Cards.add(new Card("Diamantes","Rojo","6"));
        Cards.add(new Card("Diamantes","Rojo","7"));
        Cards.add(new Card("Diamantes","Rojo","8"));
        Cards.add(new Card("Diamantes","Rojo","9"));
        Cards.add(new Card("Diamantes","Rojo","10"));
    }
    
    public void Shuffle(){
        Collections.shuffle(Cards);
        System.out.println("Se mezclo el Deck");
        System.out.println("Quedan " + Cards.size() + " en el Deck");
    }
    
    public void Head(){
        System.out.println(Cards.get(0).Palo + "," + Cards.get(0).Color + "," + Cards.get(0).Valor);
        Cards.remove(0);
        System.out.println("Quedan " + Cards.size() + " en el Deck");
    }
    
    public void Pick(){
        Random rand = new Random();
        int index = rand.nextInt(Cards.size()); 
        
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        System.out.println("Quedan " + Cards.size() + " en el Deck");
    }
    
    public void Hand(){
        Random rand = new Random();
        int index;
        
        index = rand.nextInt(Cards.size()); 
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        index = rand.nextInt(Cards.size()); 
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        index = rand.nextInt(Cards.size()); 
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        index = rand.nextInt(Cards.size()); 
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        index = rand.nextInt(Cards.size()); 
        System.out.println(Cards.get(index).Palo + "," + Cards.get(index).Color + "," + Cards.get(index).Valor);
        Cards.remove(index);
        System.out.println("Quedan " + Cards.size() + " en el Deck");
    }
      
}
