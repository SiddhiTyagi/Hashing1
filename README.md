# Hashing1
import java.util.HashSet;   // to use HashSet
import java.util.Iterator;   // to use Iterator
class Hashing1{
    public void main(){
        //like in-> ArrayList<Integer> list=new ArrayList<>();
        //list.add(element)
        
        //create
        HashSet<Integer> set=new HashSet<>();
        
        //insert
        set.add(19);
        set.add(31);
        set.add(21);
        set.add(31);
        set.add(1);
        set.add(5);
        set.add(10);
        
        //print all elements of set(in unordered way)
        System.out.println(set);
        
        //1.delete-remove
        set.remove(31);
        System.out.println(set);
        
        //2.
        set.remove(19);
        if(!set.contains(19))
        System.out.println("We removed 19 from the set");
        
        //search-contains
        if(set.contains(21))
        System.out.println("21 present in set");
        else
        System.out.println("21 not present in set");
        
        //set size
        System.out.println("The size of the set is "+set.size());
        
        //iterator in hashset has two functions- 
        //it.next() gives the next value of set & it.hasNext() checks if the set has further values
        
        //create
        Iterator it=set.iterator();
        
        //print every value of set whilst iterating
        while(it.hasNext())
        System.out.println(it.next());
    }
}
