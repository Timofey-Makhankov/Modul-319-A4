# Modul-319-A4

School Grading CLI

## Student Object

```mermaid
    classDiagram
    class Student{
        int ID
        String Name
        float[] Grades
        NaN()
    }
```

## Activity Diagram

```mermaid
    flowchart LR
    A((Start))-->B(Ask for Student)
    G-->B
    B-->|create Student|G(Add New Student)
    B-->C
    C--->|change Student|B
    C{User\nInput}
    C-->|Add Grade|D(Append Grade)
    C-->|Change Grade|E(Update/Change Grade)
    C-->|calculate Garde|F(Print Out the Average Grade)
    D--->C 
    E--->C 
    F--->C
    C-->|Userinput: X|X(Exit)
```
