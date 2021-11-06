+++

title = "Go-Urbit Core Interface"
date = "2021-11-08"

[taxonomies]
grant_type = ["Proposal"]
grant_category = ["App Dev: Other"]

[extra]
image = ""
description = "Create a go-urbit library that contains the required functions for interfacing with Ames"
reward = 3
assignee = "~litryl-tadmev"
grant_id = "P0100"
completed = false
canceled = false
link = ""

+++

# go-urbit core interface

One of the missing projects in the Urbit ecosystem is the ability to directly communicate with Urbit from another device or system using the Ames protocol.

Most particularly embedded devices and low-power systems needing to transmit messages to another ship, on which running a full Urbit ship would either be not possible, or not ideal. This also includes services running in cloud environments only needing to transmit message packets.

I am proposing to create a go-urbit library that contains the required functions for interfacing with Ames.

My end goal, as discussed with ~wicdev-wisryt for a future proposal, is to rewrite the Urbit King in go using this library for maximum security and memory safety.

## Milestones

### Milestone 1 - Go Noun

Expected Completion:
Payment: 1 Star

Implement the Noun protocol in Golang.

Core Noun functions:

- mug
- jam
- cue

Implement the core Noun structures:

- Atom
- Cell

### Milestone 2 - Go Ames Utilities

Expected Completion:
Payment: 2 stars

Implement a Golang utility library for interfacing with Ames.

- Lookup a planet's keys on Ethereum by name
- Send encrypted packets using urcrypt
- Construct and send poke
- Encode and send packet
- Write documentation on setup and usage