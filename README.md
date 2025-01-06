# Unhandled JSON Key Access in Dart

This repository demonstrates a common error in Dart when handling JSON responses: attempting to access keys that might not exist in the JSON data.  The `bug.dart` file contains the erroneous code, and `bugSolution.dart` provides a corrected version.

The problem arises when assuming a specific key always exists in the JSON response.  If the key is missing, the application will throw a runtime exception.

The solution involves checking for the key's existence before accessing its value using the `containsKey()` method or try-catch block to handle potential exceptions.