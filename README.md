Download Link: https://assignmentchef.com/product/solved-comp-352-data-structure-and-algorithms-assignment-1
<br>
<strong> </strong>

Computer Science and Software Engineering

Question 1

<strong> </strong>

<ol>

 <li>Given an array A of integers of any size, n ≥ 0, write an algorithm as a pseudo code (not a program!) that would find out the total number and their sum of even positive numbers as well as the total number and their sum of odd positive numbers in the array. For instance, assume that array A is as follows:</li>

</ol>




<table width="600">

 <tbody>

  <tr>

   <td width="59">5</td>

   <td width="59">-2</td>

   <td width="59">4</td>

   <td width="59">9</td>

   <td width="61">-250</td>

   <td width="60">99</td>

   <td width="61">108</td>

   <td width="60">-62</td>

   <td width="60">46</td>

   <td width="60">13</td>

  </tr>

 </tbody>

</table>




The algorithm would find the number of positive even numbers is 3 and their sum is 4+108+46=158 and the number of positive odd numbers is 4 and their sum is 5+9+99+13=126. Your algorithm must handle possible special cases. Finally, the algorithm must use the smallest auxiliary /additional storage to perform what is needed.




<ol>

 <li>What is the time complexity of your algorithm, in terms of Big-O?</li>

</ol>




<ol>

 <li>What is the space complexity of your algorithm, in terms of Big-O?</li>

</ol>




<h1>Question 2</h1>




Prove or disprove the following statements, using the relationship among typical growth-rate functions discussed in class:




<ol>

 <li>45 n<sup>2</sup> + 28 n + 752 is Ω(n)</li>

</ol>




<ol>

 <li>256 n + 8 n log n is Θ(log n)</li>

</ol>




<ol>

 <li>n<sup>8</sup> + log n is O(log n)</li>

</ol>




<ol>

 <li>2 n<sup>2</sup> log n + n<sup>3 </sup>is Θ(log n)</li>

</ol>




<ol>

 <li>4 n log<sup>2</sup> n + 3 n<sup>2</sup> log n is O(log n)</li>

</ol>




<ol>

 <li>n<sup>7</sup> + 0.00000001n<sup>6</sup> is Ω(n<sup>6</sup>)</li>

</ol>

<strong> </strong>




<h1>Question 3</h1>

<strong> </strong>

Consider the following algorithm: <strong> </strong>

<strong> </strong>

<strong>Algorithm <em>arraySpecialSum</em>(<em>A</em>, <em>n</em>) </strong>

<strong>     </strong>

<em>currentMax</em>  <em>A</em>[0]                               for <em>i</em>  1 to <em>n</em> − 1 do                       if <em>A</em>[<em>i</em>]  <em>currentMax</em> then                   <em>currentMax</em>  <em>A</em>[<em>i</em>]                    { increment counter <em>i</em> }




CurrentMaxOccurence = 0         for <em>i</em>  0 to <em>n</em> − 1 do                        if <em>A</em>[<em>i</em>] == <em>currentMax</em> then                      { increment <em>currentMaxOccurence</em>}

{ increment counter <em>i</em> }




specialSum = 0       for <em>i</em>  0 to <em>n</em> − 1 do                for j  1 to <em>currentMaxOccurence</em> do                    { specialSum = specialSum + A[i] }

{ increment counter j }

{ increment counter <em>i</em> }




return specialSum







<ol>

 <li>Use the analysis from the course notes to determine a time complexity function f(n) for the above algorithm. Your answer must be simple and concise.</li>

</ol>




<ol>

 <li>What is the time complexity of this algorithm, in terms of Big-O?</li>

</ol>




<ol>

 <li>What is the space complexity of this algorithm, in terms of Big-O?</li>

</ol>




<ol>

 <li>Can we improve this algorithm to achieve a better time complexity and still return the same specialSum value?</li>

 <li>If yes:

  <ul>

   <li>give a new algorithm that achieves it.</li>

   <li>provide a time complexity function f(n) for the modified algorithm.</li>

   <li>provide the time complexity of the modified algorithm, in terms of Big-O.</li>

   <li>provide your observations regarding the two algorithms with respect to time complexity.</li>

  </ul></li>

</ol>




<ol>

 <li>If no, provide explanations as to why it cannot be improved.</li>

</ol>

<strong> </strong>

<h1>Programming Questions</h1>

<strong> </strong>

We received a list of people that are going to participate in a clinical test. The list includes the name and date of birth of the participants which is stored in two arrays: <em>pName</em> and <em>pDOB</em>. The two arrays are of the same size. The arrays’ size N is the number of participants. pName[0] hold the name of the first participant and pDOB[0] hold the date of birth of the first participant; pName[N-1] hold the name of the last participant and pDOB[N-1] hold the date of birth of the last participant. The participants’ information is stored in the arrays at random. We need to separate the participants in two groups: seniors and non-seniors. A person is considered senior if she/he is 65 years of age or older. You need to provide an algorithm that takes as input the two arrays and the number of participants. Your algorithm should rearrange the participants’ information in the arrays in the following manner:

<ul>

 <li>Array position zero hold the information of the oldest person in the participants.</li>

 <li>Array position N hold the information of the oldest non-senior participant.</li>

 <li>Senior participants should be stored in a decreasing order based on their age.</li>

 <li>Non senior participants should be stored in an increasing order based on their age.</li>

</ul>




A sample of two input arrays of size 10 and their contents after rearrangements by the algorithm is shown below:




