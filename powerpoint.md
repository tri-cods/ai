# Creating a Presentation from Text
The OpenAI system can't create files but it can generate code that can be used to generate files.  In this example, we ask OpenAI to generate Microsoft Visual Basic (VBA) code to generate a PowerPoint file.  

If you don't have access to PowerPoint, you can try the same thing for Google Slides. See instructions below.

## PowerPoint version
1. Go to the [OpenAI Playground](https://platform.openai.com/playground?mode=chat) and make sure you are in Chat mode.  
2. Select GPT-4 as the model
3. Enter something like the prompt `Act as a VBA programmer. Write me VBA code to create PowerPoint slides using the following text for an academic audience and create at least 10 slides.` Then copy and paste in your article. 
     - There is a limit to the amount of text you can paste.  Stick with no more than a half page of text.
4. OpenAI should generate some code.  It may (or may not) give you instructions on how to run the code in PowerPoint.
5. Open PowerPoint and create a new presentation
6. Select Tools --> Macro --> Visual Basic Editor --> Insert --> Module.  This should open a new text area to enter code.
7. Paste in the code that OpenAI generated
8. Click on the Run menu --> Run Sub/Userform.  A new presentation should be generated.
     - It is possible that OpenAI made an error.  If so, go back and try re-running the prompt

## Google Slides version
1. Go to the [OpenAI Playground](https://platform.openai.com/playground?mode=chat) and make sure you are in Chat mode.  
2. Select GPT-4 as the model
3. Enter something like the prompt `Act as a Google App Script programmer. Write me code to create a Google Slide presentation using the following text for an academic audience and create at least 10 slides.` Then copy and paste in your article. 
     - There is a limit to the amount of text you can paste.  Stick with no more than a half page of text.
4. OpenAI should generate some code.  It may (or may not) give you instructions on how to run the code in Google Slides.
5. Open Google Slides
6. Select Extensions --> App Script
7. Replace the content in the main text box with the code output from OpenAI
8. Save the project and click the Run button.  
     - The first time running, you will need to allow Google permission to run your code.  You do need to trust that OpenAI won't do something nefarious to your Google files!
10. A new presentation should be generated.  Look in the "Execution Log" area for a link.  
