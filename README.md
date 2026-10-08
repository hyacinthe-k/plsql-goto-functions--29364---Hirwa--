# plsql-goto-functions--29364---Hirwa--
# PL/SQL GOTO Statements and Functions - Individual Assignment III

A1 01_goto/A1_number_classifier.sql  
<img width="1437" height="1771" alt="a1" src="https://github.com/user-attachments/assets/3f84a333-d290-44b8-8e40-657324aa21f4" />

A2 01_goto/A2_salary_review.sql 
<img width="1442" height="1612" alt="a2" src="https://github.com/user-attachments/assets/84163132-c91a-4674-8c12-4685b434df55" />

A3 01_goto/A3_illegal_goto.sql 
<img width="1469" height="1614" alt="a3" src="https://github.com/user-attachments/assets/545515b5-bc29-454e-93cc-a8080d54706c" />

A4 01_goto/A4_rewrite_no_goto.sql
<img width="1641" height="1653" alt="a4" src="https://github.com/user-attachments/assets/aabeb191-701a-4e6a-a78d-6f4140772493" />

B5  03_tests/B5_functions_in_select.sql 
<img width="1535" height="1646" alt="b5" src="https://github.com/user-attachments/assets/3a5d0d8f-6325-4909-9cc9-fbd5a192072a" />

C1 02_functions/C1_fn_validate_payroll.sql 
<img width="1431" height="1633" alt="c1" src="https://github.com/user-attachments/assets/f392b3f7-38b6-421b-addf-34f2a8189ad2" />

C2 docs/REFLECTION.md 
In this assignment I learned that a GOTO statement jumps to a label in the same or an enclosing block, but it can never jump into an IF, a loop or an exception handler. Doing so causes the PLS-00375 error I reproduced in A3. Rewriting A1 and A2 without GOTO (A4) showed me that IF/ELSIF, CASE and CONTINUE give the same result with code that is shorter and much easier to read, so GOTO should be used rarely. In Part B, I learned that functions must return a value, can be called directly inside SELECT, WHERE and ORDER BY statements, and need exception handling for bad input such as NULL values, negative salaries and missing departments. Combining the small functions into the payroll validator in C1 showed me how reusable, well-tested functions make larger programs simpler. The hardest part was getting label scope right and deciding how to handle invalid data, and next time I would store the tax brackets in a table instead of hard-coding them.

## How to Run (Oracle SQL Developer)
1. Run `00_setup/create_tables.sql` (F5 = Run Script).
2. Run the functions in `02_functions/` in order B1, B2, B3, B4, C1.
3. Run the programs in `01_goto/` (A1 and A4 prompt for a number).
4. Run the tests in `03_tests/`.
5. Take screenshots into `screenshots/`.


