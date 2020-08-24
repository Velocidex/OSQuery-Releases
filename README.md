# Repository to hold OSQuery releases.

OSQuery is a SQL powered operating system instrumentation, monitoring, and analytics framework.
Available for Linux, macOS, Windows, and FreeBSD. You can read more about it at https://github.com/osquery/osquery

## What is this repository?

Velociraptor can automatically use OSQuery queries directly in its artifacts. To do this, the artifact may 
define a `tool` pointing to the OSQuery download. When Velociraptor runs this artifact, it ensures the correct 
version of the tool is downloaded to the endpoint.

Using this mechanism one can simply call osquery to run an OSQuery query transparently within a standard
VQL query or artifact.

OSQuery is currently distributed as an MSI, RPM or DEB package requiring it to be completely installed on the system.
In order to ensure that osquery is not fully installed on the system, but is usable just a pure standalone query
engine we re-distribute the binary only as a release in this repository.

We do not modify the binary in any way. On windows you can verify the binary is signed by `Nickolas Anderson`.
This is merely a distribution repository.
