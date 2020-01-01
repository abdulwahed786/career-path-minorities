---
title: "Queues"
metaTitle: "This is the title tag of this page"
metaDescription: "This is the meta description"
---

### Topics
1. Introduction to Queue
2. Implementation using Arrays and Linked List
3. C++ STL Queue
4. Introduction to Dequeue
5. C++ STL Dequeue

Usage Details for C++
Declaration ```queue<int> myQueue;```
Functions:
* Push new element: myQueue.push();
* Front element: myQueue.front():
* Pop front element: myQueue.pop();
* Last element: myQueue.back();
* Size of the queue: myQueue.size();
* Check Empty: myQueue.empty(); More details at http://www.cplusplus.com/reference/queue/queue/.
Usage Details for Java can be found at https://docs.oracle.com/javase/7/docs/api/java/util/Queue.html.


Double ended Queue
Declaration ```dequeue<int> dq;```
Functions:
* Push at back: dq.push_back();
* Delete from back: dq.pop_back();
* Push at front: dq.push_front();
* Delete from front: dq.pop_front();
* Size of the dequeue: dq.size();
* Check Empty: dq.empty(); More details at http://www.cplusplus.com/reference/deque/deque/.

Usage Details for Java can be found at https://docs.oracle.com/javase/7/docs/api/java/util/Deque.html.


Problems: https://www.hackerearth.com/practice/data-structures/queues/basics-of-queues/practice-problems/

hackerrank: https://www.hackerrank.com/domains/data-structures?filters%5Bsubdomains%5D%5B%5D=queues

interviewBit (both stack+queues):
https://www.interviewbit.com/courses/programming/topics/stacks-and-queues/