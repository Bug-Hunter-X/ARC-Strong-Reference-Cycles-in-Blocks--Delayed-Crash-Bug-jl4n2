# Objective-C ARC Strong Reference Cycle Bug

This repository demonstrates a common and insidious bug in Objective-C related to Automatic Reference Counting (ARC) and strong references within blocks.  The bug manifests as a crash or unexpected behavior that may not appear immediately after the problematic code executes, making it especially difficult to debug.

The `bug.m` file contains the buggy code that demonstrates the issue. The `bugSolution.m` file offers a corrected version of the code.

## How to Reproduce

1. Clone this repository.
2. Open the project in Xcode.
3. Run the app.  The bug may or may not manifest immediately, as it depends on timing and other factors.

## Solution

The solution involves careful management of strong references within blocks, often using weak references to prevent retain cycles. The corrected code is shown in `bugSolution.m`.