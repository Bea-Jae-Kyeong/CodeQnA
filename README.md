# CodeQnA
Making a Database using SQL statement from ERD Diagram in Database Foundations
The problem-solution web page is called ‘CodeQnA’.
<img src="https://github.com/Bea-Jae-Kyeong/CodeQnA/blob/main/erdplus-diagram.png?raw=true"></img>
Programmers are the clients of my web page. When they have an issue or a
problem, they can post their doubts on the page. They can also answer freely
when they know the solution to the problem. Users can search the posting by
tag. Tag is the key point of the posting so that other users can easily search.

Table USER_c has the information of the user on the web page. They are the
client of the developer. They have the user_id, email, user name, and password.
The username is used to identify themselves by nickname. We can know by
username who uploaded the posting. Email and password are used to log in.

user_id is a primary key to identify users and it increments automatically.
Users can post their problems they have met while coding, and also give a
solution to the problem. Users can answer below Problems posted, and every
user can access to read and give a rating to the problem.

Table PROBLEM has information about Problem. Users upload their problems to
be solved on the web page. Each problem has an id called pro_id which is
unique. And they have the title, and the date it was posted.
Each problem can have many solutions, because users have different
approaches to the problem.

Table SOLUTION has information about the Solution to the posted problem.
Users can post the solution below problem or rate the solution implemented. 
When users think the solution is the best answer to the problem, they can rate
it by giving up to 5 points for good answer, and 1 points for bad answer.

Table TAG consists of tag_id, and tag_name. The tag is for users to search for
the posting. tag_name is a programming language used in the problem. This
helps users to understand the format of the code explained. We can search for
the solution by selecting programming languages that we are considering. We
can select tag from 'C', 'C++', 'Python', 'JAVA', 'JAVASCRIPT', 'Perl', 'Ruby', 'C#'.

Table PROBLEM_TAG makes connection with the problem and the tag. Tag is
used to search posted problem.
