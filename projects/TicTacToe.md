---
layout: project
type: project
image: img/TicTacToe.jpg
title: "TicTacToe (WIP)"
date: 2024
published: true
labels:
  - Java
summary: "A simple Tic Tac Toe game with a GUI, I hope to incoorperate AI into."
---

While not the flashiest project to display, it is a project I hope to continue adding onto. There are many ways to add onto this such as changing the level of difficulty of AI you play against.

Here is the framework of the tic-tac-toe with GUI.

```java
public class TicTacToeGUIFrame { 
   /** main method.
   * @param args not used.
   */
   public static void main(String[] args) {
      JFrame pfr = new JFrame("TicTacToeGUI");
      
      pfr.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
         
      pfr.getContentPane().add(new TicTacToeGUI());
      
      
      pfr.pack();
      pfr.setVisible(true);
```
