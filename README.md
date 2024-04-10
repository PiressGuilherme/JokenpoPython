# JokenpoPython

This code is a Python program that simulates a rock-paper-scissors tournament among multiple players.

Import the pandas library for data manipulation, random for random operations, and math for mathematical functions.

Define a function jogo that takes four arguments (jogador1, opcao1, jogador2, opcao2) representing the players' names and choices (rock, paper, or scissors). The function compares the choices to determine the winner and updates a DataFrame campeonato with the match details.

Define a function classifica that takes campeonato and tabela (the tournament table) as arguments. It iterates through the table, pairs players for matches, calls the jogo function to determine the winner of each match, and updates the campeonato DataFrame with the winners. It returns a DataFrame with the winners for the next round.

Load a CSV file (campeonato.csv) into a DataFrame tabela. Then, while there is more than one column in the tabela DataFrame, it creates a new campeonato DataFrame, shuffles the player order, and calls the classifica function to determine the winners of each round until there is only one winner.

Finally, it resets the tournament by reloading the CSV file into tabela, creating a new campeonato DataFrame, shuffling the player order, and printing the new player order.
