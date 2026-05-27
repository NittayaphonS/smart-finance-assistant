Connection Test - Entry 1: Debugging API Connection Logic

Artifact :

<img width="486" height="914" alt="image" src="https://github.com/user-attachments/assets/061d7238-86b0-49b1-927d-d66e1b4441ee" />

Initial Prompt: I ran this code in Google Colab using the hands_on_ai package, but I’m confused because it prints “connection successful” even though I see connection errors above it. Can you explain why this happens in beginner-friendly terms?

Improved Prompt: I’m building a Smart Finance Assistant in Google Colab using the hands_on_ai package. My try-except block prints “connection successful” even though the response contains “❌ Error: Connection error.” Please explain how the try-except block works in this situation and suggest a better way to validate the response.

Reflection: At first, I thought my code was broken because the notebook showed connection warnings. After asking AI for help, I learned that the `hands_on_ai` library handled the error internally and returned an error message instead of crashing the program. I improved my prompt by including the exact output and asking specifically about the `try-except` logic, which gave me a clearer explanation. This taught me that successful code execution does not always mean the API request actually worked.

____

Sample Transaction Data Setup - Entry 2: Generating Realistic Financial Test Data with AI

Artifact :

<img width="499" height="921" alt="image" src="https://github.com/user-attachments/assets/98faedaa-8715-447f-89b5-006476ee5690" />


Context: Using AI to create realistic Australian transaction data for testing CSV cleaning and spending analysis features.

Initial Prompt: Create sample transaction data for a Smart Finance Assistant project using pandas.

Improved Prompt: I’m building a Smart Finance Assistant for university students in Perth. Please generate realistic transaction data with Australian businesses, refunds, income transactions, and different spending categories. Include Date, Amount, Category, and Description columns, and format Amount values as strings with dollar signs so I can practice data cleaning in pandas.

Reflection: The first prompt produced generic sample data that was too simple for realistic testing. After improving the prompt with business context and technical requirements, the AI generated more useful financial data with refunds, income, and Australian businesses.

____

Foundation Data Processing Functions - Entry 3: Improving AI-Generated Python Code

Artifact:

<img width="478" height="949" alt="image" src="https://github.com/user-attachments/assets/50458586-3320-4f9c-898a-5d391b4e7fcb" />
<img width="482" height="459" alt="image" src="https://github.com/user-attachments/assets/90f82afc-5e34-4e46-91e7-a8b1635dcac9" />


Context:
I used AI to help create a data cleaning function for my Smart Finance Assistant project. The goal was to load CSV transaction data, clean dollar-sign values, and validate financial records safely.

Reflection:
The first AI response worked well but was slightly too complex for a beginner university project. Some parts, such as multiple try-except blocks, would be difficult to explain confidently in class.
Instead of using the code immediately, I refined my prompt to request a simpler and more beginner-friendly version. This taught me that AI-generated code should be reviewed carefully and adapted to match the developer’s own understanding level before being used in a project.

___

Load and Clean Transaction Data(file_path) - Entry 4: Refining AI Code for Simplicity

Artifact:

<img width="481" height="896" alt="image" src="https://github.com/user-attachments/assets/86ed4325-0e3e-4c85-8bcd-3a3a64da80ee" />


Context:
After reviewing the first AI-generated solution, I asked the AI to simplify the implementation so it would be easier to understand and explain during a class presentation.

Reflection:
The second AI response produced a much cleaner and more beginner-friendly version of the function. Advanced features such as type hints and multiple try-except blocks were removed, making the logic easier to follow step-by-step.

___

Analyze Spending Patterns(df) - Entry 5: AI-Assisted Spending Analysis Function

Artifact:

<img width="490" height="577" alt="image" src="https://github.com/user-attachments/assets/b01c530a-c9f1-4992-a8f5-ee539df42be2" />
<img width="487" height="884" alt="image" src="https://github.com/user-attachments/assets/bd1ee2a7-e05b-4bc5-a152-1c15cd2b3354" />


Context:
I used AI to help create a spending analysis function for my Smart Finance Assistant project. The goal was to analyze spending categories, calculate percentages, and generate simple financial insights from cleaned transaction data.

Reflection:
The AI-generated function used simple pandas features like groupby() and sum() to organize spending data by category. I also learned how filtering expenses and using .abs() made the financial report easier to understand. This process showed me that AI can help turn raw transaction data into useful financial insights, but I still needed to review the logic to ensure it matched my project goals.

___

Entry 6: Reviewing AI-Generated Code Carefully

Artifact:

<img width="514" height="364" alt="image" src="https://github.com/user-attachments/assets/96b60417-12d5-4767-9d7d-6a42596b86bf" />


Context:
I used AI to help generate testing code for my spending analysis function in Google Colab.

