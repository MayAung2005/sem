# USE CASE: 3 Produce a Report on the Salary of Employees in My Department

## CHARACTERISTIC INFORMATION

### Goal in Context

As a *department manager* I want *to produce a report on the salary of employees in my department* so that *I can support financial reporting for my department.*

### Scope

Company.

### Level

Primary task.

### Preconditions

The department manager's department is known. Database contains current employee salary data and department assignments.

### Success End Condition

A report containing the current salaries of employees in the manager's department is available.

### Failed End Condition

No report is produced.

### Primary Actor

Department Manager.

### Trigger

The department manager needs salary information for departmental financial reporting.

## MAIN SUCCESS SCENARIO

1. Department manager requests a salary report for their department.
2. The system identifies the manager's department.
3. The system retrieves current salary information for employees currently assigned to that department.
4. The system produces the salary report.
5. Department manager uses the report for departmental financial reporting.

## EXTENSIONS

2. **The manager's department cannot be identified**:
    1. The system informs the department manager.
    2. Department manager asks HR to check their department assignment.

3. **No employees are assigned to the department**:
    1. The system informs the department manager that no employees were found.

3. **Database is unavailable**:
    1. The system informs the department manager that salary information could not be retrieved.
    2. Department manager tries again when the database is available.

## SUB-VARIATIONS

None.

## SCHEDULE

**DUE DATE**: Release 1.0