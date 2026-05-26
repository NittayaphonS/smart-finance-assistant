Entry 1 – Debugging API Connection Logic

Artifact:

<img width="486" height="914" alt="image" src="https://github.com/user-attachments/assets/061d7238-86b0-49b1-927d-d66e1b4441ee" />

Initial Prompt: I ran this code in Google Colab using the hands_on_ai package, but I’m confused because it prints “connection successful” even though I see connection errors above it. Can you explain why this happens in beginner-friendly terms?

Improved Prompt: I’m building a Smart Finance Assistant in Google Colab using the hands_on_ai package. My try-except block prints “connection successful” even though the response contains “❌ Error: Connection error.” Please explain how the try-except block works in this situation and suggest a better way to validate the response.

Reflection: At first, I thought my code was broken because the notebook showed connection warnings. After asking AI for help, I learned that the `hands_on_ai` library handled the error internally and returned an error message instead of crashing the program. I improved my prompt by including the exact output and asking specifically about the `try-except` logic, which gave me a clearer explanation. This taught me that successful code execution does not always mean the API request actually worked.

