# Versity 
**University Portal**

A java-based web app, which provides a attractive UI to manage the the database of university.

Some of the features -
* Extract details of a student by their Roll Number.
* Search details of Courses provided by various departments
* List the Grades of students
* Add new student into the database
* Generate an instuctor's workload report
---

**Home Screen**

<img src='/images/homeScreen.PNG' title='home screen'/>


**Course Search**

<img src='/images/courseSearch.PNG' title='course search'/>

[Get more screen shots of the project here.](https://github.com/akash99-code/Versity/tree/master/images)


---

**Snapshot of the university database**

| Tables_in_university |
|----------------------|
| advisor              |
| classroom            |
| course               |
| department           |
| instructor           |
| prereq               |
| section              |
| student              |
| takes                |
| teaches              |
| time_slot            |

*advisor*
| s_ID  | i_ID  |
|-------|-------|
| 12345 | 10101 |
| 44553 | 22222 |
| 45678 | 22222 |
| 00128 | 45565 |
| 76543 | 45565 |
| 23121 | 76543 |
| 98988 | 76766 |
| 76653 | 98345 |
| 98765 | 98345 |

*classroom*
| building | room_number | capacity |
|----------|-------------|----------|
| Packard  | 101         |      500 |
| Painter  | 514         |       10 |
| Taylor   | 3128        |       70 |
| Watson   | 100         |       30 |
| Watson   | 120         |       50 |

*course*
| course_id | title                      | dept_name  | credits |
|-----------|----------------------------|------------|---------|
| BIO-101   | Intro. to Biology          | Biology    |       4 |
| BIO-301   | Genetics                   | Biology    |       4 |
| BIO-399   | Computational Biology      | Biology    |       3 |
| CS-101    | Intro. to Computer Science | Comp. Sci. |       4 |
| CS-190    | Game Design                | Comp. Sci. |       4 |
| CS-315    | Robotics                   | Comp. Sci. |       3 |
| CS-319    | Image Processing           | Comp. Sci. |       3 |
| CS-347    | Database System Concepts   | Comp. Sci. |       3 |
| EE-181    | Intro. to Digital Systems  | Elec. Eng. |       3 |
| FIN-201   | Investment Banking         | Finance    |       3 |
| HIS-351   | World History              | History    |       3 |
| MU-199    | Music Video Production     | Music      |       3 |
| PHY-101   | Physical Principles        | Physics    |       4 |

*department*
| dept_name  | building | budget    |
|------------|----------|-----------|
| Biology    | Watson   |  90000.00 |
| Comp. Sci. | Taylor   | 100000.00 |
| Elec. Eng. | Taylor   |  85000.00 |
| Finance    | Painter  | 120000.00 |
| History    | Painter  |  50000.00 |
| Music      | Packard  |  80000.00 |
| Physics    | Watson   |  70000.00 |

*instructor*
| ID    | name       | dept_name  | salary   |
|-------|------------|------------|----------|
| 10101 | Srinivasan | Comp. Sci. | 65000.00 |
| 12121 | Wu         | Finance    | 90000.00 |
| 15151 | Mozart     | Music      | 40000.00 |
| 22222 | Einstein   | Physics    | 95000.00 |
| 25638 | akash      | Biology    | 45000.00 |
| 32343 | El Said    | History    | 60000.00 |
| 33456 | Gold       | Physics    | 87000.00 |
| 45565 | Katz       | Comp. Sci. | 75000.00 |
| 58583 | Califieri  | History    | 62000.00 |
| 76543 | Singh      | Finance    | 80000.00 |
| 76766 | Crick      | Biology    | 72000.00 |
| 83821 | Brandt     | Comp. Sci. | 92000.00 |
| 98345 | Kim        | Elec. Eng. | 80000.00 |

*prereq*
| course_id | prereq_id |
|-----------|-----------|
| BIO-301   | BIO-101   |
| BIO-399   | BIO-101   |
| CS-190    | CS-101    |
| CS-315    | CS-101    |
| CS-319    | CS-101    |
| CS-347    | CS-101    |
| EE-181    | PHY-101   |

*section*
| course_id | sec_id | semester | year | building | room_number | time_slot_id |
|-----------|--------|----------|------|----------|-------------|--------------|
| BIO-101   | 1      | Summer   | 2009 | Painter  | 514         | B            |
| BIO-301   | 1      | Summer   | 2010 | Painter  | 514         | A            |
| CS-101    | 1      | Fall     | 2009 | Packard  | 101         | H            |
| CS-101    | 1      | Spring   | 2010 | Packard  | 101         | F            |
| CS-190    | 1      | Spring   | 2009 | Taylor   | 3128        | E            |
| CS-190    | 2      | Spring   | 2009 | Taylor   | 3128        | A            |
| CS-315    | 1      | Spring   | 2010 | Watson   | 120         | D            |
| CS-319    | 1      | Spring   | 2010 | Watson   | 100         | B            |
| CS-319    | 2      | Spring   | 2010 | Taylor   | 3128        | C            |
| CS-347    | 1      | Fall     | 2009 | Taylor   | 3128        | A            |
| EE-181    | 1      | Spring   | 2009 | Taylor   | 3128        | C            |
| FIN-201   | 1      | Spring   | 2010 | Packard  | 101         | B            |
| HIS-351   | 1      | Spring   | 2010 | Painter  | 514         | C            |
| MU-199    | 1      | Spring   | 2010 | Packard  | 101         | D            |
| PHY-101   | 1      | Fall     | 2009 | Watson   | 100         | A            |

*student*
| ID    | name          | dept_name  | tot_cred |
|-------|---------------|------------|----------|
| 00128 | Zhang         | Comp. Sci. |      102 |
| 12345 | Shankar       | Comp. Sci. |       32 |
| 18456 | akash         | Biology    |      603 |
| 19991 | Brandt        | History    |       80 |
| 23121 | Chavez        | Finance    |      110 |
| 44553 | Peltier       | Physics    |       56 |
| 45678 | Levy          | Physics    |       46 |
| 54321 | Williams      | Comp. Sci. |       54 |
| 55739 | Sanchez       | Music      |       38 |
| 58649 | Akash         | Finance    |       80 |
| 58845 | Akash bairagi | Finance    |       80 |
| 64546 | akaa          | Biology    |      230 |
| 66111 | akash         | Biology    |      230 |
| 66532 | akash         | Music      |      586 |
| 70557 | Snow          | Physics    |        0 |
| 76543 | Brown         | Comp. Sci. |       58 |
| 76653 | Aoi           | Elec. Eng. |       60 |
| 8535  | addfef        | Biology    |      502 |
| 98765 | Bourikas      | Elec. Eng. |       98 |
| 98988 | Tanaka        | Biology    |      120 |

*takes*
| ID    | course_id | sec_id | semester | year | grade |
|-------|-----------|--------|----------|------|-------|
| 00128 | CS-101    | 1      | Fall     | 2009 | A     |
| 00128 | CS-347    | 1      | Fall     | 2009 | A-    |
| 12345 | CS-101    | 1      | Fall     | 2009 | C     |
| 12345 | CS-190    | 2      | Spring   | 2009 | A     |
| 12345 | CS-315    | 1      | Spring   | 2010 | A     |
| 12345 | CS-347    | 1      | Fall     | 2009 | A     |
| 19991 | HIS-351   | 1      | Spring   | 2010 | B     |
| 23121 | FIN-201   | 1      | Spring   | 2010 | C|    |
| 44553 | PHY-101   | 1      | Fall     | 2009 | B-    |
| 45678 | CS-101    | 1      | Fall     | 2009 | F     |
| 45678 | CS-101    | 1      | Spring   | 2010 | B|    |
| 45678 | CS-319    | 1      | Spring   | 2010 | B     |
| 54321 | CS-101    | 1      | Fall     | 2009 | A-    |
| 54321 | CS-190    | 2      | Spring   | 2009 | B|    |
| 55739 | MU-199    | 1      | Spring   | 2010 | A-    |
| 76543 | CS-101    | 1      | Fall     | 2009 | A     |
| 76543 | CS-319    | 2      | Spring   | 2010 | A     |
| 76653 | EE-181    | 1      | Spring   | 2009 | C     |
| 98765 | CS-101    | 1      | Fall     | 2009 | C-    |
| 98765 | CS-315    | 1      | Spring   | 2010 | B     |
| 98988 | BIO-101   | 1      | Summer   | 2009 | A     |
| 98988 | BIO-301   | 1      | Summer   | 2010 | NULL  |

*teaches*
| ID    | course_id | sec_id | semester | year |
|-------|-----------|--------|----------|------|
| 76766 | BIO-101   | 1      | Summer   | 2009 |
| 76766 | BIO-301   | 1      | Summer   | 2010 |
| 10101 | CS-101    | 1      | Fall     | 2009 |
| 45565 | CS-101    | 1      | Spring   | 2010 |
| 83821 | CS-190    | 1      | Spring   | 2009 |
| 83821 | CS-190    | 2      | Spring   | 2009 |
| 10101 | CS-315    | 1      | Spring   | 2010 |
| 45565 | CS-319    | 1      | Spring   | 2010 |
| 83821 | CS-319    | 2      | Spring   | 2010 |
| 10101 | CS-347    | 1      | Fall     | 2009 |
| 98345 | EE-181    | 1      | Spring   | 2009 |
| 12121 | FIN-201   | 1      | Spring   | 2010 |
| 32343 | HIS-351   | 1      | Spring   | 2010 |
| 15151 | MU-199    | 1      | Spring   | 2010 |
| 22222 | PHY-101   | 1      | Fall     | 2009 |

*time_slot*
| time_slot_id | day | start_hr | start_min | end_hr | end_min |
|--------------|-----|----------|-----------|--------|---------|
| A            | F   |        8 |         0 |      8 |      50 |
| A            | M   |        8 |         0 |      8 |      50 |
| A            | W   |        8 |         0 |      8 |      50 |
| B            | F   |        9 |         0 |      9 |      50 |
| B            | M   |        9 |         0 |      9 |      50 |
| B            | W   |        9 |         0 |      9 |      50 |
| C            | F   |       11 |         0 |     11 |      50 |
| C            | M   |       11 |         0 |     11 |      50 |
| C            | W   |       11 |         0 |     11 |      50 |
| D            | F   |       13 |         0 |     13 |      50 |
| D            | M   |       13 |         0 |     13 |      50 |
| D            | W   |       13 |         0 |     13 |      50 |
| E            | R   |       10 |        30 |     11 |      45 |
| E            | T   |       10 |        30 |     11 |      45 |
| F            | R   |       14 |        30 |     15 |      45 |
| F            | T   |       14 |        30 |     15 |      45 |
| G            | F   |       16 |         0 |     16 |      50 |
| G            | M   |       16 |         0 |     16 |      50 |
| G            | W   |       16 |         0 |     16 |      50 |
| H            | W   |       10 |         0 |     12 |      30 |

---
**Technical Specifications**
* building Platform - Eclipse (kepler)
* Server - Tomcat v7.0
* database - MySql (at localhost)
* other concepts implemented- MVC, AJAX, JSP, jdbc driver, java beans
