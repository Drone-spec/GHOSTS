# GHOSTS NPC Framework

GHOSTS simulates what anyone might do at a computer, creating documents, browsing websites, and downloading files. GHOSTS drives all sorts of popular applications on many versions of Windows and Linux machines. Whether you're a friendly administrator or a powerful cyber adversary, GHOSTS can replicate your expected behavior.

GHOSTS has many use cases in cyber training and exercises, most notably for bringing non-player characters (NPCs) to life, but GHOSTS can be used for many other purposes where realistic activity on a computer is needed as well.

There is a [short demonstration video available on YouTube](https://www.youtube.com/watch?v=EkwK-cqwjjA) (3:03).

---

**Version 8 is here (with breaking changes!).** It has absorbed the other modules of the GHOSTS framework, [ANIMATOR (now archived)](https://github.com/cmu-sei/GHOSTS-ANIMATOR) and [SPECTRE (now archived)](https://github.com/cmu-sei/GHOSTS-SPECTRE). This was done in order to greatly simplify installation, configuration, and the administration of a GHOSTS instance, but also to bring further capability to the core agents by more tightly combining information segregated into separate databases and systems until now.

The breaking changes are:

1. Configuration file changes
2. Database changes
3. API endpoint changes

Sorry, but there is no upgrade path from previous versions — install a fresh instance to get rolling with V8.

---

## Key Links

- [Quick Start: Installation from distribution binaries](https://cmu-sei.github.io/GHOSTS/quickstart/)
- [GHOSTS Documentation](https://cmu-sei.github.io/GHOSTS/)
- [Don't hesitate to submit issues and feature requests](https://github.com/cmu-sei/GHOSTS/issues)

## Platform Components

### Ghosts Clients (Windows & Linux)

GHOSTS clients simulate users on a machine doing "user-like" things. They can be configured to:

- Browse the web
- Create and edit office documents
- Send and respond to email
- Run terminal commands
- Etc.

### Ghosts API Server

The API server provides a way for clients to interact with the GHOSTS system and its clients. It can:

- Manage clients, add/remove them from groups, etc.
- Get/manage information from clients regarding their previous or current activities, etc.
- Orchestrate new activities for particular clients to perform

### [Ghosts UI](src/ghosts.ui/README.md)

The web server provides a way for administrators to interact with the GHOSTS system and its clients.

### [Ghosts Lite](src/Ghosts.Client.Lite/)

A resource light version of the Windows GHOSTS client that can be run on minimal hardware.

### [Pandora Content Server](src/ghosts.pandora/)

A server that provides content to GHOSTS clients (or otherwise). Pandora determines what you most likely requested, creates that content, and serves it back in the response. Pandora also has the ability to serve predetermined static content for training and exercise purposes (and red-teaming).

### [Pandora Socializer Server](src/ghosts.pandora.socializer/)

The social media (x.com) server that enables Ghosts clients to post and interact with social media content.

## License

[DISTRIBUTION STATEMENT A] This material has been approved for public release and unlimited distribution.
Copyright 2017 Carnegie Mellon University. All Rights Reserved. See LICENSE.md file for terms.