Reflection:
While reviewing the AI-generated code, I noticed that the file name in the example (perth_student_spending.csv) did not match the actual CSV file name used in my notebook (student_transactions.csv). If I had copied the code directly without checking, the program would have failed because the file could not be found.

This experience taught me that AI-generated code should always be reviewed carefully before use. Even when the logic is correct, small inconsistencies between AI examples and the existing project code can still create errors. I learned the importance of checking variable names, file names, and project consistency instead of assuming AI outputs are automatically correct.

___

Generate Financial Rrecommendations(analysis_data) - Entry 7: Improving AI-Generated Recommendation Logic

Artifact:

<img width="485" height="766" alt="image" src="https://github.com/user-attachments/assets/8fd02982-35b5-4608-8df0-ce67ba52c318" />
<img width="500" height="307" alt="image" src="https://github.com/user-attachments/assets/438eb6c9-d6d9-4c0b-8f4e-fadda4d5c227" />


Context:
I used AI to help create a recommendation system that generates financial advice based on spending analysis results.

Reflection:
The AI-generated function created personalized financial recommendations using simple conditional logic. While reviewing the code, I noticed the AI used a different test variable instead of my existing analysis data, so I corrected it to keep my notebook consistent. This reminded me to always review AI-generated examples carefully before using them.

___

Chat Interface Integration – Entry 9: Debugging AI Chat Integration

Artifact:

<img width="485" height="842" alt="image" src="https://github.com/user-attachments/assets/9773656a-1c86-46fb-b7a5-1861faa657e1" />
<img width="487" height="907" alt="image" src="https://github.com/user-attachments/assets/97a3b549-6a55-4c6d-b70e-769ab92fb6e9" />


Context:
I used AI to help debug my finance chatbot integration using the hands-on-ai package.

My Prompt:
“I’m getting an error when testing my finance chatbot in Google Colab. I used `chat.say()` and now the chatbot is not working. Please explain the error in beginner-friendly language and suggest a simple fix that works with the hands-on-ai package.”

Reflection:
The AI explained that `chat.say()` was not a valid function in the hands-on-ai package and recommended using `get_response()` instead. After updating the code, the function error was fixed, but the notebook still returned a server connection error. This helped me understand that the project had two separate problems: an API usage issue and an external server connection issue. I learned the importance of separating coding errors from infrastructure problems when debugging AI systems.

___

RAG System for Financial DocumentsEntry 10: Verifying RAG Functions Before Coding

Artifact:

<img width="490" height="364" alt="image" src="https://github.com/user-attachments/assets/b9f2f383-c10d-495e-b836-109f8d6aafa5" />

<img width="492" height="722" alt="image" src="https://github.com/user-attachments/assets/99fddcb4-90ed-40ed-94ff-0fe2bf3aa65b" />


Context:
I used AI to help plan the RAG section of my Smart Finance Assistant and checked the actual functions available in the hands_on_ai.rag package before using the code.

My Prompt:
I told Gemini the exact functions returned by dir(rag) and asked it to build a beginner-friendly RAG setup using only those functions. I also asked it not to invent unavailable functions such as rag.ask() or rag.load_document().

___

Custom Financial Tools – Entry 11: Creating a Custom Savings Calculator Tool

Artifact:

<img width="495" height="809" alt="image" src="https://github.com/user-attachments/assets/8edcce85-a2a7-4e1e-a3e3-7a42fe7c19c8" />

<img width="492" height="796" alt="image" src="https://github.com/user-attachments/assets/90a72610-9fef-4deb-8a05-3f0ccd593e32" />


Context:
I used AI to help create a custom financial tool for calculating how long it will take a user to reach a savings goal.

My Prompt:
I asked Gemini to create a beginner-friendly savings calculator with inputs for current savings, monthly contribution, and target amount. I also asked it not to invent hands-on-ai agent registration code unless it was sure of the correct API.

Reflection:
The AI produced a clear savings calculator function with useful input validation, including checks for negative values and zero monthly contributions. I decided to use the Python function but not register it with the agent system yet because I had not verified the exact `hands_on_ai.agent` API. This taught me to separate working Python logic from library-specific integration code.

___

Gradio UI Integration – Entry 12: Building and Launching the Gradio Interface

Artifact:

<img width="491" height="782" alt="image" src="https://github.com/user-attachments/assets/32fe4931-ea51-4ac3-90a7-952dd1ac66f9" />

<img width="478" height="809" alt="image" src="https://github.com/user-attachments/assets/1fa34d45-d196-4c00-b436-c5f95f989ecc" />


Context:
I used AI to help combine my CSV analysis functions, recommendation system, and savings calculator into a single Gradio web interface.

My Prompt:
“I'm building a Smart Finance Assistant in Google Colab using Gradio.
I already have these functions:

