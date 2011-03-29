PBCore 2.0
==========

PBCore is a metadata standard designed to describe media, both digital and analog. Most importantly, it was designed for the Internet, and for the kinds of software applications we now use to manage, access, and share media files.

The PBCore schema is the blueprint for organizing a specified set of metadata when expressed as XML. We might have a media catalog that holds our metadata in a database, or a simple spreadsheet with titles, descriptions, etc. In fact many of us will probably always use various databases and desktop tools to form the core of our media asset management systems. PBCore XML provides a common format for these systems to talk to each other and share metadata.

The PBCore schema serves as a guide for developers of applications that “speak PBCore.” The schema also makes it possible to automatically validate PBCore records and ensure data compatibility between systems.
What’s New in 2.0

Since its introduction in 2005, PBCore has gained wide acceptance because it provides a thorough yet simple way to describe media assets. The 2.0 schema builds on the main PBCore elements without compromising its ease of use. That said, those familiar with PBCore 1.x will recognize significant differences:

* The addition of optional attributes in many elements.
* The ability to describe “multi-part instantiations,” i.e. a single media production comprised of more than one film, tape, or file.
* The inclusion of rights information at the Instantiation level, not just the Intellectual Description level.
* The option to include markup from other existing rights metadata standards, e.g. ODRL or Creative Commons.
* A simple way to show relationships between Instantiations, for example that an MPEG4 Instantiation was encoded from a QuickTime Instantiation.
* The ability to specify time-based metadata within an asset, e.g. where exactly in the timeline a particular subject is discussed or a specific person appears.
* New core elements that resolve thorny issues encountered by PBCore users: pbcoreAssetType allows you to indicate the “broad editorial format” of the asset, e.g. a program, a clip, an episode, or a scene.
* pbcoreAssetDate provides, for the first time, a way to specify the creation date of the asset, not just its Instantiations.
* It is now valid to have an asset with no Instantiations, so you can have an Intellectual Description of an asset for which no Instantiations yet exist. And conversely, you can have an Instantiation Only asset with the new root tag pbcoreInstantiationDocument.
* The addition of a new pbcoreCollection element allows the wrapping of many pbcoreDescriptionDocuments in a collection of assets for easy exchange with other systems. You can now have a PBCore “feed,” and use PBCore in RESTful web applications.
* A new pbcorePart element allows for defining segments, stories, and clips within an asset, and nested relationships between assets and asset parts.
* Extensions are now available at the Asset, Instantiation and EssenceTrack level, and can include metadata and markup from other standards.

Toward a more semantic web
--------------------------

Since 2004, PBCore has been used as a standard to catalog media and exchange metadata. It has been adopted by a growing number of public media organizations, film archives, academic institutions, and technology vendors. But until now, there was no direct way to connect PBCore metadata to the growing universe of linked data on the web.

The introduction of optional attributes in the 2.0 schema clears the way for true PBCore semantic web applications. For example, we can specify a subject term and include not just the name of a subject authority, but the URI to an authoritative subject definition. Other resources on the web that are linked to that subject term can now be related to our media asset. We can also include link attributes for pbcoreCreators and pbcoreContributors, pbcoreRelations, and many other elements.

As more PBCore assets include such unambiguous links to subject terms, people, and other media assets, it becomes possible to crawl and map many such relationships. For example, a lecture by Langston Hughes can automatically link to other Langston Hughes-related resources. By using the new “ref” attribute to specify URIs for PBCore element values, we make our media assets part of the expanding universe of linked data and semantically-enabled content.
Keeping it simple enough to use

The required core elements of PBCore have not changed in the 2.0 schema. Attributes, collections, and parts are all optional. In fact, PBCore still requires only three elements: Identifier, Title, and Description; all other elements are optional. PBCore 2.0 retains the simplicity of PBCore 1.x and remains faithful to its origins in Dublin Core.

What the 2.0 schema does is fix problems identified by the PBCore user community. Many people contributed change requests, blog posts, questions, commentary, criticism, and research. The development and review teams solicited additional feedback on early versions. As they work with PBCore 2.0, users will undoubtedly discover things that can be further refined and improved. The [PBCore 2.0 Schema](http://pbcore.org/schema/) is the result of a true community effort, and that effort should continue.

You will discover more as you explore PBCore 2.0 and begin using it with your assets and collections. The Schema Review team believes this release is a huge step forward to improve the standard, but as always, we look forward to your comments.

Use of this repository
----------------------

The PBCore team has decied to open the PBCore 2.0 repostiory in order to better share the deliberations that went in to making version 2.0 and also to allow an even wider community to participate in revisions. 

If there are changes you would like to recommend for the next version of PBCore, you can submit issues through the issue tracker on GitHub (look for the Issues tab above). And if you want to submit patches to the schema, please fork this repository and push them. We will consider your patches for the next release of PBCore (which has not yet been scheduled). 

As always, you can also comment on PBCore at [PBcore.org](http://pbcore.org) and at [PBCoreResources.org](http://pbcoreresources.org/).

