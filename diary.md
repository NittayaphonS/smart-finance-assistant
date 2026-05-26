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
