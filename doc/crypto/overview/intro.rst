.. SPDX-FileCopyrightText: Copyright 2018-2022, 2024 Arm Limited and/or its affiliates <open-source-office@arm.com>
.. SPDX-License-Identifier: CC-BY-SA-4.0 AND LicenseRef-Patent-license

Introduction
============

About Platform Security Architecture
------------------------------------

This document is one of a set of resources provided by Arm that can help organizations develop products that meet the security requirements of PSA Certified on Arm-based platforms. The PSA Certified scheme provides a framework and methodology that helps silicon manufacturers, system software providers and OEMs to develop more secure products. Arm resources that support PSA Certified range from threat models, standard architectures that simplify development and increase portability, and open-source partnerships that provide ready-to-use software. You can read more about PSA Certified here at :url:`www.psacertified.org` and find more Arm resources here at :url:`developer.arm.com/platform-security-resources`.

About the |API|
---------------

The interface described in this document is a PSA Certified API, that provides a portable programming interface to cryptographic operations, and key storage functionality, on a wide range of hardware.

The interface is user-friendly, while still providing access to the low-level primitives used in modern cryptography. It does not require that the user has access to the key material. Instead, it uses opaque key identifiers.

You can find additional resources relating to the |API| here at :url:`arm-software.github.io/psa-api/crypto`, and find other PSA Certified APIs here at :url:`arm-software.github.io/psa-api`.

This document includes:

*   A rationale for the design. See :secref:`design-goals`.
*   A high-level overview of the functionality provided by the interface. See :secref:`functionality-overview`.
*   A description of typical architectures of implementations for this specification. See :secref:`architectures`.
*   General considerations for implementers of this specification, and for applications that use the interface defined in this specification. See :secref:`implementation-considerations` and :secref:`usage-considerations`.
*   A detailed definition of the API. See :secref:`library-management`, :secref:`key-management`, and :secref:`crypto-operations`.

In future, companion documents will define *profiles* for this specification. A profile is
a minimum mandatory subset of the interface that a compliant implementation must
provide.
