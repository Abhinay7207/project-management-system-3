# Error Handling & Robustness
Implement proper error handling to manage invalid inputs and system failures without crashes.

## Code Example: Safe Integer Parsing
Handling `NumberFormatException` prevents the application from crashing when non-numeric text is entered in ID fields.

```java
// src/StartFrame.java

try {
    int id = Integer.valueOf(ID_text.getText());
    // ... logic to check ID range ...
} catch (NumberFormatException e) {
    jLabel2.setText("ID must be a number!");
}
```

## Code Example: File Operations
Wrapping file I/O in `try-catch` blocks ensures that missing files or read errors are handled gracefully.

```java
// src/StartFrame.java

try {
    bReader = new BufferedReader(new FileReader(file));
    // ... read file ...
} catch (FileNotFoundException ex) {
    Logger.getLogger(StartFrame.class.getName()).log(Level.SEVERE, null, ex);
} finally {
    if (bReader != null) {
        try {
            bReader.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```
