# Native Pigeon Tests

This directory contains native test harnesses for native and end-to-end tests
of Pigeon-generated code. The [test script](../tool/run_tests.dart) generates
native code from [pigeons/](../pigeons/) into the native test scaffolding, and
then drives the tests there.

To run these tests, use [`run_tests.dart`](../tool/run_tests.dart)

## test\_plugin

The new unified test harness for all platforms. Tests in this plugin use the
same structure as tests for the Flutter team-maintained plugins, as described
[in the repository documentation](https://github.com/flutter/flutter/wiki/Plugin-Tests).

## alternate\_language\_test\_plugin

The test harness for alternate languages, on platforms that have multiple
supported plugin languages. It covers:
- Java for Android
- Objective-C for iOS

## flutter\_null\_safe\_unit\_tests

Dart unit tests for null-safe mode. This is a legacy structure from before
NNBD was the only mode Pigeon supported; these should be folded back into
the main tests.
