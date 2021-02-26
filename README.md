# Chapter6
Exercises 6
### Exercise 6.1
#include <stdio.h>
char  line[100];   
float a,b,c,d,x, y, distance;   

int main()
{
    printf("Enter point x1: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%f", &a);
    printf("Enter point y1: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%f", &b);
    printf("Enter point x2: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%f", &c);
    printf("Enter point y2: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%f", &d);
    x = c-a;
    y = d-b;
    
    distance = sqrt (x*x + y*y);
    
    printf ("the distance is %f", distance);
}
### Exercise 6.2
#include <stdio.h>
char  line[100];   
int   g;   

int main()
{
    printf("Enter the score: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &g);
    if (0<=g && g<=60){
    	printf("F");
    }
    else
    {
        if (61<=g && g<=70){
            printf("D");
        }
	else
	{
	    if (71<=g && g<=80){
	        printf("C");
	    }
	else
	{
	    if (81<=g && g<=90){
	        printf("B");
	    }
	    else{
	    if(91<=g && g<=100){
	        printf("A");
	    }
	    }
	}
	}
    }
}
### Exercise 6.3
#include <stdio.h>
char  line[100];   
int   g;   

int main()
{
    printf("Enter the score: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &g);
    if (0<=g && g<=60){
    	printf("F");
    }
    else
    {
        if (61<=g && g<=63){
            printf("D-");
        }
        else{
            if(64<=g && g<=67){
                printf("D");
            }
            else{
                if (68<=g && g<=70){
                    printf("D+");
                }
                if (71<=g && g<=73){
                    printf("C-");
                }
                else{
                    if(74<=g && g<=77){
                        printf("C");
                    }
                    else{
                        if (78<=g && g<=80){
                            printf("C+");
                        }
                        if (81<=g && g<=83){
                            printf("B-");
                        }
                        else{
                            if(84<=g && g<=87){
                                printf("B");
                            }
                            else{
                                if (88<=g && g<=90){
                                    printf("B+");
                                }
                                if (91<=g && g<=93){
                                    printf("A-");
                                }
                                else{
                                    if(94<=g && g<=97){
                                        printf("A");
                                    }
                                    else{
                                        if (98<=g && g<=100){
                                            printf("A+");
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
        }
    }
}
### Exercise 6.4
#include <stdio.h>
char line[100];   
int  m,q,d,n,p,r; 
//I manage the quantity as 100 because I got confuse with int and float 
int main()
{
    printf("Enter the quantity of money less than $100: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &m);
    
    q = m / 25;
    r = m % 25;
    d = r / 10;
    r = r % 10;
    n = r / 5;
    r = r % 5;
    p = r / 1;
    
    printf ("The quarters you have %d, the dimes you have %d, the nickl you have %d and the pennys you have %d", q,d,n,p);
}
### Exercise 6.5
#include <stdio.h>
int main()
{
    int a;

    printf( "\n   Introduzca un a%co: ", 164 );
    scanf( "%d", &a );

    if ( a % 4 == 0 && a % 100 != 0 || a % 400 == 0 )
        printf( "Es bisiesto");
    else
        printf( "No es bisiesto");
}
### Exercise 6.6
#include <stdio.h>
char  line[100];   
int h;   
int m;
int s;

int main()
{
	s=8;
    printf("Enter the hours: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &h);
    if (h<=40){
    	m=h*s;
	}
	else{
	s=12;
	m = 320+(h-40)*s;
	}
	printf ("Your pay this week will be %d dolars", m);
}
### Exercise 6.7
#include <stdio.h>
char line[100];   
int  m,a,b,c,d; 

int main()
{
    printf("Enter the quantity of money you want to spend: ");
    fgets(line, sizeof(line), stdin);
    sscanf(line, "%d", &m);
    
    a = m / 15;
    b = m / 11;
    c = m / 6;
    d = m / 80;

    
    printf ("The chips you can buy %d or you can buy %d sodas or you can buy %d paletas lucas or you can buy %d pizzas", a,b,c,d);
}
