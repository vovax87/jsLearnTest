Hi there!
This is the entrance exam for Android Academy’s “Node.js Fundamentals Course” 2021.
In order to register for the course this year you’ll need to submit your solution to this problem in javascript.
Need help? Don’t hesitate to e-mail us: academy.tlv@gmail.com
Question:
As part of our preparation for the upcoming course we would like to have an algorithm to calculate the top N students who attend the most lectures.
Write a function that receives:
students - An array of the names of all students who registered for the course (no duplicate names).
attendees -  A 2D array - each row represents a different lecture, and it’s content is an array of the attendees (i.e attendees[0] is an array of names who attend lecture #0).
N - The number of top students to return, and will always be equal to or less than the number of students who attend the lectures.
The function should return the top N students who attended the most lectures by descending order. 
const topNStudentsAttendees = (students, attendees, N) => {
	//TODO
}
Note:
Some of the attendees are mentors! You’ll need to verify that the attendees you return are only students from the array students.
Some attendees accidentally registered twice (or more) for the same lecture, make sure you don’t count a student more than once for the same lecture.
If some students attend the same amount of lectures you can decide their order as you like.
Write your answer in javascript!!

Example :
Input: students = [‘Eden’, ‘Refael’, ‘Yoni’, ‘Nitzan’, ‘Hadas’], attendees = [[‘Eden’, ‘Refael’, ‘Yoni’, ‘Nitzan’, ‘Hadas’, ‘Ortal’], 
 [‘Berry’, ‘Nitzan’, ‘Yoni’, ‘Eden’, ‘Hadas’, ‘Ortal’], 
 [‘Maxim’, ‘Ortal’, ‘Yoni’, ‘Refael’, ‘Nitzan’, ‘Alex’], 
            [‘Eden’, ‘Andrew’, ‘Yoni’, ‘Nitzan’, ‘Ortal’,‘Nitzan’]],
N = 3	
Output: [‘Yoni’, ‘Nitzan’, ‘Eden’]
N = 3, so we need to find the top 3 students who attend the most lectures.
Yoni and Nitzan attended 4 lectures and Eden attended 3 lectures. 
Ortal attended 4 lectures, but she’s not a registered student (she does not appear in the students array). Nitzan registered 5 times, but attended only 4 lectures. This is because she registered twice for the last lecture.
