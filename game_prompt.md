I want to build a browser-based educational game to help Chinese medical students learn and remember medical English vocabulary.  
Please generate a complete `index.html` file using plain HTML + CSS + JavaScript (no frameworks).

GAME NAME:  
"Vocabulary Quest – 中英单词练习游戏"

GOAL OF GAME:  
Students practice matching 100 English medical terms with their correct Chinese translations.  
The game must support:  
- English → Chinese mode  
- Chinese → English mode  
- Randomized questions  
- Scoring  
- A timer option  
- Review mode

DATA:  
You may generate a sample list of 100 medical terms in a JavaScript array named `medicalWords`, each item structured like:
{
  english: "hypertension",
  chinese: "高血压"
}

REQUIREMENTS:

1. GAME MODES  
   - Mode A: “English → Chinese”  
   - Mode B: “Chinese → English”  
   - Mode C: “Flashcards Review Mode”  
   On the start screen, show 3 mode buttons.

2. GAMEPLAY (QUIZ MODES A & B)  
   - Show ONE word at a time (English or Chinese depending on mode).  
   - Provide 4 answer choices (multiple choice).  
   - Only ONE is correct; others must be randomly selected distractors.  
   - Give instant feedback (“Correct! 🎉” or “Wrong ❌”).  
   - After answering, automatically load the next word.  
   - Track score and total questions.  
   - After 20 questions, show “Final Score” screen.

3. FLASHCARD MODE (Mode C)  
   - Show English on front.  
   - Tap/click to flip to Chinese translation.  
   - Show “Next” and “Previous” buttons.  
   - Loop through all 100 terms.

4. UI REQUIREMENTS  
   - Bright, friendly colors.  
   - Large font for readability.  
   - Mobile-friendly responsive layout.  
   - Centered game container for consistent layout.

5. CODE STRUCTURE  
   - The ENTIRE game must be inside one file: `index.html`  
   - Include:  
     - `<style>` block for CSS  
     - `<script>` block for JavaScript  
     - `<div id="app">` main container  
   - Code must be clean and beginner-friendly.

6. AFTER GENERATING THE FILE  
   - Ask me if I want:  
     1) More words added  
     2) Hard mode (shorter answer time)  
     3) Audio pronunciation  
     4) Score saving using localStorage  

Before creating the file, explain your planned structure and ask for confirmation.
