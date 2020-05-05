# System Boundary

In analyzing the requirments for a new system, it can be useful to
establish a system boundary.  This determines what is inside the system,
and what is outside.  Things that are outside the system and interact with
it are called "actors."  Use cases can the be developed to describe the 
interaction of one (or sometimes more) actors interacting with the system.
Each use case is a concrete, specific example of an interaction with the
system.  For example, "Jenny submits video of her children homeschooling" 
would be an appropriate level for a use case.

By defining actors, and by documenting representative use cases, one can
capture the scope and the purpose of the system to be built.

An initial system diagram is presented here:

![System Boundary](boundary.svg)


## System:  CaMPa<sub>19</sub> node

The system analyzed here is a single CaMPa<sub>19</sub> node.  In this
view, other nodes can be viewed as an actor, to model exchanges between
nodes.  A single node consists of a storage system for bulk assets, a
much smaller catalog (or metadata database), and a system for running
queries by researchers.  If sufficient distribution of bulk assets,
e.g. to the public, is forseen, a Content Delivery Network may be necessary
as well.

## Actors

An initial set of known actors is pictured.  For each actor, a set of
detailed, concrete use cases can be developed.  The initial actors are:

###  Other CaMPa<sub>19</sub> node

This represents interactions with other nodes, if this functionality
is required.  A use case here might be processing of a query from a
researcher in Germany across several different EU nodes.

### Curator

It seems likely that a curator would be needed, to screen and categorize
incoming submissions, and to help better organize it.  Another possible
use case for the curator is rejecting a contribution on copyright or
decency grounds.

### Contributor

In this view, a contributor is thought of as a member of the public, 
contributing some asset.  Contributions might also come from other sources,
such as other institutions.

###  Public (Browsing Collection)

This actor is meant to capture "casual," non-research oriented interactions 
with the system by members of the public.

### Researcher

This actor captures an individual or institution performing research
on the data stored in the node.  Many question of system scope will be
answered by elaborating use cases centered around this actor.  For
example, is data mining that involves inspection of the asset payload
to be supported?  

###  Other Institution

This captures institutional actors that use the system, like a regional
library.  A regional library might make pre-curated assets available
to CaMPa<sub>19</sub> in bulk, for example, and it might serve as a
portal to the museum's assets.

