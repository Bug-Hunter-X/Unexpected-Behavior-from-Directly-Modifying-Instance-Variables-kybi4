# Unexpected Behavior from Directly Modifying Instance Variables in Ruby

This repository demonstrates a common, yet subtle, bug in Ruby stemming from directly manipulating instance variables using methods like `instance_variable_set` and `instance_variable_get`. While these methods can be useful in specific situations, they often lead to unexpected behavior and decreased code maintainability.

**Problem:** Directly modifying instance variables bypasses the encapsulation provided by methods, making it difficult to track changes and potentially breaking assumptions about the object's state. This can cause inconsistencies and make debugging a nightmare.

**Solution:** Favor using methods to access and modify the object's state. Methods provide a structured and controlled way to interact with an object's internal data.  This ensures consistency, facilitates easier debugging and testing, and adheres to good object-oriented principles.