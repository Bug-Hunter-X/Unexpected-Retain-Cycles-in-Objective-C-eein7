# Objective-C Memory Management Bug: Unexpected Retain Cycles

This repository demonstrates a common yet subtle bug in Objective-C related to memory management and property declarations.  The bug involves an unexpected retain cycle that can lead to memory leaks.  The `bug.m` file contains the buggy code, while `bugSolution.m` provides the corrected version.

## Bug Description

The bug arises from improper handling of strong references in combination with the use of a custom setter. The retain cycle occurs because the object retains itself which can lead to memory leak. The solution involves carefully managing ownership and avoid such retain cycles.