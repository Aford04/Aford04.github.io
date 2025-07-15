# Random Guessing Game Flowchart

```mermaid
flowchart TD
    Start((Start)) --> Init[Initialize: Generate random number]
    Init --> Ask[Prompt user for guess]
    Ask --> Validate{Is input valid?}
    Validate -- No --> Error[Display error message] --> Ask
    Validate -- Yes --> Compare{Compare guess to number}
    Compare -- Too Low --> LowMsg["Display Too Low"] --> Ask
    Compare -- Too High --> HighMsg["Display Too High"] --> Ask
    Compare -- Correct --> Success[Display "Correct!"]
    Success --> End((End))
```

---

## 📝Description of Steps

1. **Start**: The program begins.
2. **Initialize**: A random number is generated within a specific range (e.g., 1 to 100).
3. **Prompt User**: The program prompts the user to guess a number.
4. **Validate Input**:
   - If the input is **not valid** (e.g., non-numeric or out of range), display an error message and ask again.
   - If the input **is valid**, proceed to compare the guess.
5. **Compare Guess**:
   - If the guess is **too low**, display a message and ask again.
   - If the guess is **too high**, display a message and ask again.
   - If the guess is **correct**, display a success message.
6. **End**: The game ends after the correct guess.

---


