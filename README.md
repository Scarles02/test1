exerice 1

int i ;

int main() {
	i = 0x60;
	my_aff_alpha();
	return 0;
}

int my_aff_alpha() {
if (i <0x7A){
i++;
printf ("%c ",i);
my_aff_alpha();}
return 0;
}

exercice 2

#include <stdio.h>
#include <stdlib.h>

int i ;

int main() {
	i = 0x7B;
	my_aff_realpha();
	return 0;
}

int my_aff_realpha() {
if (i >0x61){
i--;
printf ("%c ",i);
my_aff_realpha();
}
return 0;
}

exercice 3
#include <stdio.h>
#include <stdlib.h>

int i ;

int main() {
	i = -1;
	my_aff_chiffre();
	return 0;
}

int my_aff_chiffre() {
if (i < 9){
i++;
printf ("%d ",i);
my_aff_chiffre();
}
return 0;
}

exercice 4

#include <stdio.h>
#include <stdlib.h>

int i ;

int main() {
	printf("Ecris un nombre au hasard :");
	scanf ("%d",&i);
	my_aff_isneg(i);
	return 0;
}

int my_aff_isneg(int n) {
	if(n >= 0 ) {
		printf("P");
	}
	else {
		printf("N");
	}
return 0;
}

exercice 5

#include <stdio.h>
#include <stdlib.h>
int i, j, k;
int main() {
	i = 0;
	j = 1;
	k = 2;
	my_aff_comb();
	
}
int my_aff_comb() {
	if (100*i + 10*j + k <= 789){
		printf("%d%d%d ",i,j,k);
		if (k == 9){
			
			k = j + 2;
			
			if (j < 8 ){
				
				j = i + 2 ;
				
				if(i < 7){
					
					i++;
				} 
			}
		}
		else {
			k++;
		}
	my_aff_comb();	
	}
}
