---
layout: essay
type: essay
title: "No Such Thing as Stupid Questions, or Is There?"
# All dates must be YYYY-MM-DD format!
date: 2024-09-12
published: true
labels:
  - Questions
  - Answers
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/Question.jpg">

## The Big Question

Is there such thing as a stupid question? With teachers and professors always encouraging students to ask questions and that there is no such thing as a stupid question, it would be hard to think otherwise. But this is not the case, as some questions result in the side eye of peers or a sarcastic remark from others. It all depends on the approach to a question. There are ways to build a question to avoid the unhelpful answers and ensure you get the help you need.


## The Smart Way to Ask a Question

During my search on the website Stack Overflow, a popular site where programmers can ask questions and receive feedback from other programmers, I was able to see both sides of the story. It was clear to see what attributes helped questions get helpful answers and what attributes led to questions being ignored. One question I stumbled upon was about how to use the hasNext() method from a scanner class in Java. If this sounds like a whole new language, you can think of it as a carnival ride worker looking for an open seat on the ride, and if there’s an open seat, then they let people onto the ride. Now let’s examine the question.

```
Question: How to use hasNext() from the Scanner class
Input Format

Read some unknown n lines of input from stdin(System.in) until you reach EOF; each line of input contains a non-empty String.

Output Format

For each line, print the line number, followed by a single space, and then the line content received as input:

Sample Output

Hello world
I am a file
Read me until end-of-file.  
Here is my solution. The problem being I am not able to proceed till EOF. But the output is just:

Hello world
Here is my code:

public class Solution {

    public static void main(String[] args) {
        check(1);  // call check method
    }

    static void check(int count) {          
        Scanner s = new Scanner(System.in);
        if(s.hasNext() == true) {
            String ns = s.nextLine();
            System.out.println(count + " " + ns);
            count++;
            check(count);
        }
    } 
}
```

Overall, this is a well built question that has the potential to be asked by other programmers learning java. The user provided their own code, their output, and their expected output. By providing these three things, it can help others to better understand the needs for the code and how to provide answers and solutions to the code.

```
Answer: Your code does not work because you create a new Scanner object in every recursive call. You should not use recursion for this anyways, do it iteratively instead.
Iterative version

public class Solution {

    public static void main(String[] args) {

        Scanner s = new Scanner(System.in);
        int count = 1;

        while(s.hasNext()) {
            String ns = s.nextLine();
            System.out.println(count + " " + ns);
            count++;
        }
    }
}
Recursive version

public class Solution {

    private Scanner s;

    public static void main(String[] args) {

        s = new Scanner(System.in); // initialize only once
        check(1);
    }

    public static void check(int count) {
        if(s.hasNext()) {
            String ns = s.nextLine();
            System.out.println(count + " " + ns);
            check(count + 1);
        }
    }   
}
```

The user was able to receive 13 potential answers for their question. I believe this is a smart question, especially with beginner programmers as it can be intimidating to learn a new language. I was in this position before and it is a relatable question.

## The Not so Smart Way

Let’s talk about not so smart questions. In this example, the user starts off with a broad topic question which can be a good starting point, but then they follow that up with providing a specific data set and an unclear expectation. 

```
Question: sampling unbalanced data frame columns
If I have a data frame df, which has five columns: 'A', 'B', 'C', 'D', and 'E', which contains python strings. Currently, 'B', 'C', 'D', and 'E' has unbalanced unique values (i.e., some unique values have more rows than the others). How can I sample df so that column 'B', 'C', 'D', and 'E' have balanced number of unique values (i.e., each unique value in a specific column has the same number of rows)? I want to sample with replacement so that the resulting data frame has the same length as the original data frame, though some rows may be duplicated and some may be omitted. Thanks!
```

The user was not able to fully explain their problem and left the whole question unclear. The only response to this question was to provide more information about the example and what the expected output should be.

## The Importance of Questions

All in all, asking questions is always helpful and shouldn’t be avoided. However, with that being said, it is important to format the question in a way that ensures a clear description of what is needed or what the expected outcome should be in order to receive quality feedback. Providing an insight to what you may have attempted already, or what your current code is looking like, will help the reader to better understand the question.
