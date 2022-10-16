Chris Nakayama
White Boarding Study README.md


Whiteboarding Independent Project
During your normally scheduled independent project time, you will prepare for your whiteboard interview session. 5 questions are included below for you to study and develop solutions for. At the time and date designated by your instructor, you will conduct your whiteboarding interview with a group of students. Your instructor will randomly assign you a question to whiteboard for your group, so make sure you are prepared to whiteboard each of the 5 questions.

For each of the other students in your group, we expect you to log into Epicenter to fill in and complete the peer evaluation rubrics. You can find the link for adding evaluations here: https://epicenter.epicodus.com/peer_evaluations/new. You and your group can decide when to fill out the peer evaluation, either after each whiteboard, or at the end of the session.

This is a mock technical interview, so the goal is to practice as if you were interviewing for a real job. For both the interviewers (who are giving feedback) and interviewee (who is whiteboarding), this means that you should be formal in your presentation:

Check to make sure folks can hear you, see your code.
Speak clearly, doing your best not to trail off in your speech or mumble.
Make eye contact.
Be polite and encouraging.
If the interviewee is stuck and you (the interviewer) know how to get unstuck:
Give the interviewee space to figure out next steps before offering help.
Ask the interviewee if they want help before giving help.
If you are doing this remotely, have your video turned on. If you are having a technical issue that makes it so you can't share your video, let your group members know.
At the end of the group interview session, you will be expected to submit your whiteboard solution. You can submit either a txt file or if you prefer you may submit a picture of a whiteboard or written solution. The purpose of the txt file is to write and submit an answer that includes no auto-fill from VS Code.

Expectations for Peer Evaluations
One of the objectives (listed below under "objectives") is for your peer evaluations to include constructive feedback. This means that we expect you to write full sentences and give specific examples from the interview about what the interviewee can improve upon in their performance.

This also means it's not acceptable just to write "good job!" or "that was terrible." We expect you to give both concrete and constructive feedback, whether positive or negative. Review this lesson on Giving Constructive Feedback for more specific examples.

Writing "They have nothing to improve on." is not considered constructive feedback, and will cause you to receive a failing grade. In the following week, your instructor will let you know how to make up the assignment.

Remember, this is an important time for you as the interviewer to think critically and scrutinize anything that an interviewer at a potential workplace would. If you are struggling to come up with examples of where an interview can improve, consider these:

Error handling
Handling edge cases
Testing all cases based on the possible inputs/outputs
If time remains, engaging in more discussion about the prompt. For example, what a more efficient solution might look like?
Feedback on presentation:
Eye contact
Clarity in explanations about code and decision making.
Whether assumptions were made that could have been clarified with questions
Code style (comments, variable naming)
Use of technical terminology
Objectives
Your project will be evaluated based on the following objectives:

Whiteboard solution has been submitted.
Whiteboard interview meets all requirements (based on peer feedback).
Your evaluations for peers are complete and include constructive feedback.
Questions
Question #1: Turning Strings to URLs
URLs cannot have spaces. Instead, all spaces in a string are replaced with %20. Write an algorithm that replaces all spaces in a string with %20.

You may not use the replace() method or regular expressions to solve this problem. Solve the problem with and without recursion.

Example
Input: "Jasmine Ann Jones"

Output: "Jasmine%20Ann%20Jones"

Question #2: Array Deduping
Write an algorithm that removes duplicates from an array. Do not use a function like filter() to solve this. Once you have solved the problem, demonstrate how it can be solved with filter(). Solve the problem with and without recursion.

Example
Input: [7, 9, "hi", 12, "hi", 7, 53]

Output: [7, 9, "hi", 12, 53]

Question #3: Compressing Strings
Write an algorithm that takes a string with repeated characters and compresses them, using a number to show how many times the repeated character has been compressed. For instance, aaa would be written as 3a. Solve the problem with and without recursion.

Example
Input: "aaabccdddda"

Output: "3ab2c4da"

Question #4: Checking for Uniqueness
Write an algorithm that determines whether all the elements in a string are unique. You may not convert the string into an array or use array methods to solve this problem. The algorithm should return a boolean.

Example
Input: "hello"

Output: false

Input: "copyright"

Output: true

Question #5: Array Sorting
Write an algorithm that sorts an array without using the sort() method. There are many different sorting algorithms — take the time to read about the following:

Quick sort
Merge sort
Heap sort
Insertion sort
Bubble sort
Selection sort
You may implement any of the above algorithms (or your own) to solve the problem — as long as it doesn't use sort().

Example
Input: [9, 2, 7, 12]

Output: [2, 7, 9, 12]

STUDY LOG

I studied for at least four hours on this project for White Boarding.

Some of my group was able to get together to study and some of the questions below are from our study group.

Videos:
https://www.youtube.com/watch?v=DIR_rxusO8Q

https://www.youtube.com/watch?time_continue=1&v=dIrS31CCITM&feature=emb_title

Study Examples for White Boarding From the Group:

Question 3
For question 3
function compress(string) {
  let outputString = "";
  let currentLetter = string[0];
  let count = 1;
  for (let i = 1; i < string.length; i++) {
    if (string[i] === currentLetter) {
        count++;
    } else if (count !== 1) {
        outputString += count + currentLetter;
      currentLetter = string[i];
      count = 1;
    } else {
        outputString += currentLetter;
      currentLetter = string[i];
    }
  }
  if (count === 1) {
      outputString += currentLetter;
  } else {
      outputString += count + currentLetter;
  }
  console.log(outputString);
}

compress("aaabccdddda");
snicket
 added 
BradBuchholz
 to the group.
 — 10/06/2022
Sue Roberts (she/her) — 10/06/2022
function sortArray(array){
  for (let i = 0; i < array. length; i++) {   // loop to sort array
   for (let j = i + 1; j < array. length; j++) { // loop to check 2nd number is greater than 1st number

     if(array[i] > array[j]){   // if 1st num > 2nd num switch place
       temporary = array[i];    //  temp = 1st num
       array[i] = array[j];     //  1st num = 2nd num
       array[j] = temporary;    //  2nd num = 1st num
     }
    }
  }
  return array;
}



My write up for Question number 4
Question 4

function sameness(string) {
        let notSame = "";     //empty string

        for(let i = 0; i < string.length; i++) {  //loop to check if character is in string
          if(notSame.includes(string[i]) === false) { // if charcter is in string = false
            notSame += string[i];                     // push to notSame 
          }
        }

        if (notSame === string) {    // compare input string to notSame
          return true;                 // same then return true
        } else {
          return false;                // else return false
        }
      }


      I completed the White Boarding exercise and participated as a peer for other members of my cohort. I turned in evaluations for my peers.
      
      I spoke to Cathy about what to turn in. Cathy told me a REPO with at least 4 hours of commmits to show that I studied for this exam and what resources I used. I included all of the material in this repo.