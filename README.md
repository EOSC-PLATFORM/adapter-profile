# EOSC Adapter

This repository provides material defining EOSC Adapters and their publication.

- The file `adapters.schema.json` defines Adapters metadata model --
  _i.e._, how an Adapter is described within EOSC services.
- High level information on Adapters -- what is it, how to create and
  share it through EOSC Providers portal -- is provided below.

---

**_A short guide for EOSC providers_**

This guide explains how EOSC service providers, developers, and researchers can **publish an Adapter in the EOSC Integration Suite**. Adapters are a new EOSC resource designed to simplify the integration of services with the EOSC ecosystem.

The process is intentionally lightweight: develop the adapter, document it, describe it with metadata, and publish it through the EOSC onboarding workflow.

# 1. What is an Adapter?

An **Adapter** is a software component (typically a library, wrapper, or connector) that helps a service interact with EOSC services or implement EOSC interoperability guidelines.

Adapters typically:

- Wrap EOSC APIs
- Simplify integration with EOSC services
- Translate between standards or metadata formats
- Provide client libraries for common programming languages
- Implement functionality aligned with EOSC Interoperability Framework (IF) Guidelines

Examples include:

- Python or Java wrappers for EOSC service APIs
- Metadata translators (e.g., between EOSC profiles and DCAT)
- Libraries for publishing monitoring or accounting metrics

Adapters are **optional components**: EOSC services must remain usable without them.

---

# 2. Adapter Requirements

Before publishing an Adapter, ensure it satisfies the following requirements.

## 2.1 Open Source

Adapters must be **open-source software**.

Recommended licenses include:

- Apache License 2.0
- MIT
- BSD
- Other widely accepted permissive licenses

The license must be clearly declared in the repository.

---

## 2.2 Public Code Repository

The Adapter source code must be available in a **public repository**, for example:

- GitHub
- GitLab
- Bitbucket
- Institutional repositories

The repository should contain:

- Source code
- README documentation
- License file
- Usage instructions
- Release information

---

## 2.3 Documentation

Each Adapter must provide **clear documentation**, including:

- Description of the Adapter
- Target EOSC service(s)
- Associated EOSC Interoperability Guideline
- Installation instructions
- Example usage
- API documentation (if applicable)

Documentation is typically provided in the repository README or a documentation website.

---

## 2.4 Link to an EOSC Interoperability Guideline

Every Adapter must be **associated with an EOSC Interoperability Framework (IF) Guideline**.

The guideline defines:

- the interface
- the protocol
- the interoperability rule implemented by the Adapter

Adapters act as **practical implementations of these guidelines**.

---

# 3. Develop the Adapter

The first step is to develop the software.

Typical development steps include:

1. Identify the EOSC service or guideline to support.
2. Implement the Adapter functionality.
3. Package the Adapter (library, SDK, client, connector, etc.).
4. Publish the code in a public repository.
5. Create documentation and examples.

Common Adapter implementations include:

- Python libraries
- Java SDKs
- REST API clients
- Metadata converters
- CLI tools

---

# 4. Create the Adapter Metadata Profile

Adapters are published in EOSC using a **metadata profile**.

The metadata describes the Adapter as an EOSC resource and allows it to be discovered in EOSC systems.

Typical metadata fields include:

- Adapter name
- Description
- Maintainers
- Contact email
- Organisation
- Repository URL
- Documentation URL
- Programming language
- License
- Associated Interoperability Guideline
- Related EOSC services
- Version
- Last update date

This metadata enables EOSC services such as the **IF Registry**, **Service Catalogue**, and **Marketplace** to reference the Adapter.

---

# 5. Onboard the Adapter in EOSC

Adapters are onboarded through the **EOSC Provider Dashboard**.

The process typically consists of:

1. Access the EOSC Provider Dashboard.
2. Create a new **Adapter resource entry**.
3. Fill in the Adapter metadata profile.
4. Link the Adapter to:
   - an EOSC Interoperability Guideline
   - optionally one or more EOSC services.
5. Submit the record.

Once validated, the Adapter becomes part of the **EOSC Integration Suite**.

---

# 6. Publish and Discover the Adapter

After onboarding:

- The **IF Registry** stores the Adapter definition.
- The **Service Catalogue** manages Adapter records.
- The **EOSC Marketplace / Discovery Hub** makes the Adapter discoverable.

Users can then:

- search for adapters
- view documentation
- download or install the software
- integrate it with their services.

---

# 7. Maintain the Adapter

Adapter maintainers are responsible for keeping the Adapter up to date.

Recommended practices include:

- Maintain versioned releases
- Document changes (changelog)
- Fix security or compatibility issues
- Update documentation
- Maintain compatibility with updated EOSC guidelines or services

Adapters can be updated by modifying their metadata entry and publishing new software releases.

---

# 8. Community Contributions

Adapters are designed to **grow through community contributions**.

Adapters may be developed by:

- EOSC service providers
- research infrastructures
- research communities
- third-party developers

Adapters can be maintained independently from the services they integrate.

This open model allows the EOSC ecosystem to expand its interoperability capabilities over time.

---

# Summary

Publishing an Adapter involves four main steps:

1. **Develop** an open-source adapter implementing an EOSC guideline.
2. **Publish** the code in a public repository with documentation.
3. **Create metadata** describing the Adapter.
4. **Onboard it through the EOSC Provider Dashboard**.

Once published, the Adapter becomes part of the **EOSC Integration Suite**, helping providers and users integrate services more easily within the EOSC ecosystem.
