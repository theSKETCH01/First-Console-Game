#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int player, playAgain;
    const char *object[] = {"", "Stone", "Paper", "Scissor"};

    printf("Welcome to the Stone, Paper and Scissor Game!\n\n");

    srand(time(NULL));

    for (;;)
    {
        for (;;)
        {
            printf("Choose a number (1 : Stone; 2 : Paper; 3 : Scissor): ");
            scanf("%d", &player);

            if (player < 1 || player > 3)
            {
                printf("Invalid Input, please enter a number from 1 to 3.\n");
                continue;
                ;
            }

            int computer = (rand() % 3) + 1;

            printf("You choose: %s\n", object[player]);
            printf("Computer choose: %s\n", object[computer]);

            if (player == computer)
            {
                printf("It's a DRAW!, Try again.\n");
                continue;
            }
            else if (player == 2 && computer == 1 ||
                     player == 3 && computer == 2 ||
                     player == 1 && computer == 3)
            {
                printf("You Won!.\n");
                break;
            }
            else
            {
                printf("You Lose!, Try again.\n");
                continue;
            }
        }
        printf("Wanna Play Again? (Yes = 1, No = 0): ");
        scanf("%d", &playAgain);

        if (playAgain == 1)
        {
            printf("Starting the game again...\n\n");
            continue;
        }
        else if (playAgain == 0)
        {
            printf("Thanks for playing.\n");
            break;
        }
    }
    return 0;
}
