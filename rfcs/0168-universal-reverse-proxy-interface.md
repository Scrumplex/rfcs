---
feature: universal-reverse-proxy-interface
start-date: 2023-12-29
author: Sefa Eyeoglu
co-authors: (find a buddy later to help out with the RFC)
shepherd-team: (names, to be nominated and accepted by RFC steering committee)
shepherd-leader: (name to be appointed by RFC steering committee)
related-issues: (will contain links to implementation PRs)
---

# Summary
[summary]: #summary

Implement a set of NixOS options to offer a universal interface to configure reverse proxies.
These options can be used by applications to expose themselves independent of the administrator's preferred reverse proxy.

# Motivation
[motivation]: #motivation

Currently a lot of NixOS modules provide opinionated virtual host configurations for Nginx.
Users who choose to use reverse proxies other than Nginx can not make use of these options.
They usually have to resort to configuring their reverse proxies directly,
which results in a lot of repetitve configurations.
This RFC proposes a universal interface, which modules can make use of to share configurations across reverse proxies.

# Detailed design
[design]: #detailed-design

<!--
This is the core, normative part of the RFC.
Explain the design in enough detail for somebody familiar with the ecosystem to understand, and implement.
This should get into specifics and corner-cases.
Yet, this section should also be terse, avoiding redundancy even at the cost of clarity.
-->

# Examples and Interactions
[examples-and-interactions]: #examples-and-interactions

<!--
This section illustrates the detailed design.
This section should clarify all confusion the reader has from the previous sections.
It is especially important to counterbalance the desired terseness of the detailed design;
if you feel your detailed design is rudely short, consider making this section longer instead.
-->

# Drawbacks
[drawbacks]: #drawbacks

<!--
What are the disadvantages of doing this?
-->

# Alternatives
[alternatives]: #alternatives

<!--
What other designs have been considered? What is the impact of not doing this?
For each design decision made, discuss possible alternatives and compare them to the chosen solution.
The reader should be convinced that this is indeed the best possible solution for the problem at hand.
-->

# Prior art
[prior-art]: #prior-art

[RFC 0163](https://github.com/NixOS/rfcs/pull/163) proposes a portable interface for services in general.

Using Caddy with it's adapter interface [mdleom blogpost](https://mdleom.com/blog/2020/03/14/caddy-nixos-part-3/#caddyProxy-nix)

Kubernetes has a universal interface for managing external access to services called [Ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/)


<!--
You are unlikely to be the first one to tackle this problem.
Try to dig up earlier discussions around the topic or prior attempts at improving things.
Summarize, discuss what was good or bad, and compare to the current proposal.
If applicable, have a look at what other projects and communities are doing.
You may also discuss related work here, although some of that might be better located in other sections.
-->

# Unresolved questions
[unresolved]: #unresolved-questions

<!--
What parts of the design are still TBD or unknowns?
-->

# Future work
[future]: #future-work

<!--
What future work, if any, would be implied or impacted by this feature without being directly part of the work?
-->
