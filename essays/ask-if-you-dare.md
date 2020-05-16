---
layout: essay
type: 
title: Ask If You Dare  
# All dates must be YYYY-MM-DD format!
date: 2020-01-30
labels:
  - Smart Questions
  - Software Engineering
---

<img class="ui small floated image" src="../images/questionmark.gif">

## Feel free to ask...on one condition 
We are always told never to be hesitant when asking questions, as questions are a definitive way to clarify one's understanding of things. However, this isn’t exactly to say for “dumb” questions, and Raymond's article gives scornful criticism to these types of questions as he addresses this topic. While it is important to ask questions, it is also crucial that the question is formulated in the best possible way so that it could be beneficial to not only the asker but to other people in the community as well. Often, trivial questions could do us more harm than good and could even be aggravating for software engineers who choose to voluntarily help. Formulating a question requires much thought and skill, and one question alone could even alter a person's reputation. This not only applies to the field of computer science but everyday life as well. 

## What is the Importance Anyway?
When stumped, we instinctively want immediate solutions to be relieved of the struggle, and because we demand quick answers, it is easy to e-mail an expert about it or post the question on any forum. Sometimes, answers to simple questions can be received in a matter of seconds. However, this type of approach in solving problems goes against Raymond's guide to asking practical, "smart" questions. Sure, you may get the answer to your question, but was there any benefit from it? Was there careful deliberation or any research put into it beforehand? Is it in the corresponding category? Otherwise, it would be an entirely different matter posting a question to a forum wholly irrelevant to the topic at hand. Not only would it upset software engineers like Raymond it is also disrespectful to the programming community and to those who may have already answered the question in another forum. There are a series of precepts to follow before posting to a forum, and Raymond provides these in the "When You Ask" section of his essay. Below are examples of what to do or not to do when reaching out to the community of experts. 

## Smart
This [user](https://stackoverflow.com/questions/1642028/what-is-the-operator-in-c) has read and referenced a source material, and he has included a snippet of code for the '-->' operator that he is confused about as follows. 
```C
#include <stdio.h>
int main()
{
    int x = 10;
    while (x --> 0) // x goes to 0
    {
        printf("%d ", x);
    }
}
```
The question is specific, and he has tested this in other environments in a curious attempt.  While this is merely a question about conditionals, it does show that the user is respectful of others in that he has researched elsewhere in an attempt to find an operator that involves '-->', which is later clarified by another user that it is not an operator, but two separate operators, '--' and '>' to compare x-- with 0 by the '>' operator. The question is also clear, concise with no grammatical errors. The answers to this forum has easily clarified the confusion and is provided with many different examples to differentiate the operators and better understand the statement, e.g.,  

```
while( (x--) > 0 ).
```

## Not Smart
A question that may go against Raymond's standards as a "smart" question is one that pastes his entire code and expects that someone will find his errors, like this [user](https://stackoverflow.com/questions/59999155/why-am-i-getting-iresult-value-right-shifted). His code is included as follows: 
```C
int main()
{
    unsigned int Iresult = 0x5500, Icount ;
    
    printf("before\n");
    for(Icount = 31; Icount != 0; Icount--)
    {
        printf("%d",( (Iresult >> Icount) & 1) );
    }

        printf("%d",( (Iresult >> 0) & 1) );
    printf("\n");

    Iresult =   ( ( (unsigned char *) &Iresult )[1] << 1  ) ;

    printf("after\n");
    for(Icount = 31; Icount != 0; Icount--)
    {
        printf("%d",( (Iresult >> Icount) & 1) );
    }
        printf("%d",( (Iresult >> 0) & 1) );
    printf("\n");

}
```

This user may not have thoroughly researched the web or practiced the concepts before posting his question because he assumes that he is performing a left shift, and is resulting in a right shift instead. He also does not indicate explicitly in the code the possible cause of errors nor does he say where he did his shifts, making it difficult for responders to pinpoint the problem in this broad question. Moreover, the question is typed sloppily without grammatical corrections, which gives off a bad impression.

## Insights for the future
This article is to help me formulate questions that will help me succeed as a programmer as I progress as a CS student. In a fast-paced world where technology and code are always changing and advancing, it is only vital that we learn how to ask smarter questions to better communicate with other software engineers. Clever questions assist us in developing our critical thinking abilities. Also, the last thing that engineers want is to be bogged with spam e-mails with questions that could simply be answered with a Google search. We could do them a favor and not clog up their inboxes, and ourselves a favor if we had put more effort before asking the question.
