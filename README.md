# Chapter5
Exercises chapter 5
## 5.1
```c
#include <stdio.h>

char line[100]; 
float fahrenheit;   
float centigrade; 
   

int main() {
	printf("Enter a temperature in centigrade: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%f", &centigrade);

	fahrenheit = ((9.0 / 5.0) * centigrade) + 32.0;
	printf("%f Fahrenheit.\n", fahrenheit);

	return(0);
}
```
## 5.2
```c
#include <stdio.h>

float radius;
float volume;    
char line[100];   

const float PI = 3.1416;

int main() {
	printf("Enter the radius: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%f", &radius);

	volume = (4.0 / 3.0) * PI * (radius * radius * radius);
	printf("The volume is %f.\n", volume);

	return(0);
}
```
## 5.3
```c
#include <stdio.h>

float width; 
float height;  
float perimeter;  
char line[100];    

int main() {
	printf("Height");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%f", &height);

	printf("Wwidth ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%f", &width);

	perimeter = 2.0 * (height + width);

	printf("Perimeter is %f\n", perimeter);

	return(0);
}
```
## 5.4
```c 
#include <stdio.h>

float kph;
float mph;  
char line[100]; 

int main() {
	printf("Enter kilometers: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%f", &kph);

	mph = (kph * 0.6213712);
	printf("%f miles\n", mph);

	return(0);
}
```
## 5.5
```c
#include <stdio.h>
char line[100];
int hours; 
int minutes;    
int total_minutes; 
const int MINPERHOUR = 60; 


int main() {
	printf("Enter hours: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%d", &hours);

	printf("Enter minutes: ");
	fgets(line, sizeof(line), stdin);
	sscanf(line, "%d", &minutes);

	total_minutes = minutes + (hours * MINPERHOUR);

	printf("Total: %d minutes.\n", total_minutes);

	return(0);
}
```
## 5.6
```c
#include <stdio.h>
int tot_mins;
int hrs;       
int mins;  
const int MINaHOUR = 60;    
char line_text[100];  

int main() {
	printf("Enter minutes: ");
	fgets(line_text, sizeof(line_text), stdin);
	sscanf(line_text, "%d", &tot_mins);

	hrs = (tot_mins / MINaHOUR);
	mins = (tot_mins % MINaHOUR);

	printf("%d Hours, %d Minutes.\n", hrs, mins);

	return(0);
}
```
## 5.7
```c
#include <stdio.h>

char line[100]; 
int value; 

int main() {
	printf("Enter a value: ");

	fgets(line, sizeof(line), stdin);
	sscanf(line, "%d", &value);

	printf("Twice %d is %d\n", value, value * 2);
	return(0);
}
```
