infantcode
==========

Baby steps in coding--mostly riffing off of exercises completed in online coding courses to try to make them my own!

var userChoice = prompt("Hope you're ready to play 'Rock, Paper, Scissors' with your favorite group of FRIENDS! Okay, do you choose rock, paper, scissors, fire, or water balloon?");
var computerChoice = Math.random();
if (computerChoice < 0.20) {
	computerChoice = "rock";
} else if(computerChoice <= 0.40) {
	computerChoice = "paper";
} else if(computerChoice <= 0.60) {
	computerChoice = "scissors";
} else if(computerChoice <= 0.80) {
	computerChoice = "fire";
} else {
	computerChoice = "water balloon";
} 
console.log("Computer: " + computerChoice);

var compare = function (choice1, choice2)
{
    if(choice1 === choice2) {
        return "Oh, looks like you both chose the same thin, so it's a tie! Play again?";
    }

    else if(choice1 === "rock") {
        if(choice2 === "scissors") {
            return "Rock wins!";
        }
        else if (choice2 === "fire") {
            return "Fire wins!";
        }
        else if (choice2 === "water balloon") {
            return "Rock wins!";
        }
        else {
            return "Paper wins!";
        }
    }
    else if (choice1 === "paper") {
        if(choice2 === "rock") {
            return "Paper wins!";
        }
        else if (choice2 === "fire") {
            return "Fire wins!";
        }
        else if (choice2 === "water balloon") {
            return "Water Balloon wins!";
        }
        else {
            return "Scissors wins!";
        }
    }
    else if(choice1 === "scissors") {
        if(choice2 === "rock") {
            return "Rock wins!";
        }
        else if (choice2 === "fire") {
            return "Fire wins!";
        }
        else if (choice2 === "water balloon") {
            return "Scissors wins!";
        }
        else {
            return "Scissors wins!";
        }
    }
    else if(choice1 === "fire") {
        if(choice2 === "scissors") {
            return "Fire wins!";
        }
        else if (choice2 === "rock") {
            return "Fire wins!";
        }
        else if (choice2 === "paper") {
            return "Fire wins!";
        }
        else {
            return "Water Balloon wins!";
        }
    }
    else if(choice1 === "water balloon") {
        if(choice2 === "rock") {
            return "Rock wins!";
        }
        else if (choice2 === "paper") {
            return "Water Balloon wins!";
        }
        else if (choice2 === "scissors") {
            return "Scissors wins!";
        }
        else {
            return "Water Balloon wins!";
        }
    }
}
compare(userChoice, computerChoice) 
