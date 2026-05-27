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

Entry 4: Improving AI-Generated Python Code

Artifact:

<img width="478" height="949" alt="image" src="https://github.com/user-attachments/assets/50458586-3320-4f9c-898a-5d391b4e7fcb" />
<img width="482" height="459" alt="image" src="https://github.com/user-attachments/assets/90f82afc-5e34-4e46-91e7-a8b1635dcac9" />


Context:
I used AI to help create a data cleaning function for my Smart Finance Assistant project. The goal was to load CSV transaction data, clean dollar-sign values, and validate financial records safely.

Reflection:
The first AI response worked well but was slightly too complex for a beginner university project. Some parts, such as multiple try-except blocks, would be difficult to explain confidently in class.
Instead of using the code immediately, I refined my prompt to request a simpler and more beginner-friendly version. This taught me that AI-generated code should be reviewed carefully and adapted to match the developer’s own understanding level before being used in a project.

Entry 5: Refining AI Code for Simplicity

Artifact:
<img width="481" height="896" alt="image" src="https://github.com/user-attachments/assets/86ed4325-0e3e-4c85-8bcd-3a3a64da80ee" />


Context:
After reviewing the first AI-generated solution, I asked the AI to simplify the implementation so it would be easier to understand and explain during a class presentation.

Reflection:
The second AI response produced a much cleaner and more beginner-friendly version of the function. Advanced features such as type hints and multiple try-except blocks were removed, making the logic easier to follow step-by-step.

Entry 6: AI-Assisted Spending Analysis Function

Artifact:
<img width="490" height="577" alt="image" src="https://github.com/user-attachments/assets/b01c530a-c9f1-4992-a8f5-ee539df42be2" />
<img width="487" height="884" alt="image" src="https://github.com/user-attachments/assets/bd1ee2a7-e05b-4bc5-a152-1c15cd2b3354" />


Context:
I used AI to help create a spending analysis function for my Smart Finance Assistant project. The goal was to analyze spending categories, calculate percentages, and generate simple financial insights from cleaned transaction data.

Reflection:
The AI-generated function used simple pandas features like groupby() and sum() to organize spending data by category. I also learned how filtering expenses and using .abs() made the financial report easier to understand. This process showed me that AI can help turn raw transaction data into useful financial insights, but I still needed to review the logic to ensure it matched my project goals.

Entry 7: Reviewing AI-Generated Code Carefully

Artifact:
<img width="514" height="364" alt="image" src="https://github.com/user-attachments/assets/96b60417-12d5-4767-9d7d-6a42596b86bf" />


Context:
I used AI to help generate testing code for my spending analysis function in Google Colab.

Reflection:
While reviewing the AI-generated code, I noticed that the file name in the example (perth_student_spending.csv) did not match the actual CSV file name used in my notebook (student_transactions.csv). If I had copied the code directly without checking, the program would have failed because the file could not be found.

This experience taught me that AI-generated code should always be reviewed carefully before use. Even when the logic is correct, small inconsistencies between AI examples and the existing project code can still create errors. I learned the importance of checking variable names, file names, and project consistency instead of assuming AI outputs are automatically correct.

Entry 8: Improving AI-Generated Recommendation Logic

Artifact:
<img width="485" height="766" alt="image" src="https://github.com/user-attachments/assets/8fd02982-35b5-4608-8df0-ce67ba52c318" />
<img width="500" height="307" alt="image" src="https://github.com/user-attachments/assets/438eb6c9-d6d9-4c0b-8f4e-fadda4d5c227" />


Context:
I used AI to help create a recommendation system that generates financial advice based on spending analysis results.

Reflection:
The AI-generated function created personalized financial recommendations using simple conditional logic. While reviewing the code, I noticed the AI used a different test variable instead of my existing analysis data, so I corrected it to keep my notebook consistent. This reminded me to always review AI-generated examples carefully before using them.

Developer Diary – Entry 9: Debugging AI Chat Integration

Artifact:
<img width="485" height="842" alt="image" src="https://github.com/user-attachments/assets/9773656a-1c86-46fb-b7a5-1861faa657e1" />
<img width="487" height="907" alt="image" src="https://github.com/user-attachments/assets/97a3b549-6a55-4c6d-b70e-769ab92fb6e9" />


Context:
I used AI to help debug my finance chatbot integration using the hands-on-ai package.

My Prompt:
“I’m getting an error when testing my finance chatbot in Google Colab. I used `chat.say()` and now the chatbot is not working. Please explain the error in beginner-friendly language and suggest a simple fix that works with the hands-on-ai package.”

Reflection:
The AI explained that `chat.say()` was not a valid function in the hands-on-ai package and recommended using `get_response()` instead. After updating the code, the function error was fixed, but the notebook still returned a server connection error. This helped me understand that the project had two separate problems: an API usage issue and an external server connection issue. I learned the importance of separating coding errors from infrastructure problems when debugging AI systems.

Entry 10: Verifying RAG Functions Before Coding

Artifact:
<img width="490" height="364" alt="image" src="https://github.com/user-attachments/assets/b9f2f383-c10d-495e-b836-109f8d6aafa5" />
<img width="492" height="722" alt="image" src="https://github.com/user-attachments/assets/99fddcb4-90ed-40ed-94ff-0fe2bf3aa65b" />


Context:
I used AI to help plan the RAG section of my Smart Finance Assistant and checked the actual functions available in the hands_on_ai.rag package before using the code.

My Prompt:
I told Gemini the exact functions returned by dir(rag) and asked it to build a beginner-friendly RAG setup using only those functions. I also asked it not to invent unavailable functions such as rag.ask() or rag.load_document().

Developer Diary – Entry 11: Creating a Custom Savings Calculator Tool

Artifact:
<img width="495" height="809" alt="image" src="https://github.com/user-attachments/assets/8edcce85-a2a7-4e1e-a3e3-7a42fe7c19c8" />
<img width="492" height="796" alt="image" src="https://github.com/user-attachments/assets/90a72610-9fef-4deb-8a05-3f0ccd593e32" />


Context:
I used AI to help create a custom financial tool for calculating how long it will take a user to reach a savings goal.

My Prompt:
I asked Gemini to create a beginner-friendly savings calculator with inputs for current savings, monthly contribution, and target amount. I also asked it not to invent hands-on-ai agent registration code unless it was sure of the correct API.

Reflection:
The AI produced a clear savings calculator function with useful input validation, including checks for negative values and zero monthly contributions. I decided to use the Python function but not register it with the agent system yet because I had not verified the exact `hands_on_ai.agent` API. This taught me to separate working Python logic from library-specific integration code.

Reflection:
This helped me understand that RAG works by loading text, splitting it into chunks, creating embeddings, and retrieving the most relevant information for a user question. I also learned that AI-generated code must be checked against the actual library API before use. By running dir(rag) first, I avoided copying code that used non-existent functions.

