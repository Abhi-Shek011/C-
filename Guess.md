
#include <iostream>
#include<vector>
#include <cstdlib>
#include <ctime>
using namespace std;
void play_game()
{
         int guess ; 
        int secret  ;
        int tries;
        
          srand(time(NULL));
         secret = rand() % 10 + 1 ;
         cout << "Tell How many Times You want guess" << " " << endl; 
         cin >> tries;
    
       for(int attemp = 1; attemp <= tries ; attemp++ )
       {
            cout << " Its attempt number" << attemp << endl ;
              cout << "Enter Your guess " << endl ;
               cin >> guess;

     
    
              if( guess ==  secret)
                 {
                         cout << "You guessed correct" << endl;
                     return;
                 }

                 else if ( guess > secret )
                  {
                            cout << " Number is lower" << endl ;
                     }

                if( guess < secret)
                 {
                    cout << " Number is higher" << endl ;
                 }
         
           
       }
       
       cout << " Buddy out of tires"<< " \n number was " << secret <<endl;
}
/* namespace first { 
    int x = 1; 
}
*/
int main (){
 /* 
double student = 20 ; 
student/=3;


/
    number_t age = 20 ;
    age = age- 1 ;

    std::cout << age ; 
/*
    int a,b ;
    a = 5;
    b = 4; 
    std::cout << a + b ;
    */
   /* const int PI = 3.14; 
    int PI = 3.34; 
    */
    /* std::cout << first::x; 
 std::cout << student;*/

        string Wanna; 
         string wanna_play = "Yes";
    do{
           int choice;
         cout << " Hello player " << endl ;
            cout << "1.play" << endl << "2.quit" << endl;
          cin >> choice ;
    /*
             switch(choice)
             {
                case 0 :
                cout << " its okie " << endl ;
                break;
                case 1 :
                play_game();
                break;
                default: 
                cout << "Put ur valid answer bro";
             }
       */
        if (choice == 2) {
            cout << "Magar Whyy" << endl;
            break; 
        } else if (choice == 1) {
            do {
                play_game();
                cout << "\nDo you want to play again? (Yes/No): ";
                cin >> wanna_play;
            } while (wanna_play == "Yes" || wanna_play == "yes");
        } else {
            cout << "nvalid choice!" << endl;
        }
        break;
             cout  << "wanna play the game again" << endl << "yes or no" << endl;
             cin >> Wanna ;
         }while(Wanna == "yes" );
      cout<< "thanks or playing ";
    }





     

