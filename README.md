
<script> 
 let playerScore= 0;
 let computerScore=0;
 let options=['paper','rock','scissors'];
 

 function randomComputer(){
     let randomValue= options[Math.floor(options.length * Math.random())];
     let random= randomValue.toLowerCase();
     return random;
 }
 
 function playGame(){
    for (let i=0; i<=5;i++){ 
        let playerSelection= prompt('rock,paper, or scissors?');
        computerSelection= randomComputer();
    if (playerScore===5){
        console.log('you winbaba');
        return;
    } else if (computerScore===5){
        console.log('you loseaaa');
        return;
    } else  if (playerSelection===computerSelection){
        playerScore++;
        computerScore++;
        console.log('tie');
    } else if (playerSelection==='rock'&& computerSelection==='paper'){
        computerScore++;
        console.log('you losea');
    } else if (playerSelection==='rock'&& computerSelection==='scissors'){
        playerScore++;
        console.log('you wina');} else if(playerSelection==='paper'&& computerSelection==="rock"){
            playerScore++;
            console.log('fucking win br bra');
    } else if (playerSelection==='paper'&& computerSelection==='scissors'){
            computerScore++;
            console.log('fucking lose ba bra');
    } else if (playerSelection==='scissors'&& computerSelection==="rock"){
            playerScore++;
            console.log('fucking lose bra a');
    } else if (playerSelection==='scissors'&& computerSelection==="paper"){
            computerScore++;
            console.log('fuckg win bra bra');
    }
 }
 }

playGame()
            
</script>