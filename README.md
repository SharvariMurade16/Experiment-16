# Experiment-16
## AIM
To use linked list in c++.

## Problem Statement
1.) To create a node in c++.

2.) To add node in c++.

## THEORY-
In C++, a linked list is a type of linear data structure that allows users to store data in non-adjacent memory locations. It is made up of a series of nodes, each containing two parts: a value for the data it holds and a pointer that links to the next node in the sequence. This article will cover the concept of linked lists, their implementation, and the different practical applications they serve.

 ## CODE-
 1) NODES-
```javascript
//Sharvari Murade
//23070123088
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
int main(){
    Link* l1 = new Link(6);
    cout << l1->data<<"   "<<l1->next;

}
```

2) ADDING NODES-
```javascript
//Sharvari Murade
//23070123088
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
void insert_head(Link* &head, int data){
    Link* new_node = new Link(data);
    new_node -> next= head;
    head = new_node;
}
void disp(Link*head){
    Link*temp = head;
    while (temp!= NULL){
        cout<<temp->data<<"->";
        temp = temp->next;

    }
    cout<<"NULL"<<endl;
}

int main(){
    Link*head = NULL;
    insert_head(head, 30);
    disp(head);
    insert_head(head, 32);
    disp(head);
    insert_head(head,35);
    disp(head);
    
}
```

## OUTPUTS-
1- <img width="344" alt="image" src="https://github.com/user-attachments/assets/d5567790-49db-4f76-8430-c8418b851428">

2- <img width="341" alt="image" src="https://github.com/user-attachments/assets/21801d10-0011-49e5-833f-c684576e4893">





