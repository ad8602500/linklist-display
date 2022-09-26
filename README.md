# linklist-display
Let's Code Recursive Display for Linked List
in c++ 
#include <iostream>
#include <bits/stdc++.h>

using namespace std;

class node{
    public:
    int data;
    node *next;
};

void Dispaly(node *p){
    if(p!=0){
        cout<<p->data<<" ";
        Dispaly(p->next);
    }
}


int main()
{
    node* head = NULL;
    node* second = NULL;
    node* third = NULL;
    head=new node;
    second=new node;
    third=new node;
    head->data=50;
    head->next=second;
    second->data=100;
    second->next=third;
    third->data=200;
    third->next=NULL;
    Dispaly(head);

    return 0;
}
