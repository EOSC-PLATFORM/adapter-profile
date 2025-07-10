.. _adapter:

Adapter
=======
A software component specifically addressing the task of facilitating developers in implementing software to let their services interoperate with other EOSC Services, 
for example, to join the Federating Capabilities of a Node (e.g. EOSC EU Node Core Service Providers to facilitate the integration with Core Federating Capabilities). 
Examples are software libraries that map across different communication protocols, such as data formats onto other formats, API methods onto other API methods, etc. 
Adapters are typically, but not necessarily, provided by the Service providers to facilitate interoperability with them.

In addition to the properties defined by the EOSC Resource Profile (TODO ADD LINK), the EOSC Service profile defines the following properties:

.. list-table:: 
   :header-rows: 1
   :widths: 10, 15, 15, 15, 15, 15, 15

   * - Group
     - Element name
     - Description
     - Type
     - Multiplicity
     - Required
     - Suggestions
   * - Management
     - IF guideline
     - EOSC Guideline ID
     - string
     - 1
     - M
     - chosen from a list of guidelines in the Registry
   * - 
     - documentation
     - Documentation webpage (eg, read-the-docs page)
     - URL
     - 1
     - M
     - 
   * - 
     - softwareRepository
     - Code repository webpage (eg, Github repository)
     - URL
     - 1
     - M
     - That should be a link to a specific version of that repository. According to "version", e.g. release that has been checked before approval
   * - 
     - package
     - Link to latest package release page (eg, PyPI project, Docker image, Github releases page)
     - URL
     - 0..n
     - M
     - This will probably turn to be (a list of) objects. Since packages (ie, adapter's library) is dependent on a platform and maybe other attributes (eg, Python version).
   * - 
     - programmingLanguage
     - Programming language
     - string
     - 1
     - M
     - 
   * - 
     - license
     - Software/Code license (eg, MIT, APache, GPL)
     - string
     - 1
     - M
     - FOSS license, in principle
   * - 
     - version
     - Software version
     - string
     - 1
     - M
     - 
   * - 
     - changeLog
     - Changes in the latest version
     - string
     - 1
     - M
     - 
   * - 
     - lastUpdate
     - Latest update date
     - date
     - 1
     - M
     - 
   * - Creators
     - creators
     - The main researchers involved in producing the data, or the authors of the publication, in priority order. To supply multiple creators, repeat this property.
     - object
     - 1...n
     - M
     - 
   * - 
     - creatorName
     - The full name of the creator
     - string
     - 1
     - M
     - Surname, Name
   * - 
     - creatorRole
     - The role of the creator
     - Credit vocabulary
     - 1
     - O
     - 
   * - 
     - creatorPIDSchema
     - PID schema
     - 
     - 
     - O
     - e.g. ORCID, ROR.org
   * - 
     - creatorPID
     - Uniquely identifies an individual or legal entity, according to various schemes.
     - string
     - 1
     - O
     - 
   * - 
     - affiliations
     - The organizational or institutional affiliation of the creator.
     - object
     - 0..n
     - O
     - 
   * - 
     - affiliationName
     - Name of the organisation
     - string
     - 1
     - M
     - 
   * - 
     - affiliationIdentifier
     - Uniquely identifies the organizational affiliation of the creator.
     - string
     - 1
     - O
     - ROR.org, ISNI, Wikidata
   * - 
     - email
     - email of the creator
     - string
     - 0..1
     - O
     - 
