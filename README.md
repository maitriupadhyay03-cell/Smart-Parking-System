# Smart Parking System

My second-semester Java project: a desktop app that manages a parking lot, with a Java Swing GUI and a local SQLite database.

## What it does
- Park and unpark three vehicle types: cars, motorcycles and trucks
- A parking receipt on entry; an unparking receipt with the time parked and the fee
- A dashboard that shows every slot as a card: occupied or free, and free slots per vehicle type
- Two payment modes: cash and online
- An owner view with session summaries: earnings are saved in the database, so they are still there after the app is closed and reopened

## Design
- Object-oriented model: an abstract `Vehicle` with `Car`, `Motorcycle` and `Truck`
- Singleton: `ParkingLot` (the slots) and `DatabaseManager` (all SQLite reads and writes)
- Factory: `VehicleFactory` creates the right vehicle from its type
- Strategy: `ParkingFeeStrategy` / `HourlyRateStrategy` for the fee calculation
- Custom exceptions: `ParkingFullException`, `VehicleNotFoundException`
- A UML class diagram is in `FinalProject/Readme and UML/`

## Tech
Java, Swing, SQLite through JDBC (the database is a local `smartparking.db` file, created on first run; no database server needed).

## How to run
1. Open the `FinalProject` folder in Eclipse (or any Java IDE).
2. Add the SQLite JDBC driver (`sqlite-jdbc` .jar) to the build path.
3. Run `Main.java`.

## Notes
A course project, so some parts are still basic. Ideas for later: search, and export of receipts to PDF.
