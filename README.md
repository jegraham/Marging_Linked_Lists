# Merging_Linked_Lists

Inspiration "Merge two sorted linked lists" https://www.educative.io/blog/crack-amazon-coding-interview-questions

Given two sorted linked lists, merge them so that the resulting linked list is also sorted. Consider two sorted linked lists and the merged list below them as an example.


Questions 
---------------------------------------
- What values will be in the list? All numerical? 
- Will I need to consider negatives?
- Is it s adoubly linked list?

Assumptions 
---------------------------------------
- Will be positive numbers 0+ 
- The Linked Lists will be provided
- Linked Lists are sorted

Solutions
---------------------------------------
- Take one sorted list (A) and add the second (B) to it. Iterate through A and B. If the first value in B is between current and next pointer in List A then it will be added till the next value in B is greater then the next. Then will continue. This is most likely the best and only way of merging the lists. Time and Memory will both be O(n + m).

- Another option is to point the tail of one list to the head of the next and sort the list. This would be O((n+m)log(n+m)) for time.

Testcases
---------------------------------------
- Two empty lists 
- Negative Numbers - I shouldn't be so lazy and just consider this -- I guess the sort would cover this, right?
