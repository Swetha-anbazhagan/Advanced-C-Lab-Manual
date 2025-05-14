EXP NO 26: C PROGRAM TO DISPLAY STACK ELEMENTS USING LINKED LIST.

Aim:

To write a C program to display stack elements using linked list.

Algorithm:

Define a structure Node with two members: data to store the integer value and next to point to the next node in the linked list.
Declare a global variable head representing the starting node of the linked list.
Define a function display to print the elements of the linked list.
Declare a pointer p and initialize it with the head of the linked list.
Use a while loop to traverse the linked list:
Print the data of the current node.
Move to the next node using the next pointer.
Program:
```
struct Node   
{  
float data;  
struct Node *next;  
}*head;  
void display()  
{ 
    struct Node *current=head;
    while(current!=NULL)
    {
         printf("%.2f\n",current->data);
        current=current->next;
    }
}
```
Output:

![437949501-e0c165b8-38cf-4664-b9ae-613614000676](https://github.com/user-attachments/assets/3a6ea9f4-396f-4c1b-b2c0-fc4f536886de)


Result:

Thus, the program to display stack elements using linked list is verified successfully.

EXP.NO 27: C PROGRAM TO POP AN ELEMENT FROM THE GIVEN STACK USING LINKED LIST.

Aim:

To write a C program to pop an element from the given stack using liked list.

Algorithm:

Check for Empty Stack
If head is equal to NULL, Print "Stack is empty."
Else Proceed to the next step.
Set head to point to the next node in the stack.
Program:
```
struct Node   
{  
    float data;  
    struct Node *next;  
}*head;  
void pop()  
{ 
    if(head!=0)
    {
        head=head->next;
    }
    else
    {
        printf("stack is empty");
    }
}
```
Output:

![437949691-eed7612f-e095-4dd1-bc99-a8e52d88d88a](https://github.com/user-attachments/assets/f29df0bb-8c27-48e3-b708-bc476087ba04)


Result: Thus, the program to pop an element from the given stack using liked list is verified successfully.

EXP NO:28 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING LINKED LIST.

Aim:

To write a C program to display queue elements using linked list.

Algorithm:

Check if Queue is Empty
Display Queue Elements
Print the data of the current node pointed to by front
Update front to point to the next node.
End the display function.
Program:
```
struct Node
{
    int data;
     struct Node *next;
}*front=NULL,*rear=NULL;
void display()
{
    struct Node *current=front;
    if(current==NULL)
    {
         printf("queue is empty");
    }
    else
    {
         printf("queue elements:\n");
         while(current!=NULL)
    {

         printf("%c\n",current->data);
         current=current->next;
    }
}
}
```
Output:

![437949936-ddc9d2d1-c13e-4b74-8858-4fd7c0c23b54](https://github.com/user-attachments/assets/06b9f545-7652-4db2-8ee1-5874313e62ba)


Result:

Thus, the program to display queue elements using linked list is verified successfully.

EXP NO:29 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING LINKED LIST

Aim:

To write a C program to insert elements in queue using linked list

Algorithm:

Allocate Memory for New Node
Set Data and Next Pointer
Check if Queue is Empty
Set both front and rear to point to the new node p.
Set the next pointer of the current rear to point to the new node p.
End of Enqueue Operation
Program:
```
struct Node
{
    int data;
    struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(int data)
{
    struct Node current = (struct Node)malloc(sizeof(struct Node));
    current->data = data;
    current->next = NULL;

    if (front == NULL)
    {
        front = rear = current;
    }
    else
    {
        rear->next = current;
        rear = current;
    }
}
```

Output:

![437950112-f72c26d0-172b-4367-b26e-1b9c73f3b42e](https://github.com/user-attachments/assets/36f2eccf-d15b-4f19-862a-0b83278f8267)


Result:

Thus, the program to insert elements in queue using linked list is verified successfully.

EXP NO:30 C FUNCTION TO FIND THE PEEK OF QUEUE USING LINKED LIST.

Aim:

The aim of this function is to retrieve the "peek" (the front element) of a queue implemented using a linked list

Algorithm:

Check if the queue is empty: o If the queue is empty (i.e., the front pointer is NULL), return an error or a message indicating that the queue is empty.
Access the front element: o If the queue is not empty, return the data stored in the front node of the linked list (i.e., the element at the head of the queue).
Program:
```
struct Node
{
   float data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void peek()
{
    if(front==NULL)
    {
        printf("queue is empty");
    }
    else
   {
        printf("%.2f",front->data);
   }
}
```
Output:

![437950271-eeb32fd4-d740-4d26-94f7-3ca7784d6e4a](https://github.com/user-attachments/assets/ca42e0a8-7c39-463f-aa86-bc7953064b6f)


Result:

Thus, the program to retrieve the "peek" (the front element) of a queue implemented using a linked list is verified successfully.

