# Data Validation
Implement client-side and server-side validation to prevent invalid data entry.

## Code Example: Date Validation
Custom helper method to strictly validate date formats (DD/MM/YYYY) before processing.

```java
// src/Create_Project.java

private boolean isValidDate(String dateStr) {
    java.text.SimpleDateFormat sdf = new java.text.SimpleDateFormat("dd/MM/yyyy");
    sdf.setLenient(false); // Disallow loose interpreting of dates
    try {
        sdf.parse(dateStr);
        return true;
    } catch (java.text.ParseException e) {
        return false;
    }
}
```

## Code Example: Business Logic Validation
Validating that numerical values like age and salary fall within acceptable business rules.

```java
// src/AddEmployee.java

int age = Integer.valueOf(txtAge.getText());
float salary = Float.valueOf(txtsalary_f2.getText());

if (age < 18 || age > 100) {
     lblInf.setText("Age must be between 18 and 100");
     return;
}
if (salary <= 0) {
     lblInf.setText("Salary must be positive");
     return;
}
```
