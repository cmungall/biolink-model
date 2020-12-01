---
parent: Associations
title: biolink:ExposureEventToPhenotypicFeatureAssociation
grand_parent: Classes
layout: default
---

# Class: ExposureEventToPhenotypicFeatureAssociation


Any association between an environment and a phenotypic feature, where being in the environment influences the phenotype

URI: [biolink:ExposureEventToPhenotypicFeatureAssociation](https://w3id.org/biolink/vocab/ExposureEventToPhenotypicFeatureAssociation)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[ThingToPhenotypicFeatureAssociationMixin],[SeverityValue],[Publication],[OntologyClass],[Onset],[NamedThing],[FrequencyValue],[ExposureEvent]%3Csubject%201..1-%20[ExposureEventToPhenotypicFeatureAssociation%7Cdescription:narrative_text%20%3F;id(i):string;predicate(i):predicate_type;relation(i):uriorcurie;negated(i):boolean%20%3F],[ExposureEventToPhenotypicFeatureAssociation]uses%20-.-%3E[ThingToPhenotypicFeatureAssociationMixin],[Association]%5E-[ExposureEventToPhenotypicFeatureAssociation],[ExposureEvent],[BiologicalSex],[Attribute],[Association],[Agent])

---


## Parents

 *  is_a: [Association](Association.md) - A typed association between two entities, supported by evidence

## Uses Mixins

 *  mixin: [ThingToPhenotypicFeatureAssociationMixin](ThingToPhenotypicFeatureAssociationMixin.md)

## Referenced by class


## Attributes


### Own

 * [exposure event to phenotypic feature association➞subject](exposure_event_to_phenotypic_feature_association_subject.md)  <sub>REQ</sub>
    * range: [ExposureEvent](ExposureEvent.md)

### Inherited from association:

 * [association➞id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [predicate](predicate.md)  <sub>REQ</sub>
    * Description: A high-level grouping for the relationship type. AKA minimal predicate. This is analogous to category for nodes.
    * range: [PredicateType](types/PredicateType.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: The relation which describes an association between a subject and an object in a more granular manner. Usually this is a term from Relation Ontology, but it can be any edge CURIE.
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](types/Boolean.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Agent](Agent.md)

### Inherited from entity to feature or disease qualifiers mixin:

 * [severity qualifier](severity_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state how severe the phenotype is in the subject
    * range: [SeverityValue](SeverityValue.md)
 * [onset qualifier](onset_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state when the phenotype appears is in the subject
    * range: [Onset](Onset.md)

### Inherited from frequency qualifier mixin:

 * [frequency qualifier](frequency_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state how frequent the phenotype is observed in the subject
    * range: [FrequencyValue](FrequencyValue.md)

### Inherited from material sample:

 * [has attribute](has_attribute.md)  <sub>0..*</sub>
    * Description: connects any named thing to an attribute
    * range: [Attribute](Attribute.md)
    * in subsets: (samples)

### Inherited from thing to phenotypic feature association mixin:

 * [sex qualifier](sex_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state whether the association is specific to a particular sex.
    * range: [BiologicalSex](BiologicalSex.md)
 * [thing to phenotypic feature association mixin➞description](thing_to_phenotypic_feature_association_mixin_description.md)  <sub>OPT</sub>
    * Description: A description of specific aspects of this phenotype, not otherwise covered by the phenotype ontology class
    * range: [NarrativeText](types/NarrativeText.md)
 * [thing to phenotypic feature association mixin➞object](thing_to_phenotypic_feature_association_mixin_object.md)  <sub>REQ</sub>
    * Description: phenotypic class
    * range: [PhenotypicFeature](PhenotypicFeature.md)
    * Example:    
    * Example:    
    * Example:    

### Domain for slot:

 * [exposure event to phenotypic feature association➞subject](exposure_event_to_phenotypic_feature_association_subject.md)  <sub>REQ</sub>
    * range: [ExposureEvent](ExposureEvent.md)