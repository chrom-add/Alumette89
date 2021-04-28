#include <stdio.h>
#include <stdlib.h>

int verif_total_alumette(int choice)
{
  int cpt = 0 ; 
  do
    {
      printf("Choice between 10 and 100 alumettes\n");
      scanf("%d",&choice);
      if(choice < 10 || choice > 100)
      {
	printf("Sorry choice between 10 or 100 alumettes\n");
	cpt ++ ;
      }
      if(cpt > 3 )
	{
	  printf("Sry tentative max attempt\n");
	  break;
	}
	  
    }while(choice < 10 || choice > 100); 
  return choice  ; 
}

int draw(int nbr_alumette, int i )
{ 
  while(i < nbr_alumette )
    {
      i++;
      printf("|");
    }
  if(nbr_alumette == 1)
    {
      printf("Le prochain piocheur est perdant !!\n");
      exit(0);
    }
  return 0 ;

}
int verif_choice_gamer(int gamer)
{
  int cpt = 0 ;
  int choice_final ; 
  do
    {
      printf("Veuillez choisir entre 1 et 3 alumette \n");
      scanf("%d",&gamer);
      if(gamer > 3 || gamer < 1)
	{
	  printf("Veuillez entrer des saisies correct\n");
	  cpt ++ ; 
	}
     if(cpt > 3 )
	{
	  printf("Tentative max atteinte\n");
	  exit(0);
	}
    }while(gamer < 1 || gamer > 3 );
  return gamer ;
  
}
int main(void)
{

  int choice_alumette ; 
  int gamer1 ; 
  int total_alumette ; 
  
  printf("Welcom to the AlumetteGame\n");
  total_alumette = verif_total_alumette(choice_alumette);

  int i = 0; 
  draw(total_alumette, i );
  int runing = 1 ; 
  while(runing)
  {
    /*___________________________________*/
    /*  GAMER1 */
    /*__________________________________*/
    int recup_choice1 ;
    printf("\n Gamer1 : \n");
    recup_choice1 = verif_choice_gamer(gamer1);

    total_alumette -= recup_choice1 ;
    draw(total_alumette,i);
    /* GAMER 2*/
    /*--------------------------------*/
    int gamer2 ;
    int recup_choice2 ;
    printf("\n Gamer 2 : \n");
    recup_choice2 = verif_choice_gamer(gamer2);

    total_alumette -= recup_choice2 ;
    draw(total_alumette,i);

  }
   return(0) ; 
}
