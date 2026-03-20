include <stdio.h>

2

#include <stdlib.h>

3

#include <time.h>

4

5

int main() {

6

int number, guess, attempts = 0;

7

8

/ Random number generate karne ke liye

9

srand(time(0));

10

number = rand() % 100 + 1; / 1 to 100

11

12

printf("🎮 Welcome to Number Guessing Game!\n");

13

printf("Guess a number between 1 to 100\n");

14

15

do {

16

printf("Enter your guess: ");

17

scanf("%d", &guess);

18

attempts +;

19

20

if (guess > number) {

21

printf("Too High! Try again.\n");

22

} else if (guess < number) {

23

printf("Too Low! Try again.\n");

24

} else {

25

printf("🎉 Correct! You guessed in %d attempts.\n", attempts);

26

}

27

28

} while (guess = number);

29

30

return 0;
