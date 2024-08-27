To create a deep copy of the original linked list we can use a map to establish a relationship between original nodes and their copied nodes.

We traverse the list first to create a copied node for each original node then traverse and establish the correct connections between the copied nodes similar to the arrangement of next and random pointers of the original pointers. In the end, return the head of the copied list obtained from the map.

Algorithm

Step 1:Initialise variables ‘temp’ as a pointer to the head of the original linked list to traverse it. Create an empty unordered_map, to map original nodes to their corresponding copied nodes.

Step 2: Iterate through the original linked list and for each node in the linked list create a new node with the same data value as the original data. Map the original node to its copied node in the map.

Step 3: Iterate through the original list again but this time connect the pointers of the copied nodes in the same arrangement as the original node.

Get the copied node corresponding to the original node using the map.
Set the next pointer of the copied node to the copied node mapped to the original node’s next node.
Set the random pointer of the copied node to the original node’s next node copied from the map.

Step 4: Return the head of the deep copied list which is obtained by retrieving the copied nodes mapped to the original head from the map.​
