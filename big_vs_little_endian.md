/* There are a number of ways for determining endiaanness of your device. */
/* Here is one quick way of testing endianness. */

#include <stdio.h>

int main() 
{
   unsigned int i = 1;
   char *c = (char*)&i;

   if (*c) {
       printf("Little endian");
   } else {
       printf("Big endian");
   }
   return 0;
}
