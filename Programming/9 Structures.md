
Allows the user to have a collection of related items treated as one
```C
#include <string.h>

struct student{
	char name[10]';
	int id;
	
}

student.name;
strcpy(student.name,” JAMES”); 
student.box_no = 26;
strcpy (student.city,” MERU”);
student.phone_no = 20502;

```

```C
struct weatherdata {
	double temp;
	double rainfall; 
	double wind_velocity; 
	}data1, data2;
	// data1 and data2 are 2 different instances of weatherdata
```

<h3> Assigning pointers to structures</h3>
```C
struct weatherdata{
	double temp;
	double rainfall;
	double wind_velocity;
}data1[2],ptr* // Assigns a pointer to data1[2]

ptr->temp// will access the pointer variable
```

<h3> Type def </h3>
```C

typedef int kilometers;
```

<h4> fwrite( ) </h4>
```C
fwrite (* struct, size, count, file);

//we could write the entire structure with this command: 
fwrite (&my_acct, sizeof (struct account), 1, outfile);
//Given an array of 15 of these structures, struct account my_acct[15];
//we could write all 15 elements 
fwrite (my_acct, sizeof (struct account), 15, outfile);
```

<h4> fread ( ) </h4>
```C
fread (* struct, size, count, file);

```