load_and_clean_transaction_data(file_path)
analyze_spending_patterns(df)
generate_financial_recommendations(analysis_data)
create_savings_calculator_tool(current_savings, monthly_contribution, target_amount)
Please create a beginner-friendly Gradio interface function called create_finance_assistant_ui().
Requirements:

Include a CSV upload section
Run cleaning + spending analysis when a file is uploaded
Display the spending report and recommendations
Include a simple savings calculator section
Keep the layout simple and beginner-friendly
Do not include complex chat/RAG integration yet because the hands-on-ai server may be unavailable
Use only functions I already have”

Reflection:
The AI helped generate a clean Gradio interface with separate tabs for spending analysis and savings tracking. While testing the app, I noticed that the public `gradio.live` link sometimes loaded very slowly or returned timeout errors even though the notebook showed the app was running successfully. This taught me that deployment and hosting issues are separate from coding errors. I also learned how Gradio connects front-end UI components to my Python functions through handler functions and interface layouts.

___

Foundation Function Tests – Entry 13: Testing and Validating the Finance Assistant

Artifact:

<img width="489" height="778" alt="image" src="https://github.com/user-attachments/assets/6e3cc942-795f-4e41-8d7e-e4e4dadeee27" />

<img width="493" height="807" alt="image" src="https://github.com/user-attachments/assets/6b9fcd62-3a63-47ff-b59d-30274e9b4e0e" />

<img width="488" height="329" alt="image" src="https://github.com/user-attachments/assets/fb1fabe0-6826-44e4-bd6d-b1066c825d32" />


Context:
I used AI to help create a beginner-friendly testing system for my Smart Finance Assistant.

My Prompt:
“I’m building Step 6 testing for my Smart Finance Assistant in Google Colab.
I already have these functions:

load_and_clean_transaction_data(file_path)
analyze_spending_patterns(df)
generate_financial_recommendations(analysis_data)
create_savings_calculator_tool(current_savings, monthly_contribution, target_amount)
Please create a beginner-friendly test suite using simple assert statements.
Requirements:

Create small test datasets using pandas
Test valid transaction data
Test dollar sign cleaning
Test missing category/description values
Test spending analysis totals
Test savings calculator edge cases
Keep the code simple and easy to explain
Avoid advanced testing frameworks like pytest
Use clear print statements showing which tests passed”

Reflection:
The AI helped me create structured tests that checked both normal financial data and edge cases. I successfully verified that my cleaning function handled missing values and dollar signs correctly, that spending totals were calculated accurately, and that the savings calculator safely handled invalid inputs like zero contributions and negative balances. This taught me that testing is an important part of software development because it confirms that both the technical code and the financial business logic work correctly before deployment.

___

Advanced Integration Tests – Entry 14: End-to-End Integration Testing

Artifact:

<img width="496" height="761" alt="image" src="https://github.com/user-attachments/assets/0f99f581-950f-4685-9c08-a888846005bd" />

<img width="502" height="844" alt="image" src="https://github.com/user-attachments/assets/ffceed1a-6136-4d3e-baa2-f64ef03e3682" />


Context:
I used AI to help create a simplified end-to-end integration test for my Smart Finance Assistant without relying on live AI servers or Gradio deployment.

My Prompt:
“Create a beginner-friendly integration test that simulates the complete workflow of my Smart Finance Assistant using only my existing Python functions. Test CSV loading, spending analysis, recommendation generation, and the savings calculator using assert statements and simple print outputs.”

Reflection:
The AI helped me build a full workflow test that connected my cleaning, analysis, recommendation, and savings calculator functions together. I learned that integration testing is different from unit testing because it verifies that separate parts of the system can successfully pass data between each other without crashing. I also learned that simplified integration tests are more reliable for university projects than relying on unstable external AI APIs or live servers.

___

Final Reflection – Smart Finance Assistant Project

This project helped me understand how modern AI-assisted software development works in a real business context. Throughout the development process, I used AI tools to help brainstorm ideas, generate starter code, debug errors, improve prompts, and design user-friendly financial features.

One of the most important lessons I learned was that AI-generated code should always be reviewed and tested carefully. Several times during the project, I discovered that AI suggested incorrect APIs or code structures that did not match the actual `hands_on_ai` package. By checking documentation, running `dir()` inspections, and validating outputs with tests, I learned how to critically evaluate AI suggestions instead of blindly accepting them.

Technically, I developed practical skills in:

* CSV data cleaning with pandas
* Financial spending analysis
* Error handling and validation
* Automated testing with assert statements
* Gradio interface design
* Basic RAG system concepts
* AI-assisted software development workflows

I also improved my understanding of business-focused programming by designing features around real financial problems faced by university students, such as overspending, budgeting, and savings planning.

Overall, this project showed me how AI can act as a development assistant rather than a replacement for problem-solving and critical thinking.
