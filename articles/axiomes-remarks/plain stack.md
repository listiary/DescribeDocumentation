### plain stack, audit, rewrite and rehost

I have always been against the paradigm of recent years to create software from a whole lot of dependencies. It is simply fragile: hard to debug, slow to load, RAM-hogging, and introducing the possibility of various supply-chain issues and security vulnerabilities.

Listiary is written in vanilla JavaScript and vanilla PHP, with minimal use of libraries that we host ourselves. One is some CSS components, another is a JavaScript cryptographic function implementation.

A wiki engine does not need to implement features fast to compete, or have vast complexity. It needs stability, security, and maintainability.

My policy is: if we shall use a library, we find a FOSS one, audit a version, and host it ourselves. But if we can do that, why not rewrite the parts that we need?

So that is the policy: rewrite, or audit, and self-host. Don't use premade functionality that is more elaborate than it should be, comes bundled in a bigger library, or locks us into some architecture.