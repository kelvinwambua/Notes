Instructional and global variables are stored in permanent storage area
Local variables are stored in the stack
Data structure  a group of related data items stored under the same name in memory

<h2>Memory allocation</h2>
```C
include <stdlib.h>
```
<h3>1. Malloc</h3>

This is a single memory block of any inbuild or user defined type

```C
#include <stdlib.h>
int main(){
X = (int*) malloc(100*sizeofint)// allocates enough for an array of 10 int
}
```

Malloc allocates a block contiguous bytes. Malloc can fail of the space allocated is not enough and will return null

```C
#include <stdlib.h>
int main(){
int *P, score, size;
printf("How many scores do you want to enter? ");
scanf("%d",size);
if ( score = (int *) malloc ( sizeof (int)) = = null)
{ 
	printf (“no space available \n”)’ 
	Exit (1); 
}
printf(” address of the first byte is %i \n”, score)
printf(” input the scores \n”) 
for(p = score; p<score; p++)
scanf(“ %i “,&p); 
printf(“%i is stored in address %i \n” * p,p);
return 0
}


```

<h3> Calloc</h3>
Calloc allocates multiple memory blocks

```C
#include <stdlib.h>
int main(){

struct student {
		char name[25]; 
		double age; 
		int reg_no; 
} 
typedet student record;
record *stp; 
int classNo = 30; 
stp = (record*) calloc (classNo, sizeof record);
}
```

<h3>Free</h3>
```C
free(ptr)
```
