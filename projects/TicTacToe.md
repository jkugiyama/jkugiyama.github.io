---
layout: project
type: project
image: img/TicTacToe.jpg
title: "TicTacToe(WIP)"
date: 2024
published: true
labels:
  - Java
summary: "A simple Tic Tac Toe game with a GUI, I hope to incoorperate AI into."
---

While not the flashiest project to display, it is a project I hope to continue adding onto. There are many ways to add onto this such as changing the level of difficulty of AI you play against.

Here is the board implementation of the tic-tac-toe with GUI.

```java
public class TicTacToeGUI extends JPanel {
   /********** label. **********/
   private JLabel lTitle = new JLabel("tic-tac-toe");
   /********** array for playable spots. *****/
   JButton [][] bGrid = {{ new JButton(" "), new JButton(" "), new JButton(" ")},
         {new JButton(" "), new JButton(" "), new JButton(" ")},
         {new JButton(" "), new JButton(" "), new JButton(" ") }};
   
```
