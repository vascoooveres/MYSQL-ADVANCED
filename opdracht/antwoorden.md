# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder

    SELECT races.name AS race ,circuits.name AS circuit 
    FROM circuits 
    JOIN races ON circuits.circuitId=races.circuitId 
    WHERE year = 2018;

2. Copy paste je gemaakte SQL query hieronder

    SELECT races.name AS name, drivers.surname AS surname, driver_standing.points AS points
    FROM driver_standing
    JOIN races ON driver_standing.raceId = races.raceId
    JOIN drivers ON driver_standing.driverId = drivers.driverId
    WHERE races.year= 2017 AND points= 10;

3. Copy paste je gemaakte SQL query hieronder

    SELECT drivers.forename, drivers.surname, pitstops.duration 
    FROM drivers
    LEFT JOIN pitstops ON drivers.driverId= pitstops.driverId
    WHERE duration < 25;

4. Copy paste je gemaakte SQL query hieronder
    
    SELECT constructors.name AS constructor, races.name AS GrandPrix
    FROM constructors
    JOIN races ON constructors.constructorId = races.raceId
    WHERE constructors.name = 'McLaren'

5. Copy paste je gemaakte SQL query hieronder
    
    SELECT circuits.name AS circuit, circuits.country AS country, races.name AS GrandPrix, drivers.surname AS surname
    FROM races
    LEFT JOIN circuits ON races.circuitId = circuits.circuitId
    LEFT JOIN drivers ON  drivers.driverId = drivers.driverId
    WHERE year = '1950' AND drivers.surname LIKE 'F%'