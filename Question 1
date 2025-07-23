#include<stdio.h>
#include<math.h>
int main()
{
  void identifyColor(float lamda){

    if(lamda >= 380 && lamda < 450)
        printf("Light color: Violet\n");
    else if(lamda >= 450 && lamda < 485)
        printf("Light color: Blue\n");
   else if(lamda >= 485 && lamda < 500)
        printf("Light color: Cyan\n");
   else if(lamda >= 500 && lamda < 565)
        printf("Light color: Green\n");
   else if(lamda >= 565 && lamda < 590)
        printf("Light color: Yellow\n");
   else if(lamda >= 590 && lamda < 625)
        printf("Light color: Orange\n");
   else if(lamda >= 625 && lamda <= 750)
        printf("Light color: Red\n");
   else
        printf("Light color: Invisible range\n");
    }
    int m;
    float distance_mm, deg_theta;

    printf("Enter m: ");
    scanf("%d",&m);

    printf("Enter theta (in degree): ");
    scanf("%f",&deg_theta);

    printf("Enter slit distance d (in micrometer): ");
    scanf("%f",&distance_mm);


    float degree_rads = deg_theta * (M_PI/180.0);

    float distance_m = distance_mm * 1e-6;

    float lamda_m = (distance_m * sin(degree_rads)) / m;

    float lamda_nm = lamda_m * 1e9;

    printf("\nCalculate wavelength: %.2f nm\n",lamda_nm);
    identifyColor(lamda_nm);

    return 0;


}

