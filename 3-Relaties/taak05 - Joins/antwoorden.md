# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
    SELECT * FROM game JOIN platform ON game.platform_id = platform_id
2. Copy paste je gemaakte SQL query hieronder
     SELECT * FROM game JOIN platform ON game.platform_id = platform_id WHERE game.id <= 10;
3. Copy paste je gemaakte SQL query hieronder
    SELECT name, platform FROM game JOIN platform ON game.platform_id = platform_id WHERE name = "Call of Duty: Advanced Warfare";
4. Copy paste je gemaakte SQL query hieronder
    SELECT platform, name FROM game JOIN platform ON game.platform_id = platform_id WHERE name LIKE 'FIFA%';
5. Copy paste je gemaakte SQL query hieronder
    SELECT * FROM game JOIN platform ON game.platform_id = platform_id WHERE name = 'Borderlands' AND name = 'Borderlands 2';