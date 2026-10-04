# USE CASE: 1 Produce a Report on the Salary of All Employees

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to produce a report on the salary of all employees* so that *I can support financial reporting of the organisation.*

### Scope

Company.

### Level

Primary task.

### Preconditions

Database contains current employee salary data.

### Success End Condition

A report containing the current salaries of all employees is available for HR to provide to finance.

### Failed End Condition

No report is produced.

### Primary Actor

HR Advisor.

### Trigger

A request for salary information for all employees is sent to HR by finance.

## MAIN SUCCESS SCENARIO

1. Finance requests salary information for all employees.
2. HR advisor selects the option to produce a salary report for all employees.
3. The system retrieves current salary information for all employees.
4. The system produces the salary report.
5. HR advisor provides the report to finance.

## EXTENSIONS

3. **No employee salary data is found**:
    1. The system informs the HR advisor that no salary data is available.
    2. HR advisor informs finance that the report cannot be produced.

3. **Database is unavailable**:
    1. The system informs the HR advisor that salary information could not be retrieved.
    2. HR advisor tries again when the database is available.

## SUB-VARIATIONS

None.

## SCHEDULE

**DUE DATE**: Release 1.0