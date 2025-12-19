# Integration of Components
Ensure smooth interaction between different modules for a seamless user experience.

## Code Example: Frame Navigation
Transitioning from `StartFrame` (Login) to `Employee_InfoFrame` demonstrates component integration. Data is passed between frames using public fields.

```java
// src/StartFrame.java

if(infos[0].equalsIgnoreCase(ID_text.getText()) && infos[7].equalsIgnoreCase(password_text.getText())){
    dispose(); // Close current login window
    
    // Open the next component
    Employee_InfoFrame f2 = new Employee_InfoFrame();
    f2.setVisible(true);
    f2.str = line; // Pass authenticated user data to the next component
}
```

## Code Example: Class Interaction
The `Create_Project` class integrates with `ProjectMember` to verify manager details before assignment.

```java
// src/Create_Project.java

ProjectMember member = new ProjectMember();
// ...
String message = member.SearchMember(txtEmpID.getText()); // Integration point
```
