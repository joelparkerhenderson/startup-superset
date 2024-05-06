# Twelve-Factor App methodology

https://en.wikipedia.org/wiki/Twelve-Factor_App_methodology

The Twelve-Factor App methodology is a methodology for building software-as-a-service applications. These best practices are designed to enable applications to be built with portability and resilience when deployed to the web.[1]

Codebase: There should be exactly one codebase for a deployed service with the codebase being used for many deployments.

Dependencies: All dependencies should be declared, with no implicit reliance on system tools or libraries.

Config: Configuration that varies between deployments should be stored in the environment.

Backing services: All backing services are treated as attached resources and attached and detached by the execution environment.

Build, release, run: The delivery pipeline should strictly consist of build, release, run.

Processes: Applications should be deployed as one or more stateless processes with persisted data stored on a backing service.

Port binding: Self-contained services should make themselves available to other services by specified ports.

Concurrency: Concurrency is advocated by scaling individual processes.

Disposability: Fast startup and shutdown are advocated for a more robust and resilient system.

Dev/Prod parity: All environments should be as similar as possible.

Logs: Applications should produce logs as event streams and leave the execution environment to aggregate.

Admin Processes: Any needed admin tasks should be kept in source control and packaged with the application. 

