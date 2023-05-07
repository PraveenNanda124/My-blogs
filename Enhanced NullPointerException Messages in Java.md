# Enhanced NullPointerException Messages in Java

![j](https://user-images.githubusercontent.com/116082827/236680762-e0361c74-4e50-46a2-8869-6c89eb6371cc.png)


Java 14 introduced an enhancement to NullPointerException messages that provides more detailed information about the source of the null reference. This feature can help developers to quickly identify and fix null pointer errors.



Example:



String str = null;

int length = str.length(); // Throws NullPointerException with enhanced message

