//Total Floors = 65
//Elevator can go 8 floors up at a time
//or 11 floors down at a time.Every floor must be accessed on one time?
//Does it have access to all 65 floors?


#include <stdio.h>
#include <stdint.h>


int main()
{
	int array[66];
	for (int i = 1; i < 66;i++)
	{
		array[i] = 0;
		printf("Array %d is %d\n\r", i ,array[i]); 
		//filling the array with all zeros
	}
	printf("\n\r------------------------------------------------\n\r");
	int position = 1;
	int count = 0;
	array[position] = 0;
	array[position]++;
	
	for (int i = 0; i < 8; i++)
	{
		printf("Incrementing operation\n\r");
		do
		{
			position = position + 8;
			if (array[position] == 0)
			{
				count++;
				array[position]++;
				if (position < 65)
					printf("Floor %d is %d\n\r", position, array[position]);
			}

		} while (position < 65);

		printf("---------------------------------------------\n\r");
		if (position >= 65 || array[position] > 0)
		{
			position = position - 8;
		}
		
		printf("Decrementing operation\n\r");
		do
		{
	
			position = position - 11;
			if (array[position] == 0)
			{
				count++;
				array[position]++;
				if (position > 0)
					printf("Floor %d is %d\n\r", position, array[position]);
			}
		} while (position > 0);

		if (position < 0 || array[position] > 0)
		{

			position = position + 11;
		}
		printf("---------------------------------------------\n\r");
	}
	for (int i = 1; i < 66; i++)
	{
		if(array[i] == 0)
		printf("Floor %d is %d\n\r", i ,array[i]);	
	}
	
	return 0;
}
