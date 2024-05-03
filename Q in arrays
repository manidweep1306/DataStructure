/*implementatin of queue using arrays*/
#include<stdio.h>
#include<stdlib.h>
#define MAX 10
int queue[MAX];
int front=-1,rear=-1;
void insert(int);
void display();
void delete();
int main(){
	int item,choice;
	while(1){
		printf("\n....MENU...\n");
		printf("1.insert\n2.delete\n3.display\n4.exit\n");
		printf("enter your choice:");
		scanf("%d",&choice);
		switch(choice){
			case 1: printf("enter element to insert:\n");
				scanf("%d",&item);
				insert(item);
				break;
			case 2:delete();
				break;
			case 3:display();
				break;
			case 4:exit(0);
		}
	}
}
void insert(int item){
	if(rear==MAX-1)
	printf("queue is full\n");
	else{
		queue[++rear]=item;
		if(front==-1) front=0;
	}
}
void delete(){
	if(front==-1)
	printf("queue is empty\n");
	else{
		printf("deleted element=%d\n",queue[front]);
		if(front==rear)
		front=rear=-1;
		else
		front++;
	}
}
void display(){
	if(front==-1)
	printf("queue is empty\n");
	else{
		printf("Q content\n");
		for(int i=front;i<=rear;i++)
		printf("%4d",queue[i]);
	}
}