<table width="522">

 <tbody>

  <tr>

   <td width="85">


    <table width="60">

     <tbody>

      <tr>

       <td width="60">Index</td>

      </tr>

      <tr>

       <td width="60">0</td>

      </tr>

      <tr>

       <td width="60">1</td>

      </tr>

      <tr>

       <td width="60">2</td>

      </tr>

      <tr>

       <td width="60">3</td>

      </tr>

      <tr>

       <td width="60">4</td>

      </tr>

      <tr>

       <td width="60">5</td>

      </tr>

      <tr>

       <td width="60">6</td>

      </tr>

      <tr>

       <td width="60">7</td>

      </tr>

      <tr>

       <td width="60">8</td>

      </tr>

      <tr>

       <td width="60">9</td>

      </tr>

     </tbody>

    </table></td>

   <td width="437">


    <table width="412">

     <tbody>

      <tr>

       <td colspan="2" width="164">Algorithm inputs</td>

       <td rowspan="12" width="55"><strong> </strong><strong> </strong>          </td>

       <td colspan="2" width="192">Algorithm outputs</td>

      </tr>

      <tr>

       <td width="77"><em>pName </em></td>

       <td width="87"><em>pDOB </em></td>

       <td width="90"><em>pName </em></td>

       <td width="102"><em>pDOB </em></td>

      </tr>

      <tr>

       <td width="77">Linda</td>

       <td width="87">1-1-2003</td>

       <td width="90">Sam</td>

       <td width="102">24-2-1940</td>

      </tr>

      <tr>

       <td width="77">Sam</td>

       <td width="87">24-2-1940</td>

       <td width="90">Maria</td>

       <td width="102">9-5-1941</td>

      </tr>

      <tr>

       <td width="77">Roger</td>

       <td width="87">11-12-1995</td>

       <td width="90">Melissa</td>

       <td width="102">25-7-1945</td>

      </tr>

      <tr>

       <td width="77">Alfred</td>

       <td width="87">31-3-1980</td>

       <td width="90">Roberto</td>

       <td width="102">29-6-1950</td>

      </tr>

      <tr>

       <td width="77">Roberto</td>

       <td width="87">29-6-1950</td>

       <td width="90">Thomas</td>

       <td width="102">20-7-2004</td>

      </tr>

      <tr>

       <td width="77">Melissa</td>

       <td width="87">25-7-1945</td>

       <td width="90">Linda</td>

       <td width="102">1-1-2003</td>

      </tr>

      <tr>

       <td width="77">Brian</td>

       <td width="87">15-7-2002</td>

       <td width="90">Brian</td>

       <td width="102">15-7-2002</td>

      </tr>

      <tr>

       <td width="77">Thomas</td>

       <td width="87">20-7-2004</td>

       <td width="90">Roger</td>

       <td width="102">11-12-1995</td>

      </tr>

      <tr>

       <td width="77">Leslie</td>

       <td width="87">27-4-1990</td>

       <td width="90">Leslie</td>

       <td width="102">27-4-1990</td>

      </tr>

      <tr>

       <td width="77">Maria</td>

       <td width="87">9-5-1941</td>

       <td width="90">Alfred</td>

       <td width="102">31-3-1980</td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>







<ol>

 <li>In this programming assignment, you will design an algorithm (in pseudo code), and implement (in Java), four functions as follows:

  <ul>

   <li><em>rearrangeParticipants</em>: a recursive function that take as input two arrays pName and pDOB and the number of paticipants, and returns the number of senior participants in addition to arranging the arrays as specified above.</li>

   <li><em>displaySeniorsIncreasingOrder</em>: a recursive function that takes as input the two arrays pName and pDOB and the number of senior participants and display the name and DOB of senior participants in an increasing order based on their age.</li>

   <li><em>displayNonSeniorsInreasingOrder</em>: a recursive function that takes as input the two arrays pName and pDOB, the number of non-senior participants and the total number of participants and display the name and DOB of non-senior participants in an increasing order based on their age.</li>

   <li><em>displayIncreasingOrder</em>: this function takes as input the two arrays pName and pDOB, the number of senior participants and the total number of participants and display all participants in an increasing order based on their age.</li>

  </ul></li>

</ol>




All your algorithms must handle possible special cases. For each implemented function you need to compare the runtime performance and measure the corresponding run times. You can use Java built-in time function for this purpose.

You can generate a file with random data and experiment your implementation against different size of participants’ list size N in {10, 100, 1000, 10000, 100000…,1000,000}. You should redirect the output of each set of test size to an out.txt file. You should write about your observations on the timing measurements in a separate text file. You are required to submit the fully commented Java source files, the compiled files, and the text files.




For each implemented function:

<ul>

 <li>Use the analysis from the course notes to determine a time complexity function f(n). Your answer must be simple and concise.</li>

 <li>What is the time complexity of the function in terms of Big-O?</li>

</ul>




<ol>

 <li>For <em>rearrangeParticipants</em> recursive algorithm:

  <ul>

   <li>Briefly explain whether your algorithm is linear or not.</li>

   <li>Does your algorithm use tail recursion? Why or why not? Explain your answer. If your answer is “No” then: can a tail-recursive version for this algorithm be designed?

    <ol>

     <li>If yes; write the corresponding pseudo code for that tail recursion algorithm and implement it in Java and repeat the same experiments as in part (a) above.</li>

     <li>If no, explain clearly why such tail-recursive algorithm is not feasible.</li>

    </ol></li>

  </ul></li>

</ol>





