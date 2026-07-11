# opentrackclient

This library allows POSIX software on macOS or Linux to read opentrack's headpose by loading a shared library and using a simple API. - similar to how it's done under Windows.

See otrclient-tester.c as an example. Opentrack's X-Plane plugin uses the opentrack client library as well (linked statically).

It still uses shared memory so it probably won't work if you create a sanboxed macOS. Having that abstraction now allows to use a different inter-process-communication mechanism in future.
