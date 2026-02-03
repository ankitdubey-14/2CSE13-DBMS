CREATEING TABLE 
```sql
CREATE TABLE Movie(Movie_ID INT PRIMARY KEY,
    -> MovieName VARCHAR(50) NOT NULL UNIQUE,
    -> Category VARCHAR(50) NOT NULL,
    -> ReleaseDate DATE ,
    -> ProuductionCost DECIMAL(8,2) CHECK(ProductionCost>0),
    -> BusinessCost DECIMAL(8,2) DEFAULT 0 );
```
SERT
```sql
INSERT INTO Movie
    VALUES
    -> (001,"Hindi_Movie","Musical","2018-04-03",124500.00,130000.00),
    -> (002,"Tamil_Movie","Action","2016-05-17", 112000.00,118000.00),
    -> (003,"English_Movie","Horror","2017-08-06",245000.00,360000.00),
    -> (004,"Bengali_Movie","Adventure","2017-01-04",72000.00,100000),
    -> (005,"Telugu_Movie","Action",100000,0),
    -> (006,"Punjabi_Movie","Comedy",30500.00,0);
