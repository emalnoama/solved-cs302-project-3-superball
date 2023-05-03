Download Link: https://assignmentchef.com/product/solved-cs302-project-3-superball
<br>
<strong>                                                                                                                                                                                                                                                                                                                                         </strong><strong>Project 03: Superball!</strong>




<ul>

 <li><strong>CS302 — Data Structures and Algorithms II</strong></li>

 <li><strong>(</strong><a href="http://www.cs.utk.edu/-plank)"><strong>http://www.cs.utk.edu/-plank)</strong></a></li>

 <li><strong>The original file: </strong><a href="http://www.cs.utk.edu/-plank/plank/classes/cs302/Labs/Lab5/"><strong>http://www.cs.utk.edu/-plank/plank/classes/cs302/Labs/Lab5/</strong></a><strong> (</strong><a href="http://www.cs.utk.edu/-plank/plank/classes/cs302/Labs/Lab5/)"><strong>http://www.cs.utk.edu/-plank/plank/classes/cs302/Labs/Lab5/)</strong></a></li>

</ul>

<strong>                                                                                                                                                                                                              </strong><strong>Project 03: Superball!</strong>

<strong>Superball is a simplistic game that was part of a games CD for Dr. Plank’s old Windows 95 box. It works as follows. You have a 8×10 grid which is the game board. Each cell of the game board may be empty or hold a color:</strong>

<ul>

 <li><strong>P – Purple: worth 2 points.</strong></li>

 <li><strong>B – Blue: worth 3 points.</strong></li>

 <li><strong>Y – Yellow: worth 4 points.</strong></li>

 <li><strong>R – Red: worth 5 points.</strong></li>

 <li><strong>G – Green: worth 6 points.</strong></li>

</ul>

<strong>The board starts with five random colors set. On your turn, you may do one of two things:</strong>

<ul>

 <li><strong>You may swap two cells. After the swap, five new random cells will be filled with a random colors.</strong></li>

 <li><strong>You may “score” a cell. To score a cell, the cell must be one of the “goal” cells, and there are sixteen of these, in rows 2-5, columns 0, 1, 8 and 9. (Everything is zero </strong><strong>indexed). Moreover, there must be at least five touching cells of the same color, one of which must be the goal cell that you want to score. When you score, you get the sum of the cells connected to the cell that you are scoring, and then all of those cells leave the board, and three new random ones are added.</strong></li>

</ul>

<strong>Dr. Plank has a tcl/tk/shell-scripted Superball player at /home/jplank/Superball. Simply copy that directory to your home directory: </strong><strong>UNIX&gt; cp </strong><strong>–</strong><strong>r /home/jplank/Superball $HOME</strong>

<strong>Then you can play it with —/Superball/Superball. The high score probably won’t work — you’ll have to change the open command in the file hscore to the name of your web </strong><strong>browser.</strong>

<strong>Let’s look at some screen shots. Suppose we fire up Superball:</strong>




<strong>                                                                                                                                                                                                                                                                                                                                         </strong><strong>Project 03: Superball!</strong>

The “goal” cells are marked with asterisks, and there are five non-empty cells. Our only legal action is to swap two cells — Dr. Plank swaps cells [3,6] and [5,8] below. This will make those two blue cells contiguous. In the game, we can do that by clicking on the two cells that we want to swap. Afterwards, five new cells are put on the screen. Here’s the screen shot:




<table>

 <tbody>

  <tr>

   <td width="732">

    <table width="100%">

     <tbody>

      <tr>

       <td> </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="348">

    <table width="100%">

     <tbody>

      <tr>

       <td></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="23">

    <table width="100%">

     <tbody>

      <tr>

       <td>,…….</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="28">

    <table width="100%">

     <tbody>

      <tr>

       <td><u>…r1 </u>·             <u>IL  L</u></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="11">

    <table width="100%">

     <tbody>

      <tr>

       <td>1 S</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="13">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong><em>._ A</em></strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="17">

    <table width="100%">

     <tbody>

      <tr>

       <td>.. 7 <sub>s</sub></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="19">

    <table width="100%">

     <tbody>

      <tr>

       <td>:<sup>fr</sup>.          .I</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="5">

    <table width="100%">

     <tbody>

      <tr>

       <td>•</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="21">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong>I</strong><strong>_le</strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="26">

    <table width="100%">

     <tbody>

      <tr>

       <td>L….</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="6">

    <table width="100%">

     <tbody>

      <tr>

       <td>,</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="27">

    <table width="100%">

     <tbody>

      <tr>

       <td>I I</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="40">

    <table width="100%">

     <tbody>

      <tr>

       <td><u>L</u><u>……,  </u> _</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="20">

    <table width="100%">

     <tbody>

      <tr>

       <td>I I I    I I I</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="162">

    <table width="100%">

     <tbody>

      <tr>

       <td><u>_ L IL</u>w.</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="44">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong>Empty: 70</strong><strong>Score: 0</strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="68">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong>( Collect )</strong>r<strong><u> High</u></strong><strong> Scores )</strong><strong>( </strong><strong><u>Start</u></strong><strong> Over )</strong>r <strong>Print Boards )</strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="53">

    <table width="100%">

     <tbody>

      <tr>

       <td><strong>Player Name</strong></td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<table>

 <tbody>

  <tr>

   <td width="13">

    <table width="100%">

     <tbody>

      <tr>

       <td>14</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>




<strong>Dr. Plank does a bunch more swaps and ends up with the following board:</strong>

<a href="https://web.eecs.utk.edui-semrich/ds20/assignments/proj03.html"><strong>https://web.eecs.utk.edui-semrich/ds20/assignments/proj03.html</strong></a><strong>                                                                                                                                                                                                                                   </strong>




Project 03: Superball!

<strong>We can score the green cells by clicking on cell [2,1], [3,0], [3,1] or [4,0] and then clicking “Collect”. This will score that group of eight green squares, which gets us 48 points (8*6), </strong><strong>and three new cells will be added:</strong>




