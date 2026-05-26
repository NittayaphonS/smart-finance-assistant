Week 8 — Environment Setup & Connection Debugging

Context:
I was testing the connection to the hands-on-ai server using get_response().

Problem:
The code printed “connection successful”, but the actual response contained “Error: Connection error”. This showed that the try/except block only checked whether the function returned something, not whether the AI response was successful.

AI Interaction:
I asked AI to explain why the code showed a success message even though the response contained an error.

Decision:
I decided to rerun the test and check whether the server, model, or API key might be causing the problem. I also continued working on the data-processing foundation because the project can still progress without the AI connection.

Reflection:
I learned that successful code execution does not always mean the external service worked correctly. I should inspect the actual returned response, not only whether the Python cell ran without crashing.
<img width="262" height="955" alt="image" src="https://github.com/user-attachments/assets/a319cfb3-dda8-431b-b7e9-d1eedc996d46" />
Result:
After updating the validation logic, the notebook correctly detected that the server returned an error. Instead of printing a misleading success message, it now shows “Server returned an error”.

Reflection:
This improvement made the connection test more reliable. I learned that good debugging is not only about fixing the external problem, but also about making the program report failures more clearly.




Week 8 – Debugging hands-on-ai connection

Context:
I was testing the hands-on-ai connection for my Smart Finance Assistant project.

Problem:
The AI server still returned a connection error after two attempts.

AI Interaction:
I used AI to understand why the previous connection test was misleading and how to improve the validation logic.

Decision:
I updated the code so it checks whether the returned response contains an error message. This made the output more accurate.

Reflection:
I learned that fixing code does not always mean fixing the external service. In this case, my code became better at detecting the problem, even though the server connection issue still remained. This helped me understand the difference between a coding issue and an external system issue.
<img width="331" height="687" alt="image" src="https://github.com/user-attachments/assets/1b0e1023-840b-4c98-ad83-85abc4f3add3" />








Week 8 – AI-Generated Sample Transaction Data

Context:
I needed realistic sample transaction data to test the Smart Finance Assistant.

AI Interaction:
I asked Gemini to create sample financial transaction data using Australian businesses and student-related spending categories.

Decision:
I reviewed the AI-generated data and decided it needed minor adjustment because my teacher’s starter code used dollar-sign strings for the Amount column. This would allow me to practise data cleaning later.

Reflection:
I learned that AI-generated code or data still needs to be checked against the project requirements. Gemini produced useful sample data, but I needed to compare it with the notebook structure before using it. This helped me practise evaluating AI output instead of accepting it without review.
<img width="271" height="940" alt="image" src="https://github.com/user-attachments/assets/6b737bf1-dbfb-469a-b7aa-fe4c5610ca13" />




Week 8 – Defining the Finance Problem

Context:
I needed to define a clear business problem before building the Smart Finance Assistant.

AI Interaction:
I used AI to brainstorm different personal finance problems and compare their suitability.

Decision:
I selected a problem that focused on spending awareness and budgeting support because it aligned with the transaction dataset and project goals.

Reflection:
I learned that defining the problem clearly affects later design decisions and helps keep the project focused on user value rather than only technical features.
<img width="505" height="892" alt="image" src="https://github.com/user-attachments/assets/1904e432-cbb1-4776-a17f-4289f165372b" />




Context:
I needed to define a clear business problem for the Smart Finance Assistant.

AI Interaction:
I used AI to brainstorm different finance problems and compare how well they matched the planned features.

Decision:
I selected a problem focused on making financial planning easier through transaction analysis and conversational advice.

Reflection:
I learned that defining the problem early helps guide later technical decisions and keeps the project focused on user needs rather than adding random features.
<img width="760" height="492" alt="image" src="https://github.com/user-attachments/assets/269548ab-ebab-478d-b50d-dcabf6ede371" />


Context:
I needed to define what data the Smart Finance Assistant would use and what useful outputs it should produce.

AI Interaction:
I used Gemini to help structure the project inputs and outputs based on my problem statement.

Decision:
I included both technical inputs, such as CSV transaction columns, and business outputs, such as spending summaries and budgeting recommendations.

Reflection:
I learned that identifying inputs and outputs early makes the project easier to plan because it clarifies what data needs to be cleaned, analysed, and presented to the user.
<img width="490" height="807" alt="image" src="https://github.com/user-attachments/assets/6a7d5d84-340e-413d-bdda-1df9a5adfe39" />


Context:
I needed to manually work through financial examples before implementing code.

AI Interaction:
I used Gemini to generate realistic transaction scenarios and explain how to calculate financial insights manually.

Decision:
I selected examples that reflected common student spending situations and focused on understanding the business logic behind the calculations.

Reflection:
I learned that manually calculating results first makes it easier to design and verify the later Python implementation.
<img width="522" height="850" alt="image" src="https://github.com/user-attachments/assets/912f9e10-0cf8-4532-a3eb-c5cee0730ecd" />
<img width="458" height="677" alt="image" src="https://github.com/user-attachments/assets/819c9192-0099-485e-8b3c-58c8d54814c9" />
<img width="475" height="757" alt="image" src="https://github.com/user-attachments/assets/a4826cd1-ba8e-4194-80aa-49e965a905a1" />
<img width="496" height="863" alt="image" src="https://github.com/user-attachments/assets/b3877656-c562-4a2d-9750-cc4feebda6f9" />


