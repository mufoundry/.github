# MuFoundry: A Modern MU* SDK

## What is this?
MuFoundry is a modern software development kit (SDK) for creating MU* (MUD, MUX, MUSH, MOO, etc) servers.

## Who is it for?
MU* developers who want to quickly get past the boilerplate of MU* networking and focus on game logic and content. It requires moderate to advanced Python knowledge, depending on design complexity, but every effort is made to be as beginner-friendly as possible. It's worth mentioning that networking and multiplayer games are among the most complicated programming endeavors out there.

## Major Features
- **HTTP API**: The **Game** process includes a Hypercorn server running a FastAPI app. This provides a RESTful interface with automated OpenAPI/Swagger documentation. HTTP/2 and HTTP/3 are enabled, with HTTP/3 desired for its ability to transparently reconnect roaming clients.
- **Ultimate Moddability**: The SDK is designed to be as moddable as possible. A rich config system powered by `Dynaconf` defines python paths to load classes from and plugins to load. 99% of a MuFoundy project's capabilities are handled by plugins.

## Project Structure
MuFoundry is broken down into three main repositories:
- [muforge](https://github.com/mufoundry/muforge): MuForge is the engine that runs the game server and provides the FastAPI web features.
- [muplugins](https://github.com/mufoundry/muplugins): MuPlugins are the official plugins for MuFoundry, which implement a great deal of boilerplate game logic and provide highly useful features such as chat channels and rule-based access control. Most MuFoundry flagship features such as Telnet support are implemented as plugins.
- [mucrucible](https://github.com/mufoundry/mucrucible): MuCrucible is a project skeleton that provides a starting point for creating and managing a MuFoundry project.

## More info coming soon...
