#include <stdio.h>
#include <stdlib.h>

int tesrt();


struct Node {
   int data;
   struct NodeList *follower;
};

struct NodeList {
   struct Node node;
   struct Node *next;
};


struct Node createNode(){
   struct Node lMeinGraph;
   lMeinGraph.data = 5;
   return lMeinGraph;
}

struct Node addFollowerNode(struct Node node){
   struct Node newNode;
   newNode.data = 9;
   newNode.follower = NULL;

   if(node.follower==NULL){
     struct NodeList newNodeList;;
     newNodeList.node = newNode;
     newNodeList.next = NULL;

     node.follower = &newNodeList;
   }
   //fehlt noch


   return node;
}

struct Node getFirstNodeFromNodeList(struct NodeList list){
   return list.node;
}

int getDataFromNode(struct Node node){
   return node.data;
}

//Achtung: Kann nur zusammenhängende gerichtete Graphen erstellen.
int main(void) {
   struct Node meinGraph = createNode();
   printf("%d\n",meinGraph.data);



   meinGraph = addFollowerNode(meinGraph);

     printf("Hello World\n");


printf("%d\n",getDataFromNode(getFirstNodeFromNodeList(*meinGraph.follower)));


   return 0;

}
