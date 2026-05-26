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

