# casino

Files:

Dice - small method which emulates rolling a dice:
returns a random number 1-6 when the method is called

Card - class which constructs the card to have properties suit, face, and face value
suit: String, one of "spades", "clubes", "hearts", or "diamonds"
face: String, a number "2"-"10","jack", "queen", or "king" 
faceValue: a number associated with face; 2-10 remain the same and jack-ace are 11-14
includes getter methods

DeckOfCards - class which constructs an array (deck) of 52 Card objects with the above specifications
includes methods shuffle() and draw() which put the cards in a random order and takes the first card of the array

blackjack - creates the game
main function goes throguh the game by calling methods in the order plays would be called in a game:
        //player places their bet
        bets();
        //the cards are shuffled
        shuffleDeck();
        //deal card to player using draw method from DeckOfCards and iterate
        deal(player);
        System.out.println("The player has: " + player);
        //deal card to dealer and the player can see how many points the dealer have
        deal(dealer);
        System.out.println("The dealer has: " + dealer);
        //deal another card to player and the player can see how many points the they have
        deal(player);
        System.out.println("The player has: " + player);
        //deal other card to dealer but the player can't see how many points the dealer has
        deal(dealer);
        System.out.println("Second card dealt to dealer");

        //checkCards will determine if the player has a bust or if they have 21
        checkPlayerCards();

