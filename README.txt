This solution is developed by Tanishq 2021-2025 batch. 
HOW TO RUN:
Step 1: Open the folder “newspaper_bott_deployed” on Laptop Desktop  
Step 2: Open Command Prompt and go to the address
C:\Users\Administrator\Desktop\ newspaper_bott_deployed\ newspaper_bott_deployed>
Run the command 
code .
Step 3: The main file “bot” into the folder will open in Visual Studio Code with all the prerequisite
Step 4: Run the file (Scheduler started) will appear in the window.
Step 5: Open Telegram in mobile and search “Newspaper bot”. Open it. 
Step 6: Type /start (it will start click on /setlanguage and select Hindi). Now provide any Hindi newspaper to it. It will extract all the news and will generate separate audio for them.

TECHNIQUE:
Step 1: A dataset is created by applying boxes on news using modified YOLOv8 architecture on Google Colab. Previously Utkarsh made boxes on columns.
Step 2: YOLOv8 is trained on this dataset. 
Step 3: CV2 is then used to extract these boxes in a given newspaper image. These boxes are also labeled with article, advertisement, etc. So only articles are extracted and neglect advertisement.
Step 4: Then this box is supplied to the Tesseract OCR to convert it into text.
Step 5: gTTS finally converts it into audio.


Dataset is separate, YOLOv8 code is separate. Remaining all features are in this “bot” file.
Currently this is not deployed. So we have to run the program “bot file” on computer and then use Telegram. Once deployed, there is no need to run the file in a computer, simply open the Telegram and use it. However, we have to pay $4 US Dollar per month.
 


