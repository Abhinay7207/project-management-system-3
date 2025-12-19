# Event Handling & Processing
Optimize event listeners and delegation for efficient performance.

## Code Example: Button Action Listeners
Java Swing uses `ActionListener` to handle user clicks. The logic is encapsulated within the event handler to respond immediately to user input.

```java
// src/StartFrame.java

enterscreen_button.addActionListener(new java.awt.event.ActionListener() {
    public void actionPerformed(java.awt.event.ActionEvent evt) {
        enterscreen_buttonActionPerformed(evt);
    }
});

private void enterscreen_buttonActionPerformed(java.awt.event.ActionEvent evt) {
    // Event processing logic: Validate inputs and check file database
    if(ID_text.getText().equals("")) {
        jLabel2.setText("Enter a ID number and password!!!");
    }
    // ...
}
```
