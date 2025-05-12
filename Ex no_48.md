# EX 48 WRITE A FUNCTION TO SEARCH AN ELEMENT IN THE DOUBLE- LINKED LIST.
## AIM:
To write a C functions to perform all basic operations in Doubly Linked List.

## Algorithm
1.	Start.
2.	Define a variables.
3.	Write a function to search an element in the double linked list..
4.	Read the value using scanf.
5.	Ask the user to make an input.
6.	Print out the answer.
7.	End

## Program:
```
struct Node
{
struct Node *prev;
 struct Node *next;
 int data;
}*head;

void search(int data)
{
struct Node *temp;
int item=data,i=0,flag;
 temp=head;
 if(temp==NULL)
{
printf("Empty list\n");
}
else{
while(temp!=NULL)
{
if(temp->data == item)
{
 
printf("item %d found at location %d",item,i+1);
 flag=0;
}
i++;
temp=temp->next;
}
if(flag!=0)
{
printf("Item not found\n");
}
}

}

```

## Output:
![image](https://github.com/user-attachments/assets/589a069e-b723-493d-934a-7d7018f2adbb)



## Result:
Thus the program was executed and the output was verified successfully.
