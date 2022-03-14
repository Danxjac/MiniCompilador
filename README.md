# MiniCompilador


#code source


PRINT "How many fibonacci numbers do you want?"
INPUT nums
PRINT ""

LET a = 0
LET b = 1
WHILE nums > 0 REPEAT
    PRINT a
    LET c = a + b
    LET a = b
    LET b = c
    LET nums = nums - 1
ENDWHILE


after compilacion in c

#include <stdio.h>
int main(void){
float nums;
float a;
float b;
float c;
printf("How many fibonacci numbers do you want?\n");
if(0 == scanf("%f", &nums)) {
nums = 0;
scanf("%*s");
}
printf("\n");
a = 0;
b = 1;
while(nums>0){
printf("%.2f\n", (float)(a));
c = a+b;
a = b;
b = c;
nums = nums-1;
}
return 0;
}
