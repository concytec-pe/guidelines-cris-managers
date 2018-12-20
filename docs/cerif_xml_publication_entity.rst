.. _publication:


Publication
===========
:Descripci�n: Una publicaci�n acad�mica basada en texto o canal de publicaci�n que contiene los resultados de la investigaci�n. Los CRIS suelen registrar metadatos sobre publicaciones acad�micas del �mbito de aplicaci�n de CRIS (CRIS institucional para la instituci�n, financiador de CRIS para la financiaci�n que distribuye, etc.) en el contexto de los proyectos de investigaci�n, la infraestructura, la financiaci�n, las unidades organizativas y los autores/contribuyentes. Esta entidad representa t�picamente el nivel de granularidad de un solo �tem publicado para el cual se adjunta informaci�n de atribuci�n (generalmente en forma de una lista de autores y contribuyentes). Esta entidad tambi�n se utiliza para representar canales y fuentes de publicaci�n: revistas y series de libros (incluida la continuaci�n de la serie de actas de conferencias). (Tomado de https://doi.org/10.1016/j.procs.2014.06.008)
:Ejemplos: `openaire_cerif_xml_example_publications.xml <https://github.com/openaire/guidelines-cris-managers/blob/v1.1/samples/openaire_cerif_xml_example_publications.xml>`_
:Representaci�n: Elemento XML ``Publication``; el resto de esta secci�n documenta los hijos de este elemento
:CERIF: la entidad ResultPublication (`<https://w3id.org/cerif/model#ResultPublication>`_)


Identificador interno
^^^^^^^^^^^^^^^^^^^^^
:Uso: Obligatorio (1)
:Representaci�n: Atributo XML ``id``
:CERIF: El atributo ResultPublicationIdentifier (`<https://w3id.org/cerif/model#ResultPublication.ResultPublicationIdentifier>`_)


Tipo
^^^^
:Descripci�n: El tipo de publicaci�n
:Uso: obligatorio (1)
:Representaci�n: Elemento XML ``Type`` desde el espacio de nombres `<https://www.openaire.eu/cerif-profile/vocab/COAR_Publication_Types>`_
:CERIF: the ResultPublication_Classification (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_)
:Vocabulary: Tipos de publicaci�n extra�dos del esquema conceptual COAR Resource Types: Tipos de publicaciones extra�dos del concepto de tipos de recursos COAR (http://vocabularies.coar-repositories.org/documentation/resource_types/, el t�rmino 'text' y sus descendientes en la jerarqu�a excepto 'patent').

  * **text** (`<http://purl.org/coar/resource_type/c_18cf>`_): Un recurso que consiste principalmente de palabras para leer. Los ejemplos incluyen libros, cartas, disertaciones, poemas, peri�dicos, art�culos, archivos de listas de correo. Tenga en cuenta que los facs�miles o im�genes de textos siguen siendo del g�nero Text.

    * **annotation** (`<http://purl.org/coar/resource_type/c_1162>`_): Una anotaci�n en el sentido de una nota legal es un comentario jur�dicamente explicativo de una decisi�n dictada por un tribunal judicial o arbitral.
    * **bibliography** (`<http://purl.org/coar/resource_type/c_86bc>`_): Una lista o enumeraci�n sistem�tica de obras escritas de un autor espec�fico o sobre un tema determinado.
    * **book** (`<http://purl.org/coar/resource_type/c_2f33>`_): Una publicaci�n no seriada que se completa en un volumen o en un n�mero limitado de vol�menes. (adapted from CiTO; EPrint Type vocabulary)

      * **book part** (`<http://purl.org/coar/resource_type/c_3248>`_):  Un cap�tulo o secci�n definida de un libro, generalmente con un t�tulo o n�mero separado.
    * **conference object** (`<http://purl.org/coar/resource_type/c_c94f>`_): Todo tipo de recursos digitales contribuyeron a una conferencia, como presentaciones de la conferencia (diapositivas), informes de la conferencia, conferencias, res�menes, demostraciones. En el caso de las ponencias, p�sters o actas de conferencias, se utilizar�n los conceptos espec�ficos..

      * **conference proceedings** (`<http://purl.org/coar/resource_type/c_f744>`_): Las actas de la conferencia son el registro oficial de una reuni�n de la conferencia. Se trata de una colecci�n de documentos que corresponde a las presentaciones realizadas en la conferencia. Puede incluir contenido adicional.

        * **conference paper** (`<http://purl.org/coar/resource_type/c_5794>`_): Un documento de la conferencia que se somete a una conferencia y se presenta a la audiencia. El documento de la conferencia se publica en las actas.
        * **conference poster** (`<http://purl.org/coar/resource_type/c_6670>`_): Un p�ster de la conferencia que se somete a una conferencia y se presenta all� en una presentaci�n de p�ster. El p�ster de la conferencia se publica en las actas.
      * **conference paper not in proceedings** (`<http://purl.org/coar/resource_type/c_18cp>`_): Un documento de la conferencia que se somete a una conferencia y se presenta a la audiencia. El documento de la conferencia no se publica en las actas.
      * **conference poster not in proceedings** (`<http://purl.org/coar/resource_type/c_18co>`_): Un p�ster de la conferencia que se somete a una conferencia y se presenta all� en una presentaci�n de p�ster. El p�ster de la conferencia no se publica en las actas.
    * **lecture** (`<http://purl.org/coar/resource_type/c_8544>`_): Transcripci�n de una charla pronunciada durante un evento acad�mico.
    * **letter** (`<http://purl.org/coar/resource_type/c_0857>`_): Una breve descripci�n de las nuevas e importantes investigaciones, tambi�n conocidas como "comunicaci�n". (adapted from EuroCRIS)
    * **periodical** (`<http://purl.org/coar/resource_type/c_2659>`_):  Una publicaci�n peri�dica es una publicaci�n que se publica de forma regular y continua en forma de una serie de n�meros. (Adapted from fabio)

      * **journal** (`<http://purl.org/coar/resource_type/c_0640>`_): Una publicaci�n peri�dica de art�culos de revistas (acad�micas). (Adapted from bibo)

        * **contribution to journal** (`<http://purl.org/coar/resource_type/c_3e5a>`_): Una contribuci�n a una revista denota un trabajo publicado en una revista. Si procede, se deben elegir los subt�rminos.

          * **journal article** (`<http://purl.org/coar/resource_type/c_6501>`_): Un art�culo sobre un tema en particular y publicado en un n�mero de la revista. (adapted from fabio)

            * **review article** (`<http://purl.org/coar/resource_type/c_dcae04bc>`_): Un art�culo de revisi�n es una fuente secundaria, es decir, est� escrito sobre otros art�culos, y no reporta investigaci�n original propia. (adapted from http://apus.libanswers.com/faq/2324)
            * **research article** (`<http://purl.org/coar/resource_type/c_2df8fbb1>`_): Un art�culo de investigaci�n es una fuente primaria, es decir, reporta los m�todos y resultados de un estudio original realizado por los autores. (adapted from http://apus.libanswers.com/faq/2324)
          * **editorial** (`<http://purl.org/coar/resource_type/c_b239>`_): Un ensayo breve que expresa la opini�n o posici�n de los redactores jefe de una revista (acad�mica) con respecto a un asunto pol�tico, social, cultural o profesional actual. Adapted from ODLIS
          * **data paper** (`<http://purl.org/coar/resource_type/c_beb9>`_): A data paper is a scholarly publication describing a particular dataset or group of dataset, published in the form of a peer-reviewed article in a scholarly journal. The main purpose of a data paper is to describe data, the circumstances of their collection, and information related to data features, access and potential reuse. Adapted from https://en.wikipedia.org/wiki/Data_paper and http://www.gbif.org/publishing-data/data-papers
          * **letter to the editor** (`<http://purl.org/coar/resource_type/c_545b>`_): A letter to the editor is a letter sent to a periodical about issues of concern from its readers. (adapted from Wikipedia)
    * **preprint** (`<http://purl.org/coar/resource_type/c_816b>`_): Pre-print describes the first draft of the article - before peer-review, even before any contact with a publisher. This use is common amongst academics for whom the key modification of an article is the peer-review process. Another use of the term pre-print is for the finished article, reviewed and amended, ready and accepted for publication - but separate from the version that is type-set or formatted by the publisher. This use is more common amongst publishers, for whom the final and significant stage of modification to an article is the arrangement of the material for putting to print.
    * **report** (`<http://purl.org/coar/resource_type/c_93fc>`_): A report is a separately published record of research findings, research still in progress, or other technical findings, usually bearing a report number and sometimes a grant number assigned by the funding agency. Also, an official record of the activities of a committee or corporate entity, the proceedings of a government body, or an investigation by an agency, whether published or private, usually archived or submitted to a higher authority, voluntarily or under mandate. In a more general sense, any formal account of facts or information related to a specific event or phenomenon, sometimes given at regular intervals.

      * **report part** (`<http://purl.org/coar/resource_type/c_ba1f>`_): part of a report
      * **internal report** (`<http://purl.org/coar/resource_type/c_18ww>`_): An internal report is a record of findings collected for internal use. It is not designed to be made public and may include confidential or proprietary information.
      * **memorandum** (`<http://purl.org/coar/resource_type/c_18wz>`_): It is a note, document or other communication that helps the memory by recording events or observations on a topic. A memorandum can have only a certain number of formats; it may have a format specific to an office or institution.
      * **other type of report** (`<http://purl.org/coar/resource_type/c_18wq>`_): Other types of report may include Business Plans Technical Specifications, data management plans, recommendation reports, white papers, annual reports, auditor's reports, workplace reports, census reports, trip reports, progress reports, investigative reports, budget reports, policy reports, demographic reports, credit reports, appraisal reports, inspection reports, military reports, bound reports, etc.
      * **policy report** (`<http://purl.org/coar/resource_type/c_186u>`_): A policy report is a type of report that provides an in-depth look at major policy developments and events
      * **project deliverable** (`<http://purl.org/coar/resource_type/c_18op>`_): A project deliverable is an �outcome� as a result of a project that is intended to be delivered to a customer (e.g. funder). Examples of deliverable are report, document, work package or any other building block of an overall project.
      * **report to funding agency** (`<http://purl.org/coar/resource_type/c_18hj>`_): A report to a funding agency is a document written by beneficiaries of project grants. The reporting documents can be e.g. periodic reports about progress of scientific and technical work and final report. For deliverables use �Project deliverable�.
      * **research report** (`<http://purl.org/coar/resource_type/c_18ws>`_): Research Reports are reports that typically provide an in-depth study of a particular topic or describe the results of a research project.
      * **technical report** (`<http://purl.org/coar/resource_type/c_18gh>`_): A technical report is a document that records the procedure adopted and results obtained from a scientific or technical activity or investigation.
    * **research proposal** (`<http://purl.org/coar/resource_type/c_baaf>`_): documentation for grant request
    * **review** (`<http://purl.org/coar/resource_type/c_efa0>`_): A review of others' published work.

      * **book review** (`<http://purl.org/coar/resource_type/c_ba08>`_): A written review and critical analysis of the content, scope and quality of a book or other monographic work.
    * **technical documentation** (`<http://purl.org/coar/resource_type/c_71bd>`_): Technical documentation refers to any type of documentation that describes handling, functionality and architecture of a technical product or a product under development or use.
    * **working paper** (`<http://purl.org/coar/resource_type/c_8042>`_): A working paper or preprint is a report on research that is still on-going or which has not yet been accepted for publication.
    * **thesis** (`<http://purl.org/coar/resource_type/c_46ec>`_): A thesis or dissertation is a document submitted in support of candidature for an academic degree or professional qualification presenting the author's research and findings.

      * **bachelor thesis** (`<http://purl.org/coar/resource_type/c_7a1f>`_): A thesis reporting a research project undertaken as part of an undergraduate course of education leading to a bachelor's degree.
      * **doctoral thesis** (`<http://purl.org/coar/resource_type/c_db06>`_): A thesis reporting the research undertaken during a period of graduate study leading to a doctoral degree.
      * **master thesis** (`<http://purl.org/coar/resource_type/c_bdcc>`_): A thesis reporting a research project undertaken as part of a graduate course of education leading to a master's degree.
    * **musical notation** (`<http://purl.org/coar/resource_type/c_18cw>`_): Musical notation is any system used to visually represent aurally perceived music through the use of written symbols, including ancient or modern musical symbols.



Language
^^^^^^^^
:Descripci�n: The language of the publication. Please use the IETF language tags as described in the IETF BCP 47 document.
:Uso: opcional (0..1)
:Representation: XML element ``Language``
:CERIF: the ResultPublication_Classification linking entity (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_) with the `<https://w3id.org/cerif/vocab/LanguageTags>`_ semantics


Title
^^^^^
:Descripci�n: The title of the publication
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``Title`` as a multilingual string
:CERIF: the ResultPublication.Title attribute (`<https://w3id.org/cerif/model#ResultPublication.Title>`_)



Subtitle
^^^^^^^^
:Descripci�n: The subtitle of the publication
:Uoe: opcional, possibly multiple (0..*)
:Representation: XML element ``Subtitle`` as a multilingual string
:CERIF: the ResultPublication.Subtitle attribute (`<https://w3id.org/cerif/model#ResultPublication.Subtitle>`_)



PublishedIn
^^^^^^^^^^^
:Description: The source (another Publication) where this publication appeared. E.g. a journal article lists here the journal where it appeared. To be used for a publishing channel.
:Use: optional (0..1)
:Representation: XML element ``PublishedIn`` with embedded XML element ``Publication``
:CERIF: the ResultPublication_ResultPublication linking entity (`<https://w3id.org/cerif/model#ResultPublication_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/Inter-PublicationRelations#Publication>`_ semantics (direction :1)


PartOf
^^^^^^
:Descripci�n: The Publication of which this publication is a part. E.g. a book chapter lists here the book that contains it. To be used for a containing publication.
:Uso: opcional (0..1)
:Representaci�n: XML element ``PartOf`` with embedded XML element ``Publication``
:CERIF: the ResultPublication_ResultPublication linking entity (`<https://w3id.org/cerif/model#ResultPublication_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/Inter-PublicationRelations#Part>`_ semantics (direction :1)


PublicationDate
^^^^^^^^^^^^^^^
:Descripci�n: The date the publication appeared
:Uso: opcional (0..1)
:Representaci�n: XML element ``PublicationDate``
:CERIF: the ResultPublication.ResPublDate attribute (`<https://w3id.org/cerif/model#ResultPublication.ResPublDate>`_)



Number
^^^^^^
:Descripci�n: The number of the publication (e.g. Article Number)
:Use: optional (0..1)
:Representation: XML element ``Number``
:CERIF: the ResultPublication.Number attribute (`<https://w3id.org/cerif/model#ResultPublication.Number>`_)



Volume
^^^^^^
:Descripci�n: The volume of the publishing channel where this publication appeared
:Use: optional (0..1)
:Representation: XML element ``Volume``
:CERIF: the ResultPublication.Volume attribute (`<https://w3id.org/cerif/model#ResultPublication.Volume>`_)



Issue
^^^^^
:Descripci�n: The issue of the publishing channel where this publication appeared
:Use: optional (0..1)
:Representation: XML element ``Issue``
:CERIF: the ResultPublication.Issue attribute (`<https://w3id.org/cerif/model#ResultPublication.Issue>`_)



Edition
^^^^^^^
:Descripci�n: The edition of the publication
:Use: optional (0..1)
:Representation: XML element ``Edition``
:CERIF: the ResultPublication.Edition attribute (`<https://w3id.org/cerif/model#ResultPublication.Edition>`_)



StartPage
^^^^^^^^^
:Descripci�n
: The page where this publication starts, in case the publishing channel or containing publication has numbered pages
:Use: optional (0..1)
:Representation: XML element ``StartPage``
:CERIF: the ResultPublication.StartPage attribute (`<https://w3id.org/cerif/model#ResultPublication.StartPage>`_)



EndPage
^^^^^^^
:Descripci�n: The page where this publication ends, in case the publishing channel or containing publication has numbered pages
:Uso: opcional (0..1)
:Representaci�n: XML element ``EndPage``
:CERIF: the ResultPublication.EndPage attribute (`<https://w3id.org/cerif/model#ResultPublication.EndPage>`_)



DOI
^^^
:Descripci�n: The Digital Object Identifier
:Uso: optional (0..1)
:Representaci�n: XML element ``DOI``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



Handle
^^^^^^
:Uso: opcional (0..1)
:Representaci�n: XML element ``Handle``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



PMCID
^^^^^
:Uso: opcional (0..1)
:Representaci�n: XML element ``PMCID``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



ISI-Number
^^^^^^^^^^
:Uso: opcional (0..1)
:Representaci�n: XML element ``ISI-Number``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



SCP-Number
^^^^^^^^^^
:Uso: opcional (0..1)
:Representaci�n: XML element ``SCP-Number``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



ISSN
^^^^
:Descripci�n: The International Standard Serial Number
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``ISSN``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



medium
------
:Uso: opcional
:Representaci�n: XML attribute ``medium``
:Vocabulario: ISSN Media List

  * **Print** (`<http://issn.org/vocabularies/Medium#Print>`_): Print (paper)
  * **Online** (`<http://issn.org/vocabularies/Medium#Online>`_): Online (online publication)
  * **Digital carrier** (`<http://issn.org/vocabularies/Medium#DigitalCarrier>`_): Digital carrier (CD-ROM, USB keys)
  * **Other** (`<http://issn.org/vocabularies/Medium#Other>`_): Other (Loose-leaf publications, braille, etc.)



ISBN
^^^^
:Descripci�n: The International Standard Book Number
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``ISBN``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



medium
------
:Uso: opcional
:Representaci�n: XML attribute ``medium``
:Vocabulario: ISSN Media List

  * **Print** (`<http://issn.org/vocabularies/Medium#Print>`_): Print (paper)
  * **Online** (`<http://issn.org/vocabularies/Medium#Online>`_): Online (online publication)
  * **Digital carrier** (`<http://issn.org/vocabularies/Medium#DigitalCarrier>`_): Digital carrier (CD-ROM, USB keys)
  * **Other** (`<http://issn.org/vocabularies/Medium#Other>`_): Other (Loose-leaf publications, braille, etc.)



URL
^^^
:Uso: optional (0..1)
:Representaci�n: XML element ``URL``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



URN
^^^
:Uso: opcional (0..1)
:Representaci�n: XML element ``URN``
:CERIF: the FederatedIdentifier entity (`<https://w3id.org/cerif/model#FederatedIdentifier>`_)



Authors
^^^^^^^
:Descripci�n: The authors of this publication
:Uso: opcional (0..1)
:Representaci�n: XML element ``Authors`` with ordered embedded XML elements ``Author`` that can contain an embedded person with affiliations or organisation unit



Author
------
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``Author`` with embedded XML element ``Person`` optionally followed by one or several ``Affiliation`` elements, or ``OrgUnit``
:CERIF: the Person_ResultPublication linking entity (`<https://w3id.org/cerif/model#Person_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/PersonOutputContributions#Author>`_ semantics; the OrganisationUnit_ResultPublication linking entity (`<https://w3id.org/cerif/model#OrganisationUnit_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/OrganisationOutputContributions#Author>`_ semantics


Editors
^^^^^^^
:Descripci�n: The editors of this publication
:Uso: opcional (0..1)
:Representaci�n: XML element ``Editors`` with ordered embedded XML elements ``Editor`` that can contain an embedded person with affiliations or organisation unit



Editor
------
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``Editor`` with embedded XML element ``Person`` optionally followed by one or several ``Affiliation`` elements, or ``OrgUnit``
:CERIF: the Person_ResultPublication linking entity (`<https://w3id.org/cerif/model#Person_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/PersonOutputContributions#Editor>`_ semantics; the OrganisationUnit_ResultPublication linking entity (`<https://w3id.org/cerif/model#OrganisationUnit_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/OrganisationOutputContributions#Editor>`_ semantics


Publishers
^^^^^^^^^^
:Descripci�n: The publishers of this publication
:Uso: optional (0..1)
:Representaci�n: XML element ``Publishers`` with ordered embedded XML elements ``Publisher`` that can contain an embedded organisation unit or person



Publisher
---------
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``Publisher`` with embedded XML element ``OrgUnit`` or ``Person``
:CERIF: the OrganisationUnit_ResultPublication linking entity (`<https://w3id.org/cerif/model#OrganisationUnit_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/OrganisationOutputContributions#Publisher>`_ semantics; the Person_ResultPublication linking entity (`<https://w3id.org/cerif/model#Person_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/PersonOutputContributions#Publisher>`_ semantics


License
^^^^^^^
:Descripci�n: The license of the publication
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``License`` containing the classification identifier and having a ``scheme`` attribute to specify the classification scheme identifier
:CERIF: the ResultPublication_Classification (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_)


Subject
^^^^^^^
:Descripci�n: The subject of the publication from a classification
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``Subject`` containing the classification identifier and having a ``scheme`` attribute to specify the classification scheme identifier
:CERIF: the ResultPublication_Classification (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_)


Keyword
^^^^^^^
:Descripci�n: A single keyword or key expression. Please repeat to serialize separate keywords or key expressions.
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``Keyword`` as a multilingual string
:CERIF: the ResultPublication.Keywords attribute (`<https://w3id.org/cerif/model#ResultPublication.Keywords>`_)



Abstract
^^^^^^^^
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``Abstract`` as a multilingual string
:CERIF: the ResultPublication.Abstract attribute (`<https://w3id.org/cerif/model#ResultPublication.Abstract>`_)



Status
^^^^^^
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``Status`` containing the classification identifier and having a ``scheme`` attribute to specify the classification scheme identifier
:CERIF: the ResultPublication_Classification (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_)


OriginatesFrom
^^^^^^^^^^^^^^
:Uso: optional, possibly multiple (0..*)
:Representaci�n: XML element ``OriginatesFrom`` with embedded XML element ``Project`` or ``Funding``
:CERIF: the Project_ResultPublication linking entity (`<https://w3id.org/cerif/model#Project_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/Project_Output_Roles#Originator>`_ semantics; the ResultPublication_Funding linking entity (`<https://w3id.org/cerif/model#ResultPublication_Funding>`_) with the `<https://w3id.org/cerif/vocab/Funding_Output_Roles#Originator>`_ semantics


PresentedAt
^^^^^^^^^^^
:Descripci�n: The event where this publication was presented.  [#]_ 
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``PresentedAt`` with embedded XML element ``Event``
:CERIF: the ResultPublication_Event linking entity (`<https://w3id.org/cerif/model#ResultPublication_Event>`_) with the `<https://w3id.org/cerif/vocab/EventOutputRelationships#Presented>`_ semantics

.. [#] Note: Video recordings of conference presentations are stored as alternative representations of the primary object: the conference paper. It would be unneccessarily complex to represent them as separate, linked Products.


OutputFrom
^^^^^^^^^^
:Descripci�n: This publication contains the proceedings from the linked event
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``OutputFrom`` with embedded XML element ``Event``
:CERIF: the ResultPublication_Event linking entity (`<https://w3id.org/cerif/model#ResultPublication_Event>`_) with the `<https://w3id.org/cerif/vocab/EventOutputRelationships#Output>`_ semantics


Coverage
^^^^^^^^
:Descripci�n: The event that is covered by this publication (e.g. a report about the event)
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``Coverage`` with embedded XML element ``Event``
:CERIF: the ResultPublication_Event linking entity (`<https://w3id.org/cerif/model#ResultPublication_Event>`_) with the `<https://w3id.org/cerif/vocab/EventOutputRelationships#Coverage>`_ semantics


References
^^^^^^^^^^
:Descripci�n: Result outputs that are referenced by this publication
:Uso: opcional, possibly multiple (0..*)
:Representaci�n: XML element ``References`` with embedded XML element ``Publication`` or ``Patent`` or ``Product``
:CERIF: the ResultPublication_ResultPublication linking entity (`<https://w3id.org/cerif/model#ResultPublication_ResultPublication>`_) with the `<https://w3id.org/cerif/vocab/Inter-OutputRelations#Reference>`_ semantics (direction :1); the ResultPublication_ResultProduct linking entity (`<https://w3id.org/cerif/model#ResultPublication_ResultProduct>`_) with the `<https://w3id.org/cerif/vocab/Inter-OutputRelations#Reference>`_ semantics (direction :1); the ResultPublication_ResultPatent linking entity (`<https://w3id.org/cerif/model#ResultPublication_ResultPatent>`_) with the `<https://w3id.org/cerif/vocab/Inter-OutputRelations#Reference>`_ semantics (direction :1)


ns4:Access
^^^^^^^^^^
:Descripci�n: The open access type of the publication
:Uso: opcional (0..1)
:Representaci�n: XML element ``Access`` from namespace `<http://purl.org/coar/access_right>`_
:CERIF: the ResultPublication_Classification (`<https://w3id.org/cerif/model#ResultPublication_Classification>`_)
:Vocabulario: 

  * **open access** (`<http://purl.org/coar/access_right/c_abf2>`_): Open access refers to a resource that is immediately and permanently online, and free for all on the Web, without financial and technical barriers.
  * **embargoed access** (`<http://purl.org/coar/access_right/c_f1cf>`_): Embargoed access refers to a resource that is metadata only access until released for open access on a certain date. Embargoes can be required by publishers and funders policies, or set by the author (e.g such as in the case of theses and dissertations).
  * **restricted access** (`<http://purl.org/coar/access_right/c_16ec>`_): Restricted access refers to a resource that is available in a system but with some type of restriction for full open access. This type of access can occur in a number of different situations. Some examples are described below: The user must log-in to the system in order to access the resource The user must send an email to the author or system administrator to access the resource Access to the resource is restricted to a specific community (e.g. limited to a university community)
  * **metadata only access** (`<http://purl.org/coar/access_right/c_14cb>`_): Metadata only access refers to a resource in which access is limited to metadata only. The resource itself is described by the metadata, but is not directly available through the system or platform. This type of access can occur in a number of different situations. Some examples are described below: There is no electronic copy of the resource available (record links to a physical resource) The resource is only available elsewhere for a fee (record links to a subscription-based publisher version) The resource is available open access but at a different location (record links to a version at an open access publisher or archive) The resource is available elsewhere, but not in a fully open access format (record links to a read only, or other type of resources that is not permanent or in some way restricted)
  
  