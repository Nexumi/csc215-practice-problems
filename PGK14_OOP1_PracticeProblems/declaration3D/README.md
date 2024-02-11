# [Array Declaration 3D](../)

> By: Jimmy Pan

<hr>

- Problem 1: Create a method that takes a 3D array of characters and print them out as followed.
    - Output must match the sample output (headers for each row, a tab (\t), then the symbols)
    - Hint:
        - Row is the first [2]
        - Each row in the row is the [3]
            - Hence 3 rows
        - The number of symbols per row of each row is the last [2]
- Problem 2: What type and what method did I use to create the `symbols3D` array?
    - Ragged/Jagged Array with Shorthand Notation
    - Ragged/Jagged Array with Multi-Step Approach
    - Standard Array with Shorthand Notation
    - Standard Array with Multi-Step Approach

```java
char[][][] symbols3D = new char[2][3][2];
symbols3D[0][0][0] = '!';
symbols3D[0][0][1] = '@';
symbols3D[0][1][0] = '#';
symbols3D[0][1][1] = '$';
symbols3D[0][2][0] = '%';
symbols3D[0][2][1] = '^';
symbols3D[1][0][0] = '&';
symbols3D[1][0][1] = '*';
symbols3D[1][1][0] = '(';
symbols3D[1][1][1] = ')';
symbols3D[1][2][0] = '-';
symbols3D[1][2][1] = '=';
```
```
Row 1:
    ! @
    # $
    % ^
Row 2:
    & *
    ( )
    - =
```