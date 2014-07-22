"Friends" Rock, Paper, Scissors Game
==========

NOTE: This is an experiment as I take my first baby steps in coding. Code mostly riffs off of exercises completed in online coding courses in an attempte to make them my own!




If you're anything like me, you're a huge fan of the T.V. show, "Friends".

This game is a based on an episode from "Friends" (Season 10, Episode 8), where Rachel, Phoebe, Joey, and Ross play "Rock, Paper, Scissors" to decide who will go inside for Thanksgiving dinner first. Of course, you can bet that this isn't your typical game of "Rock, Paper, Scissors". 

Watch this YouTube clip to see what kind of game you're about to play!: https://www.youtube.com/watch?v=o_xH__mg03w

=



    var userChoice = prompt("Hope you're ready to play 'Rock, Paper, Scissors' with your favorite group of FRIENDS! Okay, do you choose rock, paper, scissors, fire, or water balloon?");
    var computerChoice = Math.random();
    	if (computerChoice < 0.20) { 
    		computerChoice = "rock";
    	} else if(computerChoice <= 0.40) {
    		computerChoice = "paper";
    	} else if(computerChoice <= 0.60) {
    		computerChoice = "scissors"
    	} else if(computerChoice <= 0.80) {
    		computerChoice = "fire";
    	} else {
    		computerChoice = "water balloon";
    	}
    console.log("Computer: " + computerChoice);
    var compare = function (choice1, choice2)
    {
    if(choice1 === choice2) {
    	return "Oh, looks like you both chose the same thing, so it's a tie! PLay again?";
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
    