<strong>                                                                                                                                                                                                                                                                                                                                         </strong><strong>Project 03: Superball!</strong>

<strong>There are no cells to score here (the blues ones in the lower right-hand part of the board only compose a group of four). So Dr. Plank now reverts to swapping. Suppose we keep doing this until we reach:</strong>

<strong>We’re in trouble. Dr. Plank has now got these beautiful groups of red, green and purple cells, but he can’t score any of them because they are not connected to a goal. Dang. We </strong><strong>can only score those two groups of blue cells. When Dr. Plank does that, he is only left with four open squares, and we can’t score anything:</strong>




<strong>                                                                                                                                                                                                                                                                                                                                      </strong><strong>Project 03: Superball!</strong>

<strong>Perhaps Dr. Plank should have been a little more thoughtful while playing the game. Regardless, he is stuck. We simply swap two random squares and end the game:</strong>




Project 03: Superball!

Oh well — should have done that swap a little sooner….

For this project, we are going to deal with a text-based version of the game. Our programs will have the following parameters:

<ul>

 <li><strong>rows – </strong>the number of rows on the game board. Although the tcl/tk version has that set to eight, our programs will handle any number.</li>

 <li><strong>cols – </strong>the number of columns on the game board.</li>

 <li><strong>min-score-size – </strong>the number of contiguous cells that have to be together in order to score them. This is 5 in the tcl/tk version</li>

 <li><strong>colors – </strong>this must be a string of distinct lower-case letters. They represent that the colors that a cell can have. The point value of the first of these is 2, and each succeeding character is worth one more point. To have the same values as the tcl/tk game, this parameter should be “pbyrg”.</li>

</ul>

Dr. Plank has written an interactive game player. Call it as shown below: UNIX&gt; <strong>cd /home/jplank/cs302/Labs/Lab5/</strong>

UNIX&gt; <strong>sb-player</strong>

usage: sb-player rows cols min-score-size colors player interactive(yln) output(yln) seed

UNIX&gt; <strong>sb-player 8 10 5 pbyrg – y y </strong>–

Empty Cells: 75            Score: 0

Your Move:

The format of the board is as follows: When a letter is capitalized, it is on a goal cell. Dots and asterisks stand for empty cells — asterisks are on the goal cells. If you click on the <strong>Print Boards </strong>button in the tcl/tk game, it will print out each board on standard output in that format. That’s nice for testing.

You can type two commands:

____ II

SWAP rl cl r2 c2 SCORE r c

In the board above, you can’t score anything, so you’ll have to swap. We’ll swap the blue cell in [2,2] with the green one in [7,2]:




<table>

 <tbody>

  <tr>

   <td width="731">

    <table width="100%">

     <tbody>

      <tr>

       <td> </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>

<strong>                                                                                                                                                                                                                                                                                                                                         </strong><strong>Project 03: Superball!</strong>

<strong>It’s incredibly tedious — play along with us:</strong>







<table>

 <tbody>

  <tr>

   <td width="129">Empty Cells: 70</td>

   <td width="42">Score:</td>

   <td width="20">0</td>

   <td width="130">Empty Cells: 65</td>

   <td width="42">Score:</td>

   <td width="21">0</td>

   <td width="129">Empty Cells: 60</td>

   <td width="42">Score:</td>

   <td width="21">0</td>

   <td width="126">Empty Cells: 55</td>

   <td width="45">Score:</td>

   <td width="21">0</td>

   <td width="129">Empty Cells: 50</td>

   <td width="42">Score:</td>

   <td width="22">0</td>

  </tr>

  <tr>

   <td width="129">.r…..</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130"><strong>.b……………… </strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">.b……….. <strong>p</strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">.b..r…pp</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">.r..rgy•pp</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129"> </td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130"> </td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">….<strong>g…….. </strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126"> </td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129"> </td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**g….b**</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">**g….bB*</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">**g.p..bB*</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">**g.p..bB*</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">**g.p..bB*</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**….b.**</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">**… <strong>. b.**</strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">**r…b.*R</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">**g…b.*R</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">**g…b.*B</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**<sub>.g….</sub>*y</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">P*.g….RY</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">P*.g….YY</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">P*.g….YY</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">P*.g….YY</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**…… *p… rr<strong><u>b </u></strong></td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">**…… <strong>*p</strong>.. rr<strong>.gry…………… </strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">**…… *P<strong>………… rr</strong><strong>.grr……………. </strong></td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126"><strong>**</strong><strong><sub>.</sub></strong><strong>g</strong><strong><sub>….</sub></strong><strong>*p</strong><strong>…..  </strong>rr…<strong>rrrr…………… </strong></td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">**<sub>.g….</sub>*pp…rrr…rrrr.p….</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">Your Move: <strong>SWAP 0 1</strong></td>

   <td width="42"><strong>7 2</strong></td>

   <td width="20"> </td>

   <td width="130">Your Move: <strong>SWAP 7 3</strong></td>

   <td width="42"><strong>4 8</strong></td>

   <td width="21"> </td>

   <td width="129">Your Move: <strong>SWAP </strong><strong>3 2</strong></td>

   <td width="42"><strong>7 1</strong></td>

   <td width="21"> </td>

   <td width="126">Your Move: <strong>SWAP </strong><strong>3 9</strong></td>

   <td width="45"><strong>0 1</strong></td>

   <td width="21"> </td>

   <td width="129">Your Move: <strong>SWAP 6 0</strong></td>

   <td width="42"><strong>0 1</strong></td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">Empty Cells: 45</td>

   <td width="42">Score:</td>

   <td width="20">0</td>

   <td width="130">Empty Cells: 40</td>

   <td width="42">Score:</td>

   <td width="21">0</td>

   <td width="129">Empty Cells: 35</td>

   <td width="42">Score:</td>

   <td width="21">0</td>

   <td width="126">Empty Cells: 30</td>

   <td width="45">Score:</td>

   <td width="21">0</td>

   <td width="129">Empty Cells: 37</td>

   <td width="42">Score:</td>

   <td width="22">50</td>

  </tr>

  <tr>

   <td width="129">.p..rgy.pp</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">.p..rgy•pp</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">.p..pgy•pp</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">.p.•pgy•pp</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">.p.•pgy•pp</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">.g..g…b.</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">.g..g…b.</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">.g..g.r.b.</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">.g.pg.b.b.</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">.g.pg.b.by</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**g.p..bB*</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">**g.p.pbB*</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">G*g.p.pbB*</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">G*g.p.pbB*</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">G*g.p.pbB*</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">**g…b.*B</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">R*g…by*B</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">R*g…by*B</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">R*g.r.by*B</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">R*g.r.byGB</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">P*.g..y.YY</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">P*.g..y.YY</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">P*.g..y.YY</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">P*pg..y.YY</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">P*pg..y.YY</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129"><strong>**</strong><strong><sub>.</sub></strong><strong>g</strong><strong><sub>..</sub></strong><strong>yp*p</strong>r…rrr…rrrr.py…</td>

   <td width="42"> </td>

   <td width="20"> </td>

   <td width="130">P*.g..yp*Yr…rrrb..rrrr.pp…</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="129">R*.g..yp*Yr..grrrb..rrrrbppy..</td>

   <td width="42"> </td>

   <td width="21"> </td>

   <td width="126">R*.g.bypBYr..grrrbrrrrrppy</td>

   <td width="45"> </td>

   <td width="21"> </td>

   <td width="129">**.g.bypBY…g…b..-1<sup>)</sup>..-PPY–</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

  <tr>

   <td width="129">Your Move: <strong>SWAP 5 9</strong></td>

   <td width="42"><strong>7 </strong><strong>6</strong></td>

   <td width="20"> </td>

   <td width="130">Your Move: <strong>SWAP </strong><strong>5 0</strong></td>

   <td width="42"><strong>0 4</strong></td>

   <td width="21"> </td>

   <td width="129">Your Move: <strong>SWAP </strong><strong>7 4</strong></td>

   <td width="42"><strong>1 6</strong></td>

   <td width="21"> </td>

   <td width="126">Your Move: <strong>SCORE 5</strong></td>

   <td width="45"><strong>0</strong></td>

   <td width="21"> </td>

   <td width="129">Your Move:</td>

   <td width="42"> </td>

   <td width="22"> </td>

  </tr>

 </tbody>

