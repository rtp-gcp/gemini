# google AI Studio notes

system prompt controls the style of the answers.

* Respond in a short paragraph
* Respond as a haiku

# Base screen operations

## tokens

This is memory of the query and it represents a count of the various ways the prompt can be broken up.

Given the prompt "What is a dog" and another prompt "can you tell me about poodles?"

* character tokens
    - w, h, a, ...
* sentence tokens
    - what is a dog
    - can you tell me about poodles
* word tokens
    - what, is, a, ...
* subword tokens
    - a, bout

The token count contains the "system instructions", the "prompt/question" and the "response/answer".


## Temperature

This varies 0-1 (0-2 in reality) and determines how variable the answer/result is.  So if the same question is asked multiple times and the temperature is zero, then the result each time will be very similar.  If its 1, then the result will vary widely for the same questions/prompts.

It tends to give an commentary to the results, "You have asked a complex question", "that is a good question", etc.  It's almost like they are trying to be less dry and academic and more conversational in their
response.

## Stop sequence

This will stop the results right before the specified words are encountered.  The example
mentions using 6 to create lists of only 5 results.

## Safety

Safety settings control 

These settings can be 0-1 similar to the temperature setting
* hate speach
* harrassment 
* sexual
* dangerous

Block levels
* none
* low
* medium
* high


## Tuned models and structured prompts

Structured prompts are created using the tuned models operation.


You can provide a table on inputs and outputs.

You can upload images, but its hit or miss if it will work.  The video mentioned it only works with natural language but we got some results with one input column of text and one input column of images.  The output column had text.  When asking questions, it worked for some.  At one point we got an answer mentioning that it only works with images.  We could select the pro vision model and an internal error occured.

