# Overall Overview

![overview](../diagrams/conceptOverview.drawio.svg "overview")

The Principal Attestation Service attempts to augment arbitrary authentication
services by attesting certain attributes, or facts, about a principal. In a
traditional authentication flow, a principal provides the authentication
service with a secret, usually in the form of a username/password combination
or a token. The problem with this traditional authentication flow is that
the authentication service only validates the principals knowledge of a single
secret. A secret that easily can move between principals.

Multi Factor Authentication goes a long way to help alleviate this issue. By
forcing the principal to authenticate via "something they are" and "something
the know", an authentication service can know, with some degree of certainty,
that a principal is who they claim to be.

The problem with Multi Factor Authentication, as it is implemented today, is
that it rarely is used in machine-to-machine communication and that it is
seldom used apply different policies/levels of access based on the operational
context of the principal.

The Principal Attestation Service is built to fit into this Multi Factor
Authentication flow, by providing a vendor-agnostic way to query for, and
attest, certain facts about the state of the principal.
