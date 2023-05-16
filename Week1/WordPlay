import edu.duke.*;

public class WordPlay {

    public Boolean isVowel(char ch) {
        String vowel = "aeiou";
        for (int i = 0; i<vowel.length(); i++) {
            char currChar = vowel.charAt(i);
            if (ch == (currChar) || ch == Character.toUpperCase(currChar)) {
                return true;
            } 
        }
        return false;
    }
   //Alternative way:
    public Boolean isVowel2(char ch) {
        String vowels = "aeiou";
        char lowkey = Character.toLowerCase(ch);
        if (vowels.indexOf(lowkey) != -1){
            return true;
        }
        return false;
    }
    
    public void testVowel() {
        char sb = 's';
        System.out.println(isVowel(sb));
        System.out.println(isVowel2(sb));
    }
    
    public String replaceVowels (String phrase, char ch) {
        StringBuilder newPhrase = new StringBuilder(phrase);
        for(int i = 0; i < phrase.length(); ++i){
            char currentChar = newPhrase.charAt(i);
            if(isVowel(currentChar)) {  
                newPhrase.setCharAt(i, ch);
            }
        }
        return newPhrase.toString();
    }
    
    public void testReplaceVowels() {
        System.out.println(replaceVowels("Hello World", '*')); 
    }
    
    public String emphasize (String phrase, char ch) {
        StringBuilder newPhrase = new StringBuilder(phrase); 
        for(int i = 0; i < phrase.length(); ++i){
            char currentChar = newPhrase.charAt(i);
            
            if ((ch == Character.toLowerCase(currentChar) || 
            ch == Character.toUpperCase(currentChar)) && i % 2 == 1) {
                newPhrase.setCharAt(i, '+');
            }
            if ((ch == Character.toLowerCase(currentChar) || 
            ch == Character.toUpperCase(currentChar)) && i % 2 == 0) {
                newPhrase.setCharAt(i, '*');
            }
        }
        return newPhrase.toString();
    }
    
    public void testemphasize() {
        System.out.println(emphasize("Mary Bella Abracadabra", 'a'));
    }
}
