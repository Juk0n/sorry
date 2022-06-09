#include<stdio.h>
#include<stdlib.h>

int main(){

    int id=0;
    int age=0;
    int number=0;
    int smoney=0;
    int money=0;
    int numb=0;

    printf("$$$ welcome from the game $$$\n");
    printf("enter your age\n");
    scanf("%d",&age);

    if(age>=18){
            printf("enter your total money");
            scanf("%d",&smoney);
            while(smoney<3000){
                    printf("you dont have enough money");
                    exit(0);




            }while(age>=18){
                printf("enter your id");
                scanf("%d",&id);

                while(id==3600){
                        printf("enter your bet place money\n money must be at least 1000ks");
                        scanf("%d",&money);

                        while(money>=1000){
                                printf("enter your lottery number");
                                scanf("%d",&number);

                                if(number==rand()%100){
                                    printf("lottery winning number is %d\n\n",rand()%100);
                                    smoney=smoney*7;
                                    printf("lottery winning\n");
                                    printf("you are winner congratslution\n your total money is %d\n\n",smoney);
                                    printf("if you want to play again press1\n\n");
                                    printf("if you want to quit press 2\n\n");
                                    scanf("%d",&numb);

                                    if(numb==1){
                                            printf("welcome back from the game\n");




                                    }else{
                                        printf("thanks for playing mista");

                                    }







                                }else{
                                    printf("lottery winning number is %d\n",rand()%100);
                                    printf("you lose try again!!\n");
                                    smoney=smoney-money;
                                    printf("your total money is %d\n",smoney);
                                    printf("if you want to play again press 1\n");
                                    printf("if you want to quit the game press 2\n");
                                    scanf("%d",&numb);

                                    if(numb==1){
                                            printf("thank you for playing again\n");
                                            while(smoney<3000){
                                                    printf("you dont have enough money\n");
                                                    exit(0);



                                            }



                                    }else{
                                        printf("thank you for playing mista goodbye");
                                        exit(0);

                                    }




                                }




                        }





                }




            }








    }else{
        printf("you are not old enough");


    }







    return 0;
    }
