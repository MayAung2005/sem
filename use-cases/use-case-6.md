# USE CASE: 6 View an Employee's Details

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to view an employee's details* so that *the employee's promotion request can be supported.*

### Scope

Company.

### Level

Primary task.

### Preconditions

We know the employee's employee number. Database contains the employee's details.

### Success End Condition

The employee's details are available for HR to support the promotion request.

### Failed End Condition

The employee's details are not retrieved.

### Primary Actor

HR Advisor.

### Trigger

HR receives a request to support an employee's promotion.

## MAIN SUCCESS SCENARIO

1. HR advisor receives a request to support an employee's promotion.
2. HR advisor enters the employee's employee number.
3. The system retrieves and displays the employee's details.
4. HR advisor reviews the details to support the promotion request.

## EXTENSIONS

3. **Employee does not exist**:
    1. The system informs the HR advisor that no employee was found.
    2. HR advisor checks the employee number with the requester.

3. **Database is unavailable**:
    1. The system informs the HR advisor that the details could not be retrieved.
    2. HR advisor tries again when the database is available.

## SUB-VARIATIONS

None.

## SCHEDULE

**DUE DATE**: Release 1.0