# Relational-Data-Model
Implementation of a database system and relational algebra.

Part 1
This part contains all the fundamental functions of database, such as insert, delete, and lookup. Also, the struct and initialization functions are included in this section. As for data structure, we use HashTable to store all relational tables. For delete and lookup, some attributes can be leave unspecified as "*" (char type) or -1 (int type). In additional, we have some helper functions that print and compare tuples.
The function demo_part1() is used to run the demonstration of part 1.

Part 2
This part supports queries across more than one table. One function answers the question "What grade did NAME get in COURSE?" by querying SNAP and CSG tables. And another function answers "Where is NAME at HOUR on DAY?" by querying SNAP, CSG, CDH, and CR tables.
The function demo_part2() is used to run the demonstration of part 2.

Part 3
This part implements the relational algebra operations of tuples, including selection, projection, and join. These functions were made specifically for the requirements of this project. 
The function demo_part3() is used to run the demonstration of part 3.

Appendix: 5 relations used in the project

StudentId Name Address Phone
66252 L. Adams 55 Pear Ave. 455-9284
01376 R. Johnson 88 Apple Dr. 717-5542
39391 O. Gonzalez 62 Durian Blvd. 687-6203
74533 C. Johnson 5 Raisin Ln. 992-4616
58429 O. Gonzalez 78 Rhubarb Ave. 171-8839
99730 R. Johnson 56 Kiwi Blvd. 903-9855

Course StudentId Grade
CSC171 66252 A
CSC171 58429 B
MATH150 39391 A
DSCC201 66252 C
DSCC201 01376 B+
CSC172 99730 AMATH150 58429 C+
CSC173 74533 B+
CSC173 99730 A
DSCC201 99730 C

Course Prerequisite
CSC172 CSC171
CSC172 MATH150
CSC173 CSC172
CSC252 CSC172
CSC254 CSC252
DSCC201 CSC171
DSCC202 DSCC201
DSCC265 CSC262
DSCC265 CSC171

Course Day Hour
CSC171 M 1400
CSC171 W 1400
CSC172 M 1525
CSC172 W 1640
CSC173 M 1400
CSC173 W 1400
CSC252 M 1230
CSC252 W 1230
DSCC201 T 900
DSCC201 R 900
DSCC202 T 1650
DSCC202 R 1650
DSCC265 T 1400
DSCC265 R 1400

Course Room
CSC171 Hutchison Hall 141
CSC172 Hutchison Hall 141
CSC173 Wegmans 1400
CSC252 Wegmans 1400
CSC254 Wegmans 1400
DSCC201 Bausch & Lomb 109
DSCC202 Dewey 2162
DSCC265 Wegmans 1400
MATH150 Harkness 115
