# COMP 440: Representing and Retrieving Knowledge

Claude writes your answers here as you say them. A sentence or two is enough for each. Your
Part 0 predictions stay as you first wrote them; Part 5 asks what you would change.

**Name:** Tu Tran
**Date:** October 20, 2026

## Part 0: Predictions

### Questions that name a character, place or thing: which method will do better, and why?

I think TF-IDF will do better since the questions contain specific words that may be unique to a movie and less likely to appear in other movies.

### Vague descriptions: which method will do better, and why?

I think embedding search will do better since the questions do not contain any specific words, so we need to match in terms of what it means.

## Part 1: Build the TF-IDF model

### The settings you chose, and why

- `REMOVE_STOP_WORDS = False`: I keep the current value because I think TF-IDF will handle common words.
- `MIN_MOVIES = 1`: I keep the current value because I want to keep words that are unique to a movie (for example, character's name).
- `REPEATS_COUNT_LESS = True`: I change it to True because I do not want some words to dominate the score.

## Part 2: Top terms

### Your movies: what do the top terms get right and wrong about what makes each one distinctive?

Coco: The top terms are the characters' names, but there is no words distinctive to the movie's plot like day of the death. Encanto: Similarly, the top terms are the characters' name and the setting of the movie, but they also do not reflect the movie's plot like magical family.

## Part 3: Your own searches

### Your questions, as you typed them

1. What is the movie about a boy who dreams of being a musician but his family has banned it due to a misunderstanding of his great-great-grandfather?
2. What is the colorful Pixar movie about a boy that somehow ends up in the world of the dead?
3. What is the movie with a boy named Miguel met and found out the truth about his great-great-granfather Hector while tried to find Ernesto de la Cruz to get out of the world of the dead?

### Did the movies you meant come up? What did TF-IDF get right and wrong?

The movie I meant (Coco) came up only in Question 3 (a detail question with specific word - characters' names). Thus, TF-IDF works well for detail questions with specific keywords while it does not get the movie right for reworded or vague questions.

## Part 4: The question bank

### Which kind of question did TF-IDF handle best, and which worst? By how much?

XXXX

### The misses you looked at: what do they have in common?

XXXX

## Part 5: Embeddings

### What is a sentence embedding, in your own words?

XXXX

### Where does each method do better, and why?

XXXX

### Your Part 0 predictions: which held, and which would you change?

XXXX

### How might you combine the two methods?

XXXX
