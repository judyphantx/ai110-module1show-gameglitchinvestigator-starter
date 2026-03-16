# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
 
1. When I first ran it, the game required the user to input a number in order to guess the computer's random generated number. 
If the number was to high or too low it would tell us. The design of the game included a Developer DeBug Info, input bar, and two buttons to "Submit" or start a "New Game" 

2. 
  1. The game's "New Game" Button does not work after I won or lost a game. The only way to restart was to refresh the entire app.
  2. I made a guess of "1" but the game told me to go lower. That is not possible since the range is from 1-100. Even at "0" it told me to go lower. 
     At "99" it told me to go higher. 
      The number was 69. Unable to recognize if number is too high or too low
  3. The game's hard mode is a range of 1 to 50 and normal mode is 1 to 100. It should be the other way around. Bigger range should be the harder difficulty.
  4. The range shown per a level did not reflect in the game. At all levels the rangee was 1 to 100, when it should have changed. 
  5. The number of attempts was 1 less than given. So at hard it should be 8, but only 7 were given. Same for Easy and Normal. 

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  I used Claude. 
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
AI suggested that  attempts starts at 1 instead of 0. Doing so adds an extra attempt to the user. So it is off by 1.This was an issue I already found in the game and I was able to check within the code to see if AI was correct about the error. Yes the error is there in the code. I updated the value from 1 to 0 and tested the game. The game's backend does count correctly, but the number displayed does not start counting down until attempt #2. 

- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
