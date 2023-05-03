Download Link: https://assignmentchef.com/product/solved-cs-115-introduction-to-programming-in-python-lab-guide-08
<br>
<strong>Lab Objectives:</strong>  Classes and Inheritance​

<strong>Instructions:</strong>​ Upload your solutions as a single .zip file to the Lab08 assignment on Moodle before the end of your lab session. Use the following naming convention:

SS_Lab08_Surname_FirstName.zip where SS is the section number 01, 02, 03, etc.




<ol>

 <li>Download the class Question​ (​ <strong>py</strong>​          )​ that represents a typical Exam Question object. Review the details of this class.

  <ol>

   <li>The class stores the following data attributes:

    <ul>

     <li>questionText</li>

     <li>correctAnswer</li>

     <li>score</li>

     <li>studentAnswer</li>

    </ul></li>

   <li>The class defines the following methods:

    <ul>

     <li>an ​ __init__()​ ​ ​method​ ​that initializes the first 3 data members with values passed as parameters, initializes studentAnswer​ ​ to None.</li>

     <li>Methods to return and update the values of all data attributes.</li>

     <li>isCorrectAnswer()​: returns True if the correct answer matches the studentAnswer, false if not.</li>

     <li>answerQuestion()​: takes an answer as a parameter, and sets the studentAnswer​ with the value passed as a parameter.</li>

     <li>scoreQuestion():​ if the studentAnswer​ is correct return the question score, otherwise return 0.</li>

     <li>displayQuestion()​: prints the question text.</li>

     <li>__repr__() returns the string representation of the Question​ object formatted as in the sample run.</li>

    </ul></li>

  </ol></li>

</ol>










<ol>

 <li>Write a class called TrueFalseQuestion​       (​ <strong>py</strong>​ )​ that represents subclass of a Question​              .​</li>

 <li>The class will store the additional data attribute:

  <ul>

   <li>incorrectPoints:​ the number of points to be deducted in case of a wrong answer.</li>

  </ul></li>

</ol>




<ol>

 <li>Your class should have an ​ __init__() ​ that:​      initializes the inherited data members to values passed as parameters, using the super class __init__() ​          method.​

  <ul>

   <li>initializes the incorrectPoints​ to the final value passed as a parameter.​</li>

  </ul></li>

</ol>




<ol>

 <li>You should override the following inherited methods:

  <ul>

   <li>scoreQuestion():​ if the studentAnswer​ is correct return the question score, otherwise return the negative incorrect points.​</li>

   <li>displayQuestion(): prints the text: ‘True or False: ’ followed by the question text.</li>

  </ul></li>

</ol>




<ol start="2">

 <li>Write an application,<strong>py,</strong>​ ​ that includes the following functionality:

  <ol>

   <li>initializeQuestions():​

    <ul>

     <li>takes a fileName and an empty list as parameters. Using the data about Questions in the file, creates</li>

    </ul></li>

  </ol></li>

</ol>

Question/​ TrueFalseQuestion​  ​ objects and adds them to the list passed as parameter.




<ol>

 <li>gradeExam():​

  <ul>

   <li>Takes a list of Question ​ objects as a parameter.​</li>

   <li>Displays a header *** Grading Exam ***, see sample run for details.</li>

   <li>Scores each question and returns the total points, and the sum of the correct answers for all questions. Correct answer score should be determined using the scoreQuestion() method for each question.​</li>

   <li>For each question answered incorrectly, displays the questions with the heading ‘Incorrect Answer’. (see sample run)</li>

   <li>Displays a footer *** End of Grading ***, see sample run for details.</li>

  </ul></li>

</ol>




<ol>

 <li>The program should do the following:

  <ul>

   <li>Read the questions from the file using the function defined above.</li>

   <li>For each question in the list, display the question and input the student’s (user’s) answer.</li>

   <li>Store the student answer for each question.</li>

   <li>Once the exam is finished, grade the exam using the function, and display the final score as shown in the sample run.</li>

  </ul></li>

</ol>




<strong> </strong>

<strong>Sample File: </strong>

The file is a semi-colon delimited file, containing the following on each line: type of question (T for True False or R for regular), the question text, the correct answer, and the points. If the question is a true false question, it also contains points to deduct in case of an incorrect answer.




<strong> </strong>

<strong>Sample Run: </strong>

True or False:

Python is not a high level programming language?




Enter choice: True

Who invented Python?




Enter choice: I don’t know

In what year was Google launched on the web?




Enter choice: 1998

In computing what is Ram short for?




Enter choice: Random Access Memory True or False:

The # symbol can be places to the right of an executable statement ?




Enter choice: True True or False:

Non-zero values map to False in Python?




Enter choice: False







*****************Grading Exam***************** Incorrect Answer!

Python is not a high level programming language?

Your Answer:True

Correct Answer:False




Incorrect Answer!

Who invented Python?

Your Answer:I don’t know

Correct Answer:Guido van Rossum




*****************END OF GRADING*****************

Your score is:  17 / 27


