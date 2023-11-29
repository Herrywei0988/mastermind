# mastermind
# Mastermind is a pattern-guessing game that was first coded for a computer in the 1960s. For more history
# on the game and discussion of the rules see https://en.wikipedia.org/wiki/Mastermind_(board_game). The
# idea of Mastermind is that the computer creates a fixed sequence of symbols that must be guessed within
# a certain number of turns by the player. In our version, the following rules will be used:

''''1. The computer creates a random sequence of 4 values selected from 6 possible values: 1, 2, 3, 4, 5, 6.
    2. The player has 12 turns to guess the correct sequence.
    3. Each turn consists of the player guessing a 4-value sequence, e.g. “1234”. If the guess does not contain exactly 
       4 values in the range of 1-6, the user must be prompted to re-enter the guess.
    4. After each guess the computer displays a pattern indicating:
        a. the number of guesses with the correct symbol and position using a closed circle: ●
        b. the number of guesses with the correct symbol but wrong position using an open circle: ○
    There is a 1-to-1 mapping between guessed symbols and sequence symbols: each value
    from the guess can only be connected with a single value in the target sequence, and visa
    versa. Perfect matches take precedence over partial matches (right value in wrong
    location).
    
    Here is an example of a single guess and computer response with a pre-defined random sequence:
    
    sequence = 1121
    guess    = 1241
    result: ●●○
    The result makes sense because the 1st and 4th values of 1 are in the sequence at the right
    positions (●), while the 2nd guess value of 2 is in the target sequence but with the wrong
    position (○).
    
    Here is another example with the same guess but a different target sequence:
    
    sequence = 6321
    guess    = 1241
    result: ●○
    
    In this case the 4th value of 1 is at the right position (●), while the 2nd guess value of 2 is
    in the sequence at the wrong position (○). The 1st guess value of 1 does not yield a
    symbol even though there is a 1 in the sequence since the 4th guess value has already
    “used up” this entry in the sequence.
    
    5. If the player gets the entire correct sequence within 12 turns they win, otherwise they lose.
    If the player wins, display a congratulatory message.
    
    6. After the player loses, the correct sequence must be displayed. 
    
    Your job is to write a Mastermind program in Python that will implement the above rules. There are many
    different ways to approach this problem, but start by thinking about what kind of data structure you want
    to use to store the target sequence and player guesses, and how to work with that data structure to
    determine the result of each turn. Once your code is working, play it through several times to make sure
    the behavior is correct for both winning and losing cases.  '''
