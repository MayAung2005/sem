# USE CASE: 8 Delete an Employee's Details

## CHARACTERISTIC INFORMATION

### Goal in Context

As an *HR advisor* I want *to delete an employee's details* so that *the company is compliant with data retention legislation.*

### Scope

Company.

### Level

Primary task.

### Preconditions

We know the employee's employee number. The employee's record exists. HR has confirmed that the record is eligible for deletion under the company's data retention policy.

### Success End Condition

The employee's details eligible for deletion are removed from the database.

### Failed End Condition

The employee's details remain unchanged.

### Primary Actor

HR Advisor.

### Trigger

HR identifies an employee record that is due for deletion under the company's data retention policy.

## MAIN SUCCESS SCENARIO

1. HR advisor enters the employee's employee number.
2. The system retrieves and displays the employee's details.
3. HR advisor checks that the correct employee record has been selected.
4. HR advisor selects the option to delete the employee's details.
5. The system requests confirmation.
6. HR advisor confirms the deletion.
7. The system deletes the employee's details and confirms success.

## EXTENSIONS

2. **Employee does not exist**:
    1. The system informs the HR advisor that no employee was found.
    2. HR advisor checks the employee number.

7. **Database deletion fails**:
    1. The system informs the HR advisor that deletion failed.
    2. The employee's details remain unchanged.
    3. HR advisor tries again when the problem is resolved.

## SUB-VARIATIONS

6. **HR advisor cancels the deletion**:
    1. The system cancels the operation.
    2. The employee's details remain unchanged.

## SCHEDULE

**DUE DATE**: Release 1.0