import java.util.*;
public class ReverseString{
public static void main(String[] args){
   String sentence = "This is a string";
String[] words = sentence.split(" ");
String invertedSentece = "";
for (String word : words){
    String invertedWord = "";
    for (int i = word.length() - 1; i >= 0; i--)
        invertedWord += word.charAt(i);
    invertedSentece += invertedWord;
    invertedSentece += " ";
}
System.out.println(invertedSentece.trim());
    }
}
