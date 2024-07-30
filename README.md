
// Task-2 

// Number Guessing Game 
/*

Create a program that generates a random number and asks the user to guess it. 
Provide feedback on whether the guess is too high or too low until the user guesses
the correct answer.

*/

#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    
    srand(static_cast<unsigned int>(time(0)));
    // Generating a random number between 1 and 100
    int numberToGuess = rand() % 100 + 1;
    int userGuess = 0;

    cout << "Welcome to the Number Guessing Game!" << endl;
    cout << "I have selected a number between 1 and 100. Can you guess it?" << endl;

    while (true) {
        cout << "Enter your guess: ";
        cin >> userGuess;

        if (userGuess < numberToGuess) {
            cout << "Too low. Try again." << endl;
        } else if (userGuess > numberToGuess) {
            cout << "Too high. Try again." << endl;
        } else {
            cout << "Congratulations! You guessed the correct number!" << endl;
            break;
        }
    }

    return 0;
}

    
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
