STANDARD 3
==========

### Merge Commit Message ###



Single Revision
---------------

`Ported source_branch rXXXX to destination_branch`

Example: `Ported tb-1 r1234 to dev`



Multiple Revisions (Range)
--------------------------

`Ported source_branch r(XXXX:YYYYY) to destination_branch`

Example: `Ported tb-1 r(1234:4321) to dev`



Multiple Revisions (Cherrypick)
-------------------------------

`Ported source_branch r(XXXX, YYYYY, ZZZZ) to destination_branch`

Example: `Ported tb-1 r(123, 234:236, 345) to dev`