# Smart Parking System

This is my second semester Java project. It's a parking management system with a proper GUI, connected to a MySQL database. Took a while to build but I'm pretty happy with how it turned out.

## What it does

The system lets you park and unpark three types of vehicles — cars, motorcycles, and trucks. When you park a vehicle, it generates a parking receipt. When you unpark, you get an unparking receipt showing how long the vehicle was parked and how much it costs.

There's a dashboard that visually shows all the parking slots as cards — you can see at a glance which slots are occupied and which ones are free, and how many total slots are available for each vehicle type.

For payment, the system supports two methods: cash and online.

The owner side of the app also shows a session summary — so even if you close the app and reopen it, it loads the previous earnings from the database and shows how much money was made from past parking and unparking sessions.

## Tech used

- Java (Swing for GUI)
- - MySQL (for storing parking data, earnings, session history)
  - - Card-based layout for the dashboard
   
    - ## How to run
   
    - 1. Make sure you have Java and MySQL installed
      2. 2. Set up the database using the provided SQL file (if included)
         3. 3. Update the DB connection settings in the source if needed
            4. 4. Compile and run the main file
              
               5. ## Notes
              
               6. - Second semester project, still learning Java GUI so some parts of the code are a bit rough
                  - - The database stores everything so data persists between sessions
                    - - Might add more features later like a search function or export to PDF
