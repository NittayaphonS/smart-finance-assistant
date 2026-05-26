Entry 1 – Debugging API Connection Logic

Artifact :

<img width="486" height="914" alt="image" src="https://github.com/user-attachments/assets/061d7238-86b0-49b1-927d-d66e1b4441ee" />

Initial Prompt: I ran this code in Google Colab using the hands_on_ai package, but I’m confused because it prints “connection successful” even though I see connection errors above it. Can you explain why this happens in beginner-friendly terms?

Improved Prompt: I’m building a Smart Finance Assistant in Google Colab using the hands_on_ai package. My try-except block prints “connection successful” even though the response contains “❌ Error: Connection error.” Please explain how the try-except block works in this situation and suggest a better way to validate the response.

Reflection: At first, I thought my code was broken because the notebook showed connection warnings. After asking AI for help, I learned that the `hands_on_ai` library handled the error internally and returned an error message instead of crashing the program. I improved my prompt by including the exact output and asking specifically about the `try-except` logic, which gave me a clearer explanation. This taught me that successful code execution does not always mean the API request actually worked.

Entry 2 – Generating Realistic Financial Test Data with AI

Artifact :

<img width="499" height="921" alt="image" src="https://github.com/user-attachments/assets/98faedaa-8715-447f-89b5-006476ee5690" />


Context: Using AI to create realistic Australian transaction data for testing CSV cleaning and spending analysis features.

Initial Prompt: Create sample transaction data for a Smart Finance Assistant project using pandas.

Improved Prompt: I’m building a Smart Finance Assistant for university students in Perth. Please generate realistic transaction data with Australian businesses, refunds, income transactions, and different spending categories. Include Date, Amount, Category, and Description columns, and format Amount values as strings with dollar signs so I can practice data cleaning in pandas.

Reflection: The first prompt produced generic sample data that was too simple for realistic testing. After improving the prompt with business context and technical requirements, the AI generated more useful financial data with refunds, income, and Australian businesses.
