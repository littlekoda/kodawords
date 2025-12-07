I want to build a browser-based educational game to help Chinese medical students learn and remember medical English vocabulary.

Please generate a complete `index.html` file using plain HTML + CSS + JavaScript (NO frameworks).

===========================================================
GAME NAME:
"Vocabulary Quest – 中英单词练习游戏"
===========================================================

The game must contain FOUR modes:

-----------------------------------------------------------
MODE A: English → Chinese Multiple Choice Quiz
-----------------------------------------------------------
• Show one English medical term.
• Speak out the English word using Web Speech API.
• Provide 4 answer choices (Chinese).
• Only one is correct; 3 must be random distractors.
• Give instant “Correct! 🎉” or “Wrong ❌”.
• After answering, automatically load the next question.
• Track score and total questions.
• After 20 questions → show Final Score page.

-----------------------------------------------------------
MODE B: Chinese → English Multiple Choice Quiz
-----------------------------------------------------------
• Show one Chinese medical term.
• Provide 4 possible English translations.
• Speak out the chosen English answer.
• Same scoring and final screen as Mode A.

-----------------------------------------------------------
MODE C: Flashcard Review Mode
-----------------------------------------------------------
• Show English on front.
• When English is shown, speak it out.
• Tap/click flips card to Chinese.
• Buttons: “Next”, “Previous”.
• Loop through all 100 terms.

-----------------------------------------------------------
MODE D: Paragraph Fill-in Game (NEW – integrate previous prompt)
-----------------------------------------------------------
Goal:
Students read a short paragraph where 3 vocabulary words are removed and replaced with blanks. They must fill the blanks in the correct order.

Mechanics:
1. From the 100-word vocabulary list:
   - Randomly select 3 distinct English words.
   - Generate a short natural paragraph (2–3 sentences) that includes these 3 English words.
2. Replace each selected word with a blank placeholder “____”.
3. Display the paragraph with blanks.
4. Below the paragraph, show 3 word buttons in random order.
5. Cursor automatically highlights the FIRST blank.
6. User clicks a word:
   - If correct → fill the blank, move focus to next blank.
   - If wrong → shake animation or red highlight; stay on current blank.
7. After all blanks are correctly filled:
   - Show a message “Correct! Generating next paragraph…”
   - Automatically start a new round (new 3 words + new paragraph).
8 - The format of this section is correct, and I intended to fill in the blanks this way. However, the problem is that this paragraph lacks a medical background; the sentences within it are not logically related from a medical perspective. I hope that after filling in the correct words, this paragraph will make sense medically.

Additional UI rules:
• Large readable blanks.
• Mobile-friendly.
• Highlight active blank.
• Shuffle answer words every round.
• Avoid repeating the same paragraph too often.

-----------------------------------------------------------
DATA (shared by all 4 games)
-----------------------------------------------------------
Generate a sample list of 100 medical terms:

medicalWords = [
  { english: "hypertension", chinese: "高血压" },
  { english: "fracture", chinese: "骨折" },
  ...
];

-----------------------------------------------------------
UI REQUIREMENTS
-----------------------------------------------------------
• Start screen shows 4 big mode buttons:
    A: 英 → 中
    B: 中 → 英
    C: Flashcards
    D: Paragraph Fill
• Bright, friendly colors.
• Large readable text, mobile-friendly.
• All screens rendered inside:
      <div id="app"></div>
• Clean, organized layout.

-----------------------------------------------------------
TECHNICAL REQUIREMENTS
-----------------------------------------------------------
• Entire game MUST be inside ONE file: index.html
• Use:
    <style> for CSS
    <script> for JavaScript
• Use Web Speech API for English audio.
• No external libraries.
• Code must be clear, modular, and well-commented.
• Allow easy future expansion.

-----------------------------------------------------------
AFTER GENERATING THE FILE
-----------------------------------------------------------
Ask me if I want:
1) More vocabulary words
2) Hard mode (shorter answer time)
3) Better paragraph generation
4) Saving progress using localStorage
