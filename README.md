# Binary-MinHeap Aidan Chavez and Ashlyn Storie SMC
Professor Das

Binary Min Heap Assignment for CS -222
Assignment Descriotion: 
For this assignment you must implement a Binary Heap. You can choose to do a Min Heap or a Max Heap. 
You can use an array-based implementation or a linked implementation. 
You can do it individually or as a pair. 
Your implementation must support the following methods: 
1. insert()
2. extract_min() or extract_max() - depending on your implementation
3. display() - to confirm that the Heap is working correctly. Use a display() similar to the one done for UBST in class. 

Report: 
Introduction / Setting the context:
We decided to use an array-based implementation to create our Binary Minimum Heap. In order to do so, we had to create an insert() method to allow new values to be added to the tree. We also created different getter functions, which would find the index of either a parent or child of an imputed value. This could help with the swapping necessary for a Min Heap. We also prioritized creating a display function using the same pattern from the in-class UBST code and an extract_min, which allowed us to present and remove the minimum value from the tree. When creating a Binary Min Heap, the key is to track the order of the values within your index so that it will correctly display itself. 

Problems Faced:
When we first started working on this code, we tried to do an array rather than an ArrayList, but this caused us to run into a consistent wall of how to remove values from the list. The only way we could fix that issue while still keeping it a more traditional array is to shift each value over individually. This did not seem very effective, so we switched to an arraylist. This also proved beneficial when dealing with not knowing what size array we would need. Another roadblock we hit was when dealing with swapping after removing the minimum. We had to try a few different approaches to calling the swap function before we finally figured out how to get the end value to go to the top (index 0) and then swap using our child functions rather than the parent function, as we had previously when creating the insert function. 

Testing Process:
The testing process highlighted a lot of the problems I mentioned above. We created a Driver class, which we used to check each method consistently. There ended up being a lot of random “System.out.println” s put in place to see where specifically an array went Out of Bounds or to make sure the correct number was picked up for the correct format. Some of those “System.out.println”’s were left in the code but simply commented out so that as we continued on, we could make sure new changes did not affect old code. One of the places we tested most consistently was when mapping out the extract_min portion of the code. It was necessary to determine the correct process for removing the minimum value and how things were swapped. 
