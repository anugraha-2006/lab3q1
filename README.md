a)
Step 1: Create a new node
Step 2: Set new_node.data = new_data
Step 3: Set new_node.next = head
Step 4: Set head = new_node

b)
Step 1: Create a new node
Step 2: Set new_node.data = new_data
Step 3: Set new_node.next = NULL
Step 4: If head is NULL, set head = new_node and STOP
Step 5: Set temp = head
Step 6: While temp.next ≠ NULL, set temp = temp.next
Step 7: Set temp.next = new_node

c)
Step 1: Set temp = head
Step 2: While temp ≠ NULL and temp.data ≠ target_data, set temp = temp.next
Step 3: If temp = NULL, print "Node not found" and STOP
Step 4: Create new_node
Step 5: Set new_node.data = new_data
Step 6: Set new_node.next = temp.next
Step 7: Set temp.next = new_node

d) Insert Before a Given Node
Step 1: If head = NULL, STOP
Step 2: If head.data = target_data, call InsertAtBeginning(new_data) and STOP
Step 3: Set prev = NULL, curr = head
Step 4: While curr ≠ NULL and curr.data ≠ target_data:
           Set prev = curr
           Set curr = curr.next
Step 5: If curr = NULL, print "Node not found" and STOP
Step 6: Create new_node
Step 7: Set new_node.data = new_data
Step 8: Set new_node.next = curr
Step 9: Set prev.next = new_node

e) Delete from Beginning
Step 1: If head = NULL, print "List is empty" and STOP
Step 2: Set temp = head
Step 3: Set head = head.next
Step 4: Free temp

f) Delete from End
Step 1: If head = NULL, print "List is empty" and STOP
Step 2: If head.next = NULL:
           Free head
           Set head = NULL
           STOP
Step 3: Set temp = head
Step 4: While temp.next.next ≠ NULL, set temp = temp.next
Step 5: Free temp.next
Step 6: Set temp.next = NULL

g) Delete After a Given Node
Step 1: Set temp = head
Step 2: While temp ≠ NULL and temp.data ≠ target_data, set temp = temp.next
Step 3: If temp = NULL or temp.next = NULL, print "Deletion not possible" and STOP
Step 4: Set node_to_delete = temp.next
Step 5: Set temp.next = node_to_delete.next
Step 6: Free node_to_delete


h) Display / Traverse Linked List
Step 1: Set temp = head
Step 2: While temp ≠ NULL:
           Print temp.data
           Set temp = temp.next
i) Search for an Element
Step 1: Set temp = head, position = 1
Step 2: While temp ≠ NULL:
           If temp.data = target_data:
               Print "Element found at position", position
               STOP
           Set temp = temp.next
           Increment position by 1
Step 3: Print "Element not found"


j) Count the Number of Nodes 
Step 1: Set count = 0, temp = head
Step 2: While temp ≠ NULL:
           Increment count by 1
           Set temp = temp.next
Step 3: Return count

k) Reverse the Linked List
Step 1: Set prev = NULL, curr = head
Step 2: While curr ≠ NULL:
           Set next = curr.next
           Set curr.next = prev
           Set prev = curr
           Set curr = next
Step 3: Set head = prev
