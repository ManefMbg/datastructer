ALGORITHM elements

1- Declare Variables:
VAR
    set1, set2 : ARRAY_OF INTEGER;
    i, j, sum: INTEGER;
    found: BOOLEAN;
    
BEGIN

2- Read Input Lists:

    write("Give me the first list");
    read(set1);
    write("Give me the second list");
    read(set2);
    
3- Initialize Sum:
    sum=0;

4- Iterate Through set1:

    FOR i FROM 0 TO set1.length-1 DO
    found:=FALSE;
    FOR j FROM set2.length-1 TO max  DO
        IF (set1[i] = set2[j]) THEN
            found:= TRUE;
            BREAK;

        END_IF
    END_FOR 
        IF (found = FALSE) THEN
            sum:=sum+set1[i]
        END_IF
    END_FOR
    
5- Iterate Through set2:

    FOR i FROM 0 TO set2.length-1 DO
        found:=FALSE;
        FOR j FROM set1.length-1 TO max DO
            IF (set2[i] - set1[j]) THEN
                found:= TRUE;
                BREAK;
            END_IF
        END_FOR
        IF (found:=FALSE) THEN
            sum:=sum+set2[i]

        END_IF
    END_FOR

6- Print Result:  

    write("The sum of set1 and set 2: ")
END
