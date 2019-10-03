---
title: 'Example 2'
date: 2019-02-11T19:27:37+10:00
weight: 20
---

standardese looks for documentation comments as shown in the following example:

```cpp
/// A regular C++ style documentation comment.
/// Multiple C++ style comments are merged automatically.
///   This line has *two* leading whitespaces because one is always skipped.

//! A C++ style comment using an exclamation mark.
/// It will also merge with other C++ style comments.
//! But don't worry, also with the exclamation mark styles.

/** A C style documentation commment. */
/** This is a different comment, they aren't merged.
 * But you can be fancy with the star at the beginning of the line.
 * It will ignore all whitespace, the star and the first following whitespace.
 */

/*! You can also use an exclamation mark. */
/// But neither will merge with any other comment.

int x; //< An end-of-line comment.
/// It will merge with C++ style comments.
int y; //< But this is a different end-of-line comment.
```

