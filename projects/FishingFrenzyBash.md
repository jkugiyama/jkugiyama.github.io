---
layout: project
type: project
image: img/fishinggame.png
title: "Fish Frenzy Bash"
date: 2023
published: true
labels:
  - Java
  - GitHub
summary: "A text based fishing game that my team developed in ICS 211."
---


Fishing frenzy bash is a text based fishing game that I helped create as a team project in ICS 211, Fall 2023. Through this project, I was able to strengthen my skills in coding through implementing hierarchal relationships amongst 21 Java files, ultimately demonstrating proper usage of inheritance and polymorphism. Along with that, I was able to practice working alongside a team, with emphasis on communication, as well as engage with the usage of Github.

Here is some code used to create the pond where the fishing takes place.

```java
public class FishingFrenzyBash {
   /** Max size capacity for pond. */
   static final int POND_SIZE = 56;
   /** Game duration in months. */
   static final int GAME_LENGTH = 12;
   /** Number of turns for player per month. */
   static final int PLAY = 3;
   /** 
   * Main method.
   * @param args not used
   */
   public static void main(String[] args) {
      // ArrayList for fish pond
      ArrayList<FishableI_a> lokoIa = new ArrayList<>();
      boolean fish = true;
      
      //Filliing up pond with baby fish
      lokoIa = FishingFrenzyBash.fillPond();
      
      // if(fish) {
   //          System.out.println(lokoIa);
   //       }
      
      //Simulating two years for fish growth
      FishingFrenzyBash.growFish(lokoIa);
      //Open pond for fishing
      FishingFrenzyBash.lawaIa(lokoIa);
      //
      
   } //close main
   
   /**
   * Fill pond method.
   * @return aList the fish pond
   */
   public static ArrayList<FishableI_a> fillPond() {
      ArrayList<FishableI_a> aList = new ArrayList<>();
      
      //make 50 baby fish in the pond
      
      for (int i = 0; i < 14; i++) {
         aList.add(new MoiLi_i());
         aList.add(new Oama());
         aList.add(new Pua_ama());
         aList.add(new Ohua());
      }
      return aList;
   
   } //close fillPond
```
 
Source: <a href="https://github.com/ICSatKCC/a6-lawa-i-fishing-game-f23-g4_f23_a6"><i class="large github icon "></i>ICSatKCC/a6-lawa-i-fishing-game-f23-g4_f23_a6</a>
