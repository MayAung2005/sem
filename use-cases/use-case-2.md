# USE CASE: 2 Produce a Report on the Salary of Employees in a Department

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to produce a report on the salary of employees in a department* so that *I can support financial reporting of the organisation.*

### Scope

Company.

### Level

Primary task.

### Preconditions

We know the department. Database contains current employee salary data and department assignments.

### Success End Condition

A report containing the current salaries of employees in the selected department is available for HR to provide to finance.

### Failed End Condition

No report is produced.

### Primary Actor

HR Advisor.

### Trigger

A request for salary information for a department is sent to HR by finance.

## MAIN SUCCESS SCENARIO

1. Finance requests salary information for a department.
2. HR advisor enters or selects the department.
3. The system retrieves current salary information for employees currently assigned to that department.
4. The system produces the salary report.
5. HR advisor provides the report to finance.

## EXTENSIONS

3. **Department does not exist**:
    1. The system informs the HR advisor that the department does not exist.
    2. HR advisor checks the department details with finance.

3. **No employees are assigned to the department**:
    1. The system informs the HR advisor that no employees were found.
    2. HR advisor informs finance that no employee salary information is available for that department.

3. **Database is unavailable**:
    1. The system informs the HR advisor that salary information could not be retrieved.
    2. HR advisor tries again when the database is available.

## SUB-VARIATIONS

None.

## SCHEDULE

**DUE DATE**: Release 1.0