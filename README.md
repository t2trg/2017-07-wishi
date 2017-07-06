# Workshop on IoT Semantic/Hypermedia Interoperability

When: July 15/16, 2017 (weekend before IETF99)

Where: Hilton Prague (IETF meeting hotel), room Berlin/Brussels. Pobřežní 1, Prague, Czech Republic

Meeting sponsor: [Ericsson](https://www.ericsson.com/en/internet-of-things).

Registration: https://goo.gl/forms/yUTebqK9C84Ef01i2

Please register by **June 23rd**. Registration and meeting is free of cost (thanks Ericsson) but we need to know number of participants for meeting logistics.

Draft agenda is available [here](https://github.com/t2trg/2017-07-wishi/blob/master/AGENDA.md).

# Workshop plan

One of the interesting questions in the IoT space is the role of
hypermedia and/or semantic interoperability for reducing setup
overhead and thus TCO, and, more generally, enabling interoperation in
the first place.

For example, OMA and IPSO smart objects use the LWM2M object model,
which defines a set of pre-structured URI templates and registry of
object identifiers with semantics attached. This provides
machine-readable representations of the semantics, but self
description is not being used much.

OCF has a hypermedia approach with discovery using /oic/res etc.,
which relies on self-description via pointing to predefined resource
types and interface types, which in turn use a number of specification
techniques, including JSON schema and RAML.

There is also iot.schema.org, which will allow us to gather further
semantic interoperability information in potentially a more granular
way.

W3C WoT cares a lot about self-description, with an RDF-based take on
semantics and describing things.

T2TRG cares about pulling all this together.

On July 15, we will have a workshop that includes people from these
organizations/groups.  The focus will be on building a landscape that
can benefit from the various approaches, without necessarily papering
over all the holes or filling in all the rifts.  On July 16, we will
have additional time for follow-on work groups that want to make
progress on specific issues.

The venue is the Prague Hilton, the same hotel that will host IETF99
directly after that.  To further minimize travel, we chose the weekend
directly after the July W3C WoT meeting in close by Düsseldorf.

Elements of the agenda:

## State of the union

We will have "state of the union" talks from each of the
organizations, discussing from a personal perspective where we are on
interoperability in the organization and what are the next steps.

## Research contributions, prototypes

We issued a [call for contributions][cfc], with a goal of getting new
views and new voices into the mix.  This solicits research on the
approaches available for building hybrid, overarching systems, as well
as some practical systems that are already demonstrating how this
could be made to work in practice, such as systems for converting some
of the formal notations and/or self descriptions into each other.

[cfc]: https://github.com/t2trg/2017-07-wishi/blob/master/CALL-FOR-CONTRIBUTIONS.md

## Specific topics

The below topics (and any other that come up) could be discussed on
Saturday and/or result in more detailed breakouts on Sunday.

### Interops

The "device ecosystem" oriented SDOs are now increasingly using common
protocols and formats (CBOR, CoAP, IPv6) which is creating one narrow
waist in the system, and we can look into creating a narrow waist also
around semantic interoperability and hypermedia design patterns.
Ultimately, it should not matter which device ecosystem(s) you use for
your application.  The device ecosystems can maintain their focus on
intra-op and certification while an over arching web-like layer of
interoperability can add more value to all of them.

Now is a good time to start to organize cross-ecosystem interops,
where we attempt to orchestrate devices and sources from these
different device ecosystems. At this point we need to consider
orchestration across applications as well as device to device
interoperability.

We have also discussed a lot about conducting more of the actual
testing over the Internet. This seems like a good concept to build in
from the beginning. What are the tools we need to conduct an online
hyper-semantic interop series? Is it staged, from basic to more
sophisticated?

This seems to represent the canonical use case for both W3C WoT and
iot.schema.org, as well as the various translators and bridges being
created.

### Hypermedia forms

HTML has a form element that can be used to construct POST request
bodies (and other request payloads, such as for PATCH).  An M2M
equivalent has been lacking for quite some time, although there are
proposals.  Now that we have FETCH and PATCH (RFC 8132), the need is
even more pronounced.  What are the next steps towards common
Hypermedia "forms", which would help at least T2TRG, OCF, and WoT?

### Hypermedia-driven applications in general

T2TRG has a number of drafts documenting how application developers
use hypermedia to aid in building thing-to-thing (and thing-to-cloud)
systems.  Are these complete?  What else do we know about that? What
about documents from, say, W3C or IPSO?

### Model translation

We now have multiple proposals for data modeling (YANG, CDDL, JSON
Schema, JSON Content Rules) as well as ad-hoc metamodels.  What are
the semantic powers of these modeling approaches?  Can we
automatically translate between them so we can make models of one
ecosystem available for the other ones?  How do we tap hidden Gems
such as the ZigBee Cluster Library or the Bluetooth GATT specs? What
about interaction modeling (also YANG, RAML, Swagger, ...)?
