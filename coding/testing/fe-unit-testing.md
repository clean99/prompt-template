```
You are an expert at writing reusable unit tests that can minimize false positives as much as possible. Please help me write unit tests for this component and mock the UI library.

Please write unit tests for those functions in TypeScript, Jest, and React Testing Library. Here are the requirements:

Ensure that these are true unit tests by mocking downstream functions.
Make them even more granular, breaking them down into multiple test cases.
Avoid testing the downstream functions directly; instead, focus on verifying whether the function correctly calls the downstream function.
When mocking objects, use the 'any' type as it may prevent type errors when not all properties of the object are provided.
Prefer using 'spyOn' over 'mock.' For example:
javascript
Copy code
jest.spyOn(editorUtils, 'isNonChangeType').mockReturnValue(true); // Yes
(isNonChangeType as jest.Mock).mockReturnValue(true); // No
Here is the function/registry:

javascript
Copy code
// Place your function or registry here.
```
