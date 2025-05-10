# Simple Quiz Game

questions = [
    {
        "question": "What is the capital of France?",
        "options": ["A. Paris", "B. Berlin", "C. Rome", "D. Madrid"],
        "answer": "A"
    },
    {
        "question": "Which planet is known as the Red Planet?",
        "options": ["A. Earth", "B. Mars", "C. Jupiter", "D. Venus"],
        "answer": "B"
    },
    {
        "question": "Who wrote 'Harry Potter'?",
        "options": ["A. J.R.R. Tolkien", "B. Stephen King", "C. J.K. Rowling", "D. George R.R. Martin"],
        "answer": "C"
    },
    {
        "question": "What is the largest ocean on Earth?",
        "options": ["A. Atlantic", "B. Indian", "C. Arctic", "D. Pacific"],
        "answer": "D"
    }
]

def run_quiz():
    score = 0
    print("=== Welcome to the Quiz Game ===\n")
    for idx, q in enumerate(questions, 1):
        print(f"Q{idx}: {q['question']}")
        for option in q["options"]:
            print(option)
        answer = input("Your answer (A/B/C/D): ").strip().upper()

        if answer == q["answer"]:
            print("✅ Correct!\n")
            score += 1
        else:
            print(f"❌ Incorrect. The right answer was {q['answer']}.\n")

    print(f"🎉 You scored {score} out of {len(questions)}.")

if __name__ == "__main__":
    run_quiz()
# task3
