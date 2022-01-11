# Stack Cheat Sheet

## Common Terms

1. **Push**: Nodes or items that are put into a stack are pushed, O(1)
2. **Pop**: Removing nodes or items using the pop method
3. **Top**: the top of the stack
4. **Peek**: Shows the value of the top node on the stack

## FILO

- First In Last Out: This means the first item in the stack will be the last item popped out

## LIFO

- Last In First Out: This means the last item in will be the first item out

## Pushing

1. Identify the *Node* you want to add
2. Set *Next* to current top *Node*
3. Reassign *Top* ref to new *Node*

- Code:
    `push(value)`
        `node = new Node(value)`
        `node.next = Top`
        `Top = node`

## Pop

1. Create a ref named *temp* that is the *Top* Node you want to remove
2. Reassign *Top* to the variable *Next* of your *temp* node
3. Set the *temps* *Next* variable to *NULL*
4. Return *temp*

- Code:
    `pop(value)`
        `Node temp = top`
        `top = top.next`
        `temp.next = null`
        `return temp.value`

## Peek

- Code:
    `peek()`
        `return top.value`
- Will throw exception if stack is empty

# Queues Cheat Sheet

## Common Terms

1. **Enqueue**: Nodes or items that are added to the queue
2. **Dequeue**: Removed nodes or items
3. **Front**: the first item in the queue
4. **Rear**: the last item in the queue
5. **Peek**: View the first item
6. **IsEmpty**: returns true when empty and false when populated

## FIFO

- First In First Out: This means the first item in the stack will be the first item out

## LILO

- Last In Last Out: This means the last item in will be the last item out

## Enqueue

- Code:
    `enqueue(value)`
        `node = new Node(value)`
        `rear.next = node`
        `rear = node`

## Dequeue

- Code:
    `dequeue()`
        `node_temp = front`
        `front = front.next`
        `node_temp.next = NULL`
        `return node_temp.value`

## Peek

- Code:
    `peek()`
        `return front.value`
- Will throw exception if stack is empty

# Useful Links

- [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)