# Rekommendation
Recommendation model for the Bangkit 2024 Capstone Project ABA-I (Ayo Baca Indonesia).

# Execute the IPYNB file
1. Download the IPYNB file.
2. Download the storyy.csv file and save it in the local directory.
3. Upload the IPYNB file to Google Colaboratory.
4. Run the file.
   
# Preparing a database
1. Download the file "story_db" from the "data" folder.
2. Open the XAMPP application and start Apache and MySQL.
3. Click on the "admin" button next to MySQL.
4. Click on "New" to create a new database.
5. In the "Database name" field, enter "story_db" and leave the other settings as they are, then click "Create".
6. Go to the newly created database "story_db".
7. Look at the top tab, then select the "Import" menu.
8. In the "Choose file" section, select the "story_db" file that you downloaded.
9. Scroll down and ensure the SQL format is selected.
10. Scroll further down and click on "Import" to import the file.

# Implementing the model
1. Download tha app.py file.
2. Download the files in the "model" folder: "rekomendasiByStoryID.h5" and "vectorizer.pkl" and save it.
3. Download the requirements.txt file and save it.
4. For app.py, edit the "model_path" and "vectorizer_path" sections according to where you have saved your .h5 and .pkl files.
5. Create a virtual environment.
6. Activate the virtual environment.
7. Install the required packages "pip install -r requirements.txt".
8. Enter "python app.py" to execute it, and make sure you are connected to the database.
9. Open the postman app.
10. In the header tab, set the key to "Content-Type" and the value to "application/json". 
11. Next, in the Body tab, select the raw format, and choose JSON format on the right side.
12. For example, enter the following JSON:
    {
    "story_id": 10,
    "top_n": 5
  }
13. Send post request in the POSTMAN APP "http://127.0.0.1:5000/recommend"

![image](https://github.com/Mus-lihah/rekommendation/assets/113479745/620b1e63-1b02-4fb4-bcc8-ab5ca6324578)