</table>




<strong>                                                                                                                                                                                                                                                                                                                                           </strong><strong>Project 03: Superball!</strong>

<strong>Program #1: Sb-read</strong>

Dr. Plank has provided <strong>sb-read.cpp (</strong><a href="http://www.cs.utk.eduNplank/plank/classesics302/Labs/Lab5/sb-read.cpp)"><strong>http://www.cs.utk.eduNplank/plank/classesics302/Labs/Lab5/sb-read.cpp)</strong></a> for us. This program takes the four parameters detailed above, reads in a game board with those parameters and prints out some very basic information. For example, the following board:

May be represented by the following text (in <strong>input-1.bct (</strong><a href="http://www.cs.utk.eduNplankiplank/classes/cs302/Labs/Lab5/input-1.bct)):"><strong>http://www.cs.utk.eduNplankiplank/classes/cs302/Labs/Lab5/input-1.bct)):</strong></a>

<ul>

 <li><strong>••)</strong><strong><sup>(</sup></strong><strong>YrYY•1</strong><strong><sup>3</sup></strong> <strong>y.rg•yppyp </strong><strong>**gg.yrpPP </strong><strong>GGgbgybp** </strong><strong>R*bg.yrp*P </strong><strong>G*gygyypY* </strong><strong>yyybpby.pb </strong><strong>.pgg.yp•bb</strong></li>

</ul>

When we run <strong>sb-read </strong>on it, we get the following:




<strong>                                                                                                                                                                                                                                                                                                                                           </strong><strong>Project 03: Superball!</strong>

UNIX&gt; <strong>sb-read 8 10 5 pbyrg &lt; input-1.txt</strong>

Empty cells:                                 20

Non-Empty cells:                           60

Number of pieces in goal cells: 8 Sum of their values: 33 UNIX&gt;

There are three purple pieces in goal cells, one yellow, three green and one red. That makes a total of 32 + 4 + 5 + 3*6 = 33.

You should take a look at <strong>sb-read.cpp (</strong><a href="http://www.cs.utk.eduNplankiplank/classes/cs302/Labs/Lab5/sb-read.cpp)"><strong>http://www.cs.utk.eduNplankiplank/classes/cs302/Labs/Lab5/sb-read.cpp)</strong></a><strong>. </strong>In particular, look at the <strong>Superball </strong>class:

<table>

 <tbody>

  <tr>

   <td width="251">class Superball {public:Superball(int argc, char **argv); int r;int c;int mss;int empty;vector &lt;int&gt; board; vector &lt;int&gt; goals; vector &lt;int&gt; colors;}.;</td>

  </tr>

 </tbody>

</table>

<strong>Mss </strong>is min-score-size. <strong>Empty </strong>is the number of empty cells in the board. <strong>Board </strong>is a vector of <strong>r* c </strong>integers. The element in [i,j] is in entry <strong>board[i*c+j], </strong>and is either ‘.’,'”‘ or a lower case letter. <strong>goals </strong>is another array of <strong>r* c </strong>integers. It is equal to 0 if the cell is not a goal cell, and 1 if it is a goal cell. <strong>Colors </strong>is an array of 256 elements, which should be indexed by a letter. Its value is the value of the letter (e.g. in the above example, <strong>colors[‘p’] = 2).</strong>

<strong>sb-read </strong>does all manner of error checking for you. It is a nice program from which to build your other programs.

<strong>Program #2: Sb-analyze</strong>

You are to write this one.

With <strong>sb-analyze, </strong>you are to start with <strong>sb-read.cpp </strong>as a base, and augment it so that it prints out all possible scoring sets. For example, in the above game board (represented by <strong>input-1.txt (</strong><a href="http://www.cs.utk.eduNplank/plankiclasses/cs302/Labs/Lab5/input-tbct)),"><strong>http://www.cs.utk.eduNplank/plankiclasses/cs302/Labs/Lab5/input-tbct)),</strong></a> there are two scoring sets — the set of 10 purple cells in the upper right-hand corner, and the set of 6 green cells on the left side of the screen. Here is the output to <strong>sb_analyze:</strong>




<strong>                                                                                                                                                                                                                                                                                                                                            </strong><strong>Project 03: Superball!</strong>




UNIX&gt; <strong>sb-analyze</strong>

usage: sb-analyze rows cols min-score-size colors

UNIX&gt; <strong>sb</strong><strong>–</strong><strong>analyze 8 10 5 pbyrg &lt; input</strong><strong>–</strong><strong>1.txt </strong>Scoring sets:

Size: 10 Char: p Scoring Cell: 2,8 Size: 6 Char: g Scoring Cell: 3,0 UNIX&gt;

Each set must be printed exactly once, but in any order, and with any legal goal cell. Thus, the following output would also be ok:

UNIX&gt; <strong>sb-analyze 8 10 5 pbyrg &lt; input-1.txt </strong>Scoring sets:

Size: 6 Char: g Scoring Cell: 3,1 Size: 10 Char: p Scoring Cell: 2,9 UNIX&gt;

Think about how you would use the disjoint sets data structure to implement this — it is a straightforward connected components application. We would recommend augmenting your <strong>Superball </strong>class with a <strong>DisjointSet, </strong>and then having a method called <strong>analyze_superball() </strong>that performs the analysis.

Here’s another example:










This is in the file <strong>input-2.txt (</strong><a href="http://www.cs.utk.edui"><strong>http://www.cs.utk.edui</strong></a><strong>—jplank/plank/classes/cs302/Labs/Lab5/input-2.txt):</strong>




<strong>7/12/2020                                                                                                                                                                                                                                                                                                                                           </strong><strong>Project 03: Superball!</strong>

yyggyryybp ggrgpyppyp RBgggyrpPP GGgggybpPP RGygryrpBP YGyygyypYB yyybpbyppb ppggyypbbb

UNIX&gt; <strong>sb-analyze 8 10 5 pbyrg &lt; input-2.txt</strong>

<table>

 <tbody>

  <tr>

   <td width="71">Scoring</td>

   <td colspan="2" width="60">sets:</td>

   <td width="16"> </td>

   <td width="88"> </td>

   <td width="729"> </td>

  </tr>

  <tr>

   <td width="71">Size:</td>

   <td width="22">14</td>

   <td width="39">Char:</td>

   <td width="16">g</td>

   <td width="88">Scoring Cell:</td>

   <td width="729">5,1</td>

  </tr>

  <tr>

   <td width="71">Size:</td>

   <td width="22">15</td>

   <td width="39">Char:</td>

   <td width="16">p</td>

   <td width="88">Scoring Cell:</td>

   <td width="729">4,9</td>

  </tr>

  <tr>

   <td width="71">Size:</td>

   <td width="22">7</td>

   <td width="39">Char:</td>

   <td width="16">y</td>

   <td width="88">Scoring Cell:</td>

   <td width="729">5,0</td>

  </tr>

  <tr>

   <td width="71">Size:</td>

   <td width="22">5</td>

   <td width="39">Char:</td>

   <td width="16">b</td>

   <td width="88">Scoring Cell:</td>

   <td width="729">5,9</td>

  </tr>

  <tr>

   <td width="71">UNIX&gt;</td>

   <td width="22"> </td>

   <td width="39"> </td>

   <td width="16"> </td>

   <td width="88"> </td>

   <td width="729"> </td>

  </tr>

 </tbody>

</table>




<strong>Program #3: Sb-play</strong>

Your next program takes the same arguments and input as <strong>sb-analyze. </strong>However, now its job is to print a single move as would be accepted as input for the <strong>sb-player </strong>program. In other words, it needs to output a SWAP or SCORE line with legal values.

If you have fewer than five pieces and cannot score any, you will lose the game — you should do that by swapping two legal pieces so that the game can end.

The <strong>sb-player </strong>program takes as its 5th argument the name of a program that it will use for input. Dr. Plank also also provided three programs – <strong>sb-play, sb-play2 </strong>and <strong>sb-play3 </strong>in that directory. <strong>sb-play </strong>simply swaps two random cells until there are fewer than five empty, then it scores a set if it can. The other two are smarter, but are by no means the best one can do.

Here’s <strong>sb-player </strong>running on <strong>sb-play2 </strong>(note, <strong>sb-player </strong>creates a temporary file, so you must run it from your own directory):

UNIX&gt; <strong>/home/jplank/cs302/Labs/Lab5/sb-player 8 10 5 pbyrg /home/jplank/cs302/Labs/Lab5/sb-play2 y y </strong>-Empty Cells: 75         Score: 0




g

* *

<strong>*Pr……….. </strong>

<strong>** . . p . . . **</strong>

<strong><u>b </u></strong>




Type Return for the next play




<strong>                                                                                                                                                                                                                                                                                                                                              </strong><strong>Project 03: Superball!</strong>

It waits for you to press the return key. When you do so, it will send the game board to <strong>/home/jplank/cs302/Labs/Lab5/sp-play2 </strong>and perform the output. Here’s what happens: <strong>Move is: SWAP 5 4 3 2</strong>

<strong>Empty Cells: 70               </strong><strong>Score: 0</strong>

<strong>g…………….. g</strong>

<strong>…………… Y</strong>

<strong>**……………. **</strong>

<strong>*p<sub>p……………………… </sub>**</strong>

<strong>**………….. G*</strong>

<strong>**.. r……….. **</strong>

.<strong>.g                <u>b </u></strong>

<strong>………… g.</strong>

<strong>Type Return for the next play</strong>

You can bet that the next move will swap that <strong>b </strong>with one of the g’s: <strong>Move </strong><strong>is: SWAP 6 8 0 0</strong>

<strong>Empty Cells: 65               </strong><strong>Score: 0</strong>

<strong>Type Return for the next play</strong>

And so on. <strong>If </strong>you run it with <strong>n </strong>for the 6th argument, it will simply run the program without your input:




<strong>                                                                                                                                                                                                                                                                                                                                          </strong><strong>Project 03: Superball!</strong>

UNIX&gt; <strong>/home/jplank/cs302/Labs/Lab5/sb-player 8 10 5 pbyrg /home/jplank/cs302/Labs/Lab5/sb-play2 n y </strong>-Empty Cells: 75      Score: 0

<strong>**y</strong><strong><sub>..</sub></strong><strong>y</strong><strong><sub>..</sub></strong><strong>**</strong><strong>**      **</strong>

<strong>*p………….. **</strong>

p•g•

Move is: SWAP 3 5 3 2

<em>… a bunch of output skipped…</em>

Empty Cells: 1        Score: 505

yyrrgggpyy grrbppg.yg GYbgygggPB GBggpgbpPB PPgggggrYB YBbybgpbYR pprrrggggr byyrppppgg

Move is: SWAP 0 1 7 5

Game over. Final score = 505 UNIX&gt;

<strong>Even though there were no good moves at the end, the program did a final SWAP so that the game could finish.</strong>

<strong>If you run with the 7th argument as </strong><strong>n, </strong><strong>it will only print out the end result, and the last argument can specify a seed (it uses the current time if that argument is “-“), so that you can </strong><strong>compare multiple players on the same game:</strong>

<table>

 <tbody>

  <tr>

   <td width="307">UNIX&gt; <strong>/home/jplank/cs302/Labs/Lab5/sb-player 8 </strong>Game over. Final score = 0UNIX&gt; <strong>/home/jplank/cs302/Labs/Lab5/sb</strong><strong>–</strong><strong>player 8 </strong>Game over. Final score = 855UNIX&gt; <strong>/home/jplank/cs302/Labs/Lab5/sb</strong><strong>–</strong><strong>player 8 </strong>Game over. Final score = 2572UNIX&gt;</td>

   <td width="657"><strong>10 5 pbyrg /home/jplank/cs302/Labs/Lab5/sb-play n n 1 </strong><strong>10 5 pbyrg /home/jplank/cs302/Labs/Lab5/sb-play2 n n 1 10 5 pbyrg /home/jplank/cs302/Labs/Lab5/sb-play3 n n 1</strong></td>

  </tr>

 </tbody>

</table>




Project 03: Superball!

It can take a while for these to run — if it appears to be hanging, send the process a <strong>QUIT </strong>signal and it will print out what the current score is.

<strong>Shell Script to Run Multiple Times</strong>

The file <strong>run_multiple.sh (</strong><a href="http://www.cs.utk.edui"><strong>http://www.cs.utk.edui</strong></a><strong>—jplankiplank/classes/cs302/Labs/Lab5/run_multiple.sh) </strong>is a shell script to run the player on multiple seeds and average the results. Examples:

UNIX&gt; <strong>sh run_multiple.sh</strong>

usage: sh run_multiple.sh r c mss colors player nruns starting_seed

UNIX&gt; <strong>sh run_multiple.sh 8 10 5 pbyrg sb</strong><strong>–</strong><strong>play 10 1</strong>

<table>

 <tbody>

  <tr>

   <td width="51">Run</td>

   <td width="28">1 –</td>

   <td width="60">Score:</td>

   <td width="40">38</td>

   <td width="71">– Average</td>

   <td width="713">38.000</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">2 –</td>

   <td width="60">Score:</td>

   <td width="40">0</td>

   <td width="71">– Average</td>

   <td width="713">19.000</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">3 –</td>

   <td width="60">Score:</td>

   <td width="40">0</td>

   <td width="71">– Average</td>

   <td width="713">12.667</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">4 –</td>

   <td width="60">Score:</td>

   <td width="40">57</td>

   <td width="71">– Average</td>

   <td width="713">23.750</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">5 –</td>

   <td width="60">Score:</td>

   <td width="40">0</td>

   <td width="71">– Average</td>

   <td width="713">19.000</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">6</td>

   <td width="60">–  Score:</td>

   <td width="40">0</td>

   <td width="71">– Average</td>

   <td width="713">15.833</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">7</td>

   <td width="60">–  Score:</td>

   <td width="40">89</td>

   <td width="71">– Average</td>

   <td width="713">26.286</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">8</td>

   <td width="60">– Score:</td>

   <td width="40">15</td>

   <td width="71">– Average</td>

   <td width="713">24.875</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">9</td>

   <td width="60">– Score:</td>

   <td width="40">0</td>

   <td width="71">– Average</td>

   <td width="713">22.111</td>

  </tr>

  <tr>

   <td width="51">Run</td>

   <td width="28">10</td>

   <td width="60">– Score:</td>

   <td width="40">20</td>

   <td width="71">– Average</td>

   <td width="713">21.900</td>

  </tr>

 </tbody>

</table>

UNIX&gt; <strong>sh run_multiple.sh 8 10 5 pbyrg sb</strong><strong>–</strong><strong>play2 10 1</strong>

<table>

 <tbody>

  <tr>

   <td width="52">Run</td>

   <td width="27">1 –</td>

   <td width="54">Score:</td>

   <td width="46">855</td>

   <td width="65">– Average</td>

   <td width="719">855.000</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">2 –</td>

   <td width="54">Score:</td>

   <td width="46">979</td>

   <td width="65">– Average</td>

   <td width="719">917.000</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">3 –</td>

   <td width="54">Score:</td>

   <td width="46">650</td>

   <td width="65">– Average</td>

   <td width="719">828.000</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">4 –</td>

   <td width="54">Score:</td>

   <td width="46">833</td>

   <td width="65">– Average</td>

   <td width="719">829.250</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">5</td>

   <td width="54">– Score:</td>

   <td width="46">832</td>

   <td width="65">– Average</td>

   <td width="719">829.800</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">6</td>

   <td width="54">– Score:</td>

   <td width="46">3326</td>

   <td width="65">– Average</td>

   <td width="719">1245.833</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">7</td>

   <td width="54">– Score:</td>

   <td width="46">1507</td>

   <td width="65">– Average</td>

   <td width="719">1283.143</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27"><strong>8</strong></td>

   <td width="54"><strong>– </strong>Score:</td>

   <td width="46">3643</td>

   <td width="65">– Average</td>

   <td width="719">1578.125</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">9</td>

   <td width="54">– Score:</td>

   <td width="46">610</td>

   <td width="65">– Average</td>

   <td width="719">1470.556</td>

  </tr>

  <tr>

   <td width="52">Run</td>

   <td width="27">10</td>

   <td width="54">– Score:</td>

   <td width="46">862</td>

   <td width="65">– Average</td>

   <td width="719">1409.700</td>

  </tr>

 </tbody>

</table>

UNIX&gt; <strong>sh run_multiple.sh 8 10 5 pbyrg sb</strong><strong>–</strong><strong>play3 10 1</strong>

<table>

 <tbody>

  <tr>

   <td width="59">Run</td>

   <td width="21">1 –</td>

   <td width="54">Score:</td>

   <td width="46">2572</td>

   <td width="65">– Average</td>

   <td width="718">2572.000</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">2 –</td>

   <td width="54">Score:</td>

   <td width="46">2708</td>

   <td width="65">– Average</td>

   <td width="718">2640.000</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">3 –</td>

   <td width="54">Score:</td>

   <td width="46">745</td>

   <td width="65">– Average</td>

   <td width="718">2008.333</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">4 –</td>

   <td width="54">Score:</td>

   <td width="46">424</td>

   <td width="65">– Average</td>

   <td width="718">1612.250</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">5</td>

   <td width="54">–  Score:</td>

   <td width="46">1888</td>

   <td width="65">– Average</td>

   <td width="718">1667.400</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">6</td>

   <td width="54">–  Score:</td>

   <td width="46">7140</td>

   <td width="65">– Average</td>

   <td width="718">2579.500</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">7</td>

   <td width="54">– Score:</td>

   <td width="46">3475</td>

   <td width="65">– Average</td>

   <td width="718">2707.429</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">8</td>

   <td width="54">– Score:</td>

   <td width="46">1701</td>

   <td width="65">– Average</td>

   <td width="718">2581.625</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">9</td>

   <td width="54">– Score:</td>

   <td width="46">2699</td>

   <td width="65">– Average</td>

   <td width="718">2594.667</td>

  </tr>

  <tr>

   <td width="59">Run</td>

   <td width="21">10</td>

   <td width="54">–  Score:</td>

   <td width="46">2291</td>

   <td width="65">– Average</td>

   <td width="718">2564.300</td>

  </tr>

  <tr>

   <td width="59">UNIX&gt;</td>

   <td width="21"> </td>

   <td width="54"> </td>

   <td width="46"> </td>

   <td width="65"> </td>

   <td width="718"> </td>

  </tr>

 </tbody>

</table>




Obviously, <strong>to get a meaningful average, many more runs (than 10) will be required.</strong>




<strong>                                                                                                                                                                                                                                                                                                                                           </strong><strong>Project 03: Superball!</strong>

Oh, and make your programs run in reasonable time. Roughly 5 seconds for every thousand points, and if you are burning all that time, your program better be killing Dr. Plank’s….

<strong>The Superball Challenge</strong>

To get credit, your player needs to average over 100 points on runs of 100 games.

We will run a Superball tournament with all of your players with extra lab points going to the winners:

<ul>

 <li>1st place: 20 extra lab points.</li>

 <li>2nd place: 10 extra lab points.</li>

 <li>3rd place: 5 extra lab points.</li>

</ul>

Dr. Plank and I have previously performed the challenge eight times:

<ul>

 <li>CS140 in 2007.</li>

 <li>CS302 in 2010.</li>

 <li>CS302 in 2011.</li>

 <li>CS302 in 2012.</li>

 <li>CS302 in 2013.</li>

 <li>CS302 in 2014.</li>

 <li>CS302 in 2015.</li>

 <li>CS302 in 2018.</li>

 <li>CS302 in 2019 (SJE)</li>

</ul>

Here’s the Superball Challenge Hall Of Fame (scores over 650):

<table>

 <tbody>

  <tr>

   <td width="33"><strong>Rank</strong></td>

   <td width="52"><strong>Average</strong></td>

   <td width="104"><strong>Name</strong></td>

   <td width="115"><strong>Semester</strong></td>

  </tr>

  <tr>

   <td width="33">1</td>

   <td width="52">31814.13</td>

   <td width="104">Grant Bruer</td>

   <td width="115">CS302, Fall, 2015</td>

  </tr>

  <tr>

   <td width="33">2</td>

   <td width="52">24278.49</td>

   <td width="104">Alexander Teepe</td>

   <td width="115">CS302, Fall, 2015</td>

  </tr>

  <tr>

   <td width="33">3</td>

   <td width="52">17367.77</td>

   <td width="104">Joseph Connor</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">4</td>

   <td width="52">17021.37</td>

   <td width="104">Cory Walker</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">5</td>

   <td width="52">16963.40</td>

   <td width="104">Seth Kitchens</td>

   <td width="115">CS302, Fall, 2015</td>

  </tr>

  <tr>

   <td width="33">6</td>

   <td width="52">14555.83</td>

   <td width="104">Ben Arnold (Tie)</td>

   <td width="115">CS302, Fall, 2012</td>

  </tr>

  <tr>

   <td width="33">7</td>

   <td width="52">14555.83</td>

   <td width="104">Adam Disney (Tie)</td>

   <td width="115">CS302, Fall, 2011</td>

  </tr>

  <tr>

   <td width="33">8</td>

   <td width="52">13657.79</td>

   <td width="104">Isaak Sikkema</td>

   <td width="115">CS302, Fall, 2018</td>

  </tr>

  <tr>

   <td width="33">9</td>

   <td width="52">12963.47</td>

   <td width="104">Jake Davis          ,</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">10</td>

   <td width="52">12634.29</td>

   <td width="104">Jake Lamberson</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">11</td>

   <td width="52">11722.05</td>

   <td width="104">Parker Mitchell</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">12</td>

   <td width="52">11418.77</td>

   <td width="104">James Pickens</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">13</td>

   <td width="52">11380.74</td>

   <td width="104">Nathan Ziebart</td>

   <td width="115">CS302, Fall, 2011</td>

  </tr>

  <tr>

   <td width="33">14</td>

   <td width="52">11291.39</td>

   <td width="104">Michael Jugan</td>

   <td width="115">CS302, Fall, 2010</td>

  </tr>

  <tr>

   <td width="33">15</td>

   <td width="52">10576.96</td>

   <td width="104">Tyler Shields</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

  <tr>

   <td width="33">16</td>

   <td width="52">8770.67</td>

   <td width="104">Nathan Swartz</td>

   <td width="115">S302, Spring, 2019</td>

  </tr>

  <tr>

   <td width="33">17</td>

   <td width="52">7475.07</td>

   <td width="104">Jared Smith</td>

   <td width="115">CS302, Fall, 2014</td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td width="33"><strong>18</strong></td>

   <td width="52"><strong>7216.28</strong></td>

   <td width="104"><strong>_</strong><strong>Michael Bowie</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>19</strong></td>

   <td width="52"><strong>7003.56</strong></td>

   <td width="104"><strong>Andrew LaPrise</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>20</strong></td>

   <td width="52"><strong>6100.28</strong></td>

   <td width="104"><strong>Chris Nagy</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>21</strong></td>

   <td width="52"><strong>5467.56</strong></td>

   <td width="104"><strong>Tyler Marshall</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>22</strong></td>

   <td width="52"><strong>5262.80</strong></td>

   <td width="104"><strong>Harry Channing</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>23</strong></td>

   <td width="52"><strong>5116.13</strong></td>

   <td width="104"><strong>Kyle Bashour</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>24</strong></td>

   <td width="52"><strong>4808.03</strong></td>

   <td width="104"><strong>Matt Baumgartner</strong></td>

   <td width="115"><strong>CS302, Fall, 2010</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>25</strong></td>

   <td width="52"><strong>4586.51</strong></td>

   <td width="104"><strong>Jeramy Harrison</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>26</strong></td>

   <td width="52"><strong>4531.96</strong></td>

   <td width="104"><strong>Philip Hicks</strong></td>

   <td width="115"><strong>CS302, Spring, 2019</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>27</strong></td>

   <td width="52"><strong>4057.08</strong></td>

   <td width="104"><strong>Phillip McKnight</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>28</strong></td>

   <td width="52"><strong>3882.53</strong></td>

   <td width="104"><strong>Pranshu Bansal</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>29</strong></td>

   <td width="52"><strong>3882.28</strong></td>

   <td width="104"><strong>Kemal Fidan</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>30</strong></td>

   <td width="52"><strong>3852.87</strong></td>

   <td width="104"><strong>Yaohung Tsai</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>31</strong></td>

   <td width="52"><strong>3849.24</strong></td>

   <td width="104"><strong>Chris Richardson</strong></td>

   <td width="115"><strong>CS302, Fall, 2010</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>32</strong></td>

   <td width="52"><strong>3809.41</strong></td>

   <td width="104"><strong>Arthur Vidineyev</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>33</strong></td>

   <td width="52"><strong>3588.35</strong></td>

   <td width="104"><strong>Kevin Dunn</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>34</strong></td>

   <td width="52"><strong>3464.83</strong></td>

   <td width="104"><strong>Patrick Slavick</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>35</strong></td>

   <td width="52"><strong>3436.21</strong></td>

   <td width="104"><strong>sb-play3</strong></td>

   <td width="115"><strong>CS140, Fall, 2007</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>36</strong></td>

   <td width="52"><strong>3400.50</strong></td>

   <td width="104"><strong>Kody Bloodworth</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>37</strong></td>

   <td width="52"><strong>3080.15</strong></td>

   <td width="104"><strong>Andrew Messing</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>38</strong></td>

   <td width="52"><strong>2903.38</strong></td>

   <td width="104"><strong>Adam LaClair</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>39</strong></td>

   <td width="52"><strong>2555.36</strong></td>

   <td width="104"><strong>Mohammad Fathi</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>40</strong></td>

   <td width="52"><strong>2532.89</strong></td>

   <td width="104"><strong>Trevor Sharpe</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>41</strong></td>

   <td width="52"><strong>2521.44</strong></td>

   <td width="104"><strong>Justus Camp</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>42</strong></td>

   <td width="52"><strong>2335.88</strong></td>

   <td width="104"><strong>Mark Clark</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>43</strong></td>

   <td width="52"><strong>2307.16</strong></td>

   <td width="104"><strong>John Burnum</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>44</strong></td>

   <td width="52"><strong>2205.17</strong></td>

   <td width="104"><strong>Shawn Cox</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>45</strong></td>

   <td width="52"><strong>2163.70</strong></td>

   <td width="104"><strong>Alex Wetherington</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>46</strong></td>

   <td width="52"><strong>2134.99</strong></td>

   <td width="104"><strong>Julian Kohann</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>47</strong></td>

   <td width="52"><strong>2011.38</strong></td>

   <td width="104"><strong>Wells Phillip</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>48</strong></td>

   <td width="52"><strong>1919.72</strong></td>

   <td width="104"><strong>Ravi Patel</strong></td>

   <td width="115"><strong>CS302, spring, 2019</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>49</strong></td>

   <td width="52"><strong>1778.83</strong></td>

   <td width="104"><strong>Keith Clinart</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>50</strong></td>

   <td width="52"><strong>1740.19</strong></td>

   <td width="104"><strong>Luke Bechtel</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>51</strong></td>

   <td width="52"><strong>1634.49</strong></td>

   <td width="104"><strong>William Brummette</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>52</strong></td>

   <td width="52"><strong>1602.83</strong></td>

   <td width="104"><strong>Forrest Sable</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>53</strong></td>

   <td width="52"><strong>1470.84</strong></td>

   <td width="104"><strong>Christopher Tester</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>54</strong></td>

   <td width="52"><strong>1433.48</strong></td>

   <td width="104"><strong>Xiao Zhou</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>55</strong></td>

   <td width="52"><strong>1430.54</strong></td>

   <td width="104"><strong>Jonathan Burns</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>56</strong></td>

   <td width="52"><strong>1340.32</strong></td>

   <td width="104"><strong>John Murray</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>57</strong></td>

   <td width="52"><strong>1329.34</strong></td>

   <td width="104"><strong>Benjamin Brock</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>58</strong></td>

   <td width="52"><strong>1257.56</strong></td>

   <td width="104"><strong>Dylan Lee</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

 </tbody>

</table>




<strong>7/12/2020                                                                                                                                                                                                                                                                                                                                              </strong><strong>Project 03: Superball!</strong>

<table>

 <tbody>

  <tr>

   <td width="33"><strong>59</strong></td>

   <td width="52"><strong>1202.06</strong></td>

   <td width="104"><strong>_</strong><strong>Bandara</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>60</strong></td>

   <td width="52"><strong>1149.80</strong></td>

   <td width="104"><strong>Will Houston</strong></td>

   <td width="115"><strong>CS302, Fall, 2010</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>61</strong></td>

   <td width="52"><strong>1119.85</strong></td>

   <td width="104"><strong>Kevin Chiang</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>62</strong></td>

   <td width="52"><strong>1096.48</strong></td>

   <td width="104"><strong>Daniel Cash</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>63</strong></td>

   <td width="52"><strong>1059.91</strong></td>

   <td width="104"><strong>Kaleb McClure</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>64</strong></td>

   <td width="52"><strong>1058.26</strong></td>

   <td width="104"><strong>sb-play2</strong></td>

   <td width="115"><strong>CS140, Fall, 2007</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>65</strong></td>

   <td width="52"><strong>1029.63</strong></td>

   <td width="104"><strong>Lydia San George</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>66</strong></td>

   <td width="52"><strong>972.36</strong></td>

   <td width="104"><strong>Erik Rutledge</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>67</strong></td>

   <td width="52"><strong>959.79</strong></td>

   <td width="104"><strong>Daniel Nichols</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>68</strong></td>

   <td width="52"><strong>917.92</strong></td>

   <td width="104"><strong>Vasu Kalaria</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>69</strong></td>

   <td width="52"><strong>908.09</strong></td>

   <td width="104"><strong>Chris Rains</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>70</strong></td>

   <td width="52"><strong>875.44</strong></td>

   <td width="104"><strong>Allen McBride</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>71</strong></td>

   <td width="52"><strong>840.94</strong></td>

   <td width="104"><strong>Spencer Howell</strong></td>

   <td width="115"><strong>CS302, Fall, 2018</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>72</strong></td>

   <td width="52"><strong>830.79</strong></td>

   <td width="104"><strong>David Cunningham</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>73</strong></td>

   <td width="52"><strong>810.17</strong></td>

   <td width="104"><strong>Collin Bell</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>74</strong></td>

   <td width="52"><strong>763.58</strong></td>

   <td width="104"><strong>Jacob Lambert</strong></td>

   <td width="115"><strong>CS302, Fall, 2013</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>75</strong></td>

   <td width="52"><strong>703.67</strong></td>

   <td width="104"><strong>Scott Marcus</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>76</strong></td>

   <td width="52"><strong>703.00</strong></td>

   <td width="104"><strong>Don Lopez</strong></td>

   <td width="115"><strong>CS140, Fall, 2007</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>77</strong></td>

   <td width="52"><strong>700.90</strong></td>

   <td width="104"><strong>Tony Abston</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>78</strong></td>

   <td width="52"><strong>682.56</strong></td>

   <td width="104"><strong> Jackson Collier   </strong><strong>‘</strong></td>

   <td width="115"><strong>CS302, Fall, 2014</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>79</strong></td>

   <td width="52"><strong>677.83</strong></td>

   <td width="104"><strong>KC Bentjen</strong></td>

   <td width="115"><strong>CS302, Fall, 2011</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>80</strong></td>

   <td width="52"><strong>665.60</strong></td>

   <td width="104"><strong>Joshua Clark</strong></td>

   <td width="115"><strong>CS302, Fall, 2012</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>81</strong></td>

   <td width="52"><strong>659.96</strong></td>

   <td width="104"><strong>Warren Dewit</strong></td>

   <td width="115"><strong>CS302, Fall, 2010</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>82</strong></td>

   <td width="52"><strong>654.67</strong></td>

   <td width="104"><strong>Coburn Brandon</strong></td>

   <td width="115"><strong>CS302, Fall, 2015</strong></td>

  </tr>

  <tr>

   <td width="33"><strong>83</strong></td>

   <td width="52"><strong>650.98</strong></td>

   <td width="104"><strong>Joaquin Bujalance</strong></td>

   <td width="115"><strong>CS140, Fall, 2007</strong></td>

  </tr>

 </tbody>

</table>




<strong>Hints</strong>

<strong>Play the game for a bit to try to figure out some strategies. However, one good way to write a game player is to figure out a way to come up with a rating for a game board. Then when you are faced with making a move, you analyze all potential moves by trying them out and choosing the one that gives you the resulting board with the highest rating.</strong>