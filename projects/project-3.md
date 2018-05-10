---
layout: project
type: project
image: images/output.png
title: Sudoku Solver
permalink: projects/sudoku
# All dates must be YYYY-MM-DD format!
date: 2017-04-12
labels:
  - Java
summary: A sudoku solver that I created for ICS 211
---

<img class="ui image" src="{{ site.baseurl }}/images/output.png">
<img class="ui image" src="{{ site.baseurl }}/images/input.png">

For my ICS 211 class I was tasked to create a working sudoku solver that would take in input from a text file and output the finished result in another text file. 

Some code that shows how the code checks if the number fits.

```java

static boolean checkSquare(int n, int m) {

			//checks columns
			for (int a = 0; a < 9; ++a)  
			    if (k == matrix[a][m] && a!=n) return false;
          
			for (int a = 0; a < 9; ++a)  //checks row
			    if (k == matrix[n][a] && a!=m) return false;
			      int row = (n / 3)*3;
			      int col = (m / 3)*3;

			for (int a = 0; a < 3; ++a)
			    for (int b = 0; b < 3; ++b)
			    //checks the square
			    if (k == matrix[row+a][col+b] && row+a != n && row+b != m) return false;
          
			return true;

}

```
