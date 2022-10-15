Chris Nakayama
White Boarding Study README.md

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