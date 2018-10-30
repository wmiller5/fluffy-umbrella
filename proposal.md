# X-Team 07 Project Proposal

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

Briefly describe a problem that your team would like to solve.  
Describe at a high level a program that could solve that problem.

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)  
College Calender


2. Output: Describe the output your program will produce. Include and example format of the output produced.
   * The program will output a list of all coming assignments ordered by due date. For those due on the same date, order them by their weights on grade. 
   * example output:  
       Journalism MediaAnalysisEssay 10/26/2018 9:55am 15%  
       History paper 10/26/2018 11:59pm 20%  
       Computer Science p3 10/29/2018 11:59pm 10%
 

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.
   There are two functions of the program. 
   * Input information of an assignment: assignmentName, dueDate, subject, weight  
   ex. MediaAnalysisEssay, 10/26/2018 9:55am, Journalism, 15%
   * Current date on which the user want a schedule.  
   ex. 10/31/2018


4. User Interface: Describe a user interface for your program. Use text menus or a simple graphic user interface.  
   For now, we plan to simply make it a Text interface.  
   But for further promotion to students, it would be most probably an app. See the following figure.  
   <img src="https://i.imgur.com/sOoa4Y9.jpg" width=200><br>


5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
   1. AssignmentNode(String name, String due, String subject, int weight)
       * This class generates objects to store each assignment's basic information such as name, due date and time, course, and grade weights.
       * It should be able to initialize an instance according to the user's inputs.
       * Consider possible variances on the inputs. For example, some assignment may have more than one due day (part a, part b); and users may sometimes want to add more information (remarks). Thus, there should be more than one constructors to adapt to the user's inputs.
   2. CustomLinkedList
       * Our customized data structure to store all the AssignmentNodes.
       * It should enable node insert, delete, and the most important, get according to due date and grade weights. So it will probably use priority queue. We are still thinking about how to arrange nodes: by date, subject, or other criteria.
   3. Main (enable the user to run other staff)
       * The main class is used for user input and command for schedule output. Also, it will call methods in the CustomLinkedList to perform tasked required by the user.

Name each interface or class and briefly describe its function or purpose.


## Edit and Submit this file and any figures referenced by this document.

