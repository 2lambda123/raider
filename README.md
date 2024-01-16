![Raider logo](https://raiderauth.com/images/logo/logo.png)

# Quick links

- [Website](https://raiderauth.com/).
- [OWASP page](https://owasp.org/www-project-raider/).
- [Documentation](https://docs.raiderauth.com/en/latest/).
- [Installation](https://docs.raiderauth.com/en/latest/overview/install.html).
- [FAQ](https://docs.raiderauth.com/en/latest/overview/faq.html).
- [Getting started](https://docs.raiderauth.com/en/latest/tutorials/getting_started.html).
- [Running the Project Locally](#running-the-project-locally)
- [Executing Tests](#executing-tests)
- [Troubleshooting Common Issues](#troubleshooting)
- [Additional Resources](#additional-resources)
- [Architecture](https://docs.raiderauth.com/en/latest/case_studies/architecture.html).
- [Discussions](https://github.com/OWASP/raider/discussions).
- [Issues](https://github.com/OWASP/raider/issues).
- [Twitter](@raiderauth).
- [Fediverse](@raiderauth@infosec.exchange).

# What is Raider

OWASP Raider was developed with the goal to improve web authentication
testing. By now it has evolved and can be used for all kinds of
stateful HTTP processes.  It abstracts the client-server information
exchange as a finite state machine. Each step comprises one request
with inputs, one response with outputs, arbitrary actions to do on the
response, and conditional links to other stages. Thus, a graph-like
structure is created. Raider allows you to simulate complex systems
while allowing you to control each piece of data you get in and out of
the system.

# Graph-like architecture

Raider defines a DSL to describe the information flow between the
client and the server for HTTP processes. Each step of the process is
described by a Flow, which contains the Request with inputs, Response
with outputs, and arbitrary actions including links to other Flows:

![Flows](https://raiderauth.com/images/illustrations/raider_flows.png)

Chaining several Flows together can be used to simulate any stateful
HTTP process. FlowGraphs indicate the starting point. They can be
placed on any Flow. A FlowGraphs runs all Flows in the link until
Success/Failure is returned or if there are no more links.

![Flows and FlowGraphs](https://raiderauth.com/images/illustrations/graph.png)

# Configuration

Raider's configuration is inspired by Emacs. Hylang is used, which is
LISP on top of Python. LISP is used because of its "Code is Data, Data
is Code" property. With the magic of LISP macros generating
configuration automatically becomes easy. Flexibility is in its DNA,
meaning it can be infinitely extended with actual code. 
You can use it for example to create, store, reproduce, and share
proof-of-concepts easily for HTTP attacks. With Raider you can also
search through your Projects, filter by hyfile, Flows, FlowGraphs,
etc... Then you run either just one step, or a chain of steps, so you
can automate and run tests on any HTTP process.


![Example hylang configuration](https://raiderauth.com/images/illustrations/config.png)


# Command line interface

You can use it for example to create, store, reproduce, and share.

## Running the Project Locally
To run the project locally, follow these steps:
1. Step 1
2. Step 2
3. Step 3

## Executing Tests
To execute tests, use the following steps:
1. Step 1
2. Step 2
3. Step 3

## Troubleshooting GitHub Actions
If you encounter issues with GitHub Actions, follow these troubleshooting steps:
1. Check the workflow logs to identify the cause of the failure.
2. Identify any error messages or warnings in the logs.
3. Take appropriate actions based on the identified issues.

## Additional Resources
For additional resources and support, visit:
- [Community Forum](https://forum.raiderauth.com)
- [Knowledge Base](https://docs.raiderauth.com/kb)
- [Contact Support](https://raiderauth.com/support)
proof-of-concepts easily for HTTP attacks. With Raider you can also
search through your Projects, filter by hyfile, Flows, FlowGraphs,
etc... Then you run either just one step, or a chain of steps, so you
can automate and run tests on any HTTP process.

You can also search through your Projects, filter by hyfile, Flows,
FlowGraphs, etc… Then you run either just one step, or a chain of
steps, so you can automate and run tests the HTTP process.
