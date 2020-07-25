# Thinking like a chatbot

With great power comes great responsibility. And with great traffic comes great conversations, or at least lots of conversations. One of our ventures in Nigeria has been growing leaps and bounds since we went live in December last year. Along with the user base, the number of people reaching out to the customer support teams has also been growing. And what better opportunity to express my love for automation at this problem.

I decided to spin up a chatbot. I had a theoretical understanding of how chat bots work but then there is a reason why the word "experience" was invented. I wanted to take this opportunity to not just apply and improve my learning but also to create a lucid guide to understand deeper concepts and best practices in creating chat bots.

## Basics

First the basics. Feel free to skip this section if you understand chat bots WELL. Else no harm spending 10 minutes revising your concepts.

A chatbot draws on the concept of how a dialog in a natural language is constructed There are following key concepts in a chatbot:

- Context
- Intent
- Utterance
- Entity

Let's take an example of a dialog between a girl called Cherry and a cafe waiter called Happy (as written on his nameplate).

```english
Cherry: Hey, Are you Happy?

Happy: Yes, I am Happy.

Cherry: Can I get a juice?

Happy: Sure, would you like orange?

Cherry: Yes, I love orange.

Happy: Great, I can serve it in a jug or paper cup

Cherry: I'll take a paper cup

Happy: Should I serve in a green cup?

Cherry: No, Do you have any other color?

Happy: Sure, would you like orange?

Cherry: No way, I hate orange. Are you feeling ok?

Happy: Yes, I am feeling ok.

Cherry: Are you happy?

Happy: Nah actually I am sad.
```

Now we will use the above story to understand the key parts of a conversation which matter in chatbot development.

## Intent

An Intent is an option from the set of expected objectives a user could have when interacting with someone or a chatbot. Taking the above conversation example, we can see that Cherry had the following set of intentions:

```english
Confirm name: Hey, Are you Happy?

```

## Context

There's something more interesting about this conversation. Both Happy and Cherry answer the same question differently in a different **Context**. Cherry loves orange juice but hates the color orange. Though Happy's question was the same in both situations: `Sure, would you like orange?`, Cherry could understand what he meant. How? Because she remembered what the previous conversation was about and *connected* that conversation with this question to completely comprehend what Happy meant to ask.

This is what Context does; it establishes a link between conversations. Hence, if we include a set of values as *context* each time Happy asks `Sure, would you like orange?` then we can complete the picture and present this as a question, without the need to specify the history of the conversation.

```english
Context 1: Select color, Select utensil
Statement 1: Sure, would you like orange?

Context 2: Select fruit, Select drink
Statement 2: Sure, would you like orange?
```

As you can see from the statements above, the context helps understand what the statement is about? It can also be seen as a set of play cards which help you retain the complete background of the conversation. It helps the user stay focused on the specific topic or subject the conversation is about.

This was important, hence so much time for this. Once you are clear about Context, what follows is a lot simpler.
