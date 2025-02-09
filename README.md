# Unhandled Exception in Asynchronous Dart Code

This repository demonstrates a common error in asynchronous Dart code: failing to properly handle exceptions during network requests.  The `bug.dart` file contains code that makes an HTTP request but doesn't adequately handle potential errors. The `bugSolution.dart` file shows how to fix the issue by using `try-catch` blocks and proper exception handling.

## Problem

The original code lacks robust error handling. If the HTTP request fails or the JSON response is malformed, the application might crash or behave unpredictably.  Good error handling improves the reliability and maintainability of the application.

## Solution

The solution involves using a `try-catch` block to wrap the asynchronous operation.  The `catch` block handles exceptions and allows for graceful error handling, preventing crashes and providing informative error messages.