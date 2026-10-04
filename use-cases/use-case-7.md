# USE CASE: 7 Update an Employee's Details

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to update an employee's details* so that *the employee's details are kept up-to-date.*

### Scope

Company.

### Level

Primary task.

### Preconditions

We know the employee's employee number. The employee's record exists, and HR has the updated details.

### Success End Condition

The employee's updated details are saved in the database.

### Failed End Condition

The employee's existing details remain unchanged.

### Primary Actor

HR Advisor.

### Trigger

HR receives a request to change an employee's details.

## MAIN SUCCESS SCENARIO

1. HR advisor receives the updated employee details.
2. HR advisor enters the employee's employee number.
3. The system retrieves and displays the existing employee details.
4. HR advisor changes the relevant details.
5. The system validates the updated details.
6. HR advisor confirms the changes.
7. The system saves the updated details and confirms success.

## EXTENSIONS

3. **Employee does not exist**:
    1. The system informs the HR advisor that no employee was found.
    2. HR advisor checks the employee number with the requester.

5. **Updated details are missing or invalid**:
    1. The system identifies the details that need correcting.
    2. HR advisor corrects the details.
    3. The system validates the details again.

7. **Database save fails**:
    1. The system informs the HR advisor that the update failed.
    2. The employee's existing details remain unchanged.
    3. HR advisor tries again when the problem is resolved.

## SUB-VARIATIONS

6. **HR advisor cancels the update**:
    1. The system discards the proposed changes.
    2. The employee's existing details remain unchanged.

## SCHEDULE

**DUE DATE**: Release 1.0