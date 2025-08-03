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
