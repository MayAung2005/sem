# USE CASE: 5 Add a New Employee's Details

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to add a new employee's details* so that *I can ensure the new employee is paid.*

### Scope

Company.

### Level

Primary task.

### Preconditions

HR has the required details for the new employee. Database is available.

### Success End Condition

The new employee's details, including the information required for payment, are stored in the database.

### Failed End Condition

No new employee record is created.

### Primary Actor

HR Advisor.

### Trigger

HR receives notification that a new employee is joining the company.

## MAIN SUCCESS SCENARIO

1. HR advisor receives the new employee's details.
2. HR advisor selects the option to add a new employee.
3. HR advisor enters the required employee details.
4. The system validates the details and checks for an existing employee record.
5. The system saves the new employee's details.
6. The system confirms that the employee was added successfully.

## EXTENSIONS

4. **Required details are missing or invalid**:
    1. The system identifies the details that need correcting.
    2. HR advisor corrects the details.
    3. The system validates the details again.

4. **Employee record already exists**:
    1. The system informs the HR advisor that the employee already exists.
    2. HR advisor checks the existing record before proceeding.

5. **Database save fails**:
    1. The system informs the HR advisor that the employee was not added.
    2. No incomplete employee record is retained.
    3. HR advisor tries again when the problem is resolved.

## SUB-VARIATIONS

None.

## SCHEDULE

**DUE DATE**: Release 1.0