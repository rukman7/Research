# Project idea

## Attribute based access control

Attribute based access control is one of the ways to manage & control access to data in a system. A set of attributes shall be assigned to every user based on the resources that they shall access. 

## Components to ABAC

Components of ABAC
There are several components involved in Attribute-Based Access Control, which are common throughout each organization, regardless of the company structure or industry it belongs to.

### 1. Subject
In ABAC, the subject refers to the user requesting access to a resource for a task. Some of the user attributes of the subject include the subject ID, job roles, group memberships, organizational memberships, management level, and other unique factors. In an ABAC system, this information is obtained through an HR portal or employee directory.

### 2. Resource
The resource refers to the object, i.e. the file, document, application, network resource, or any other thing that the subject is requesting permission to access. The identifying characteristics of the resource include the creation date, owner, name, type, and data sensitivity.

### 3. Action
The action describes the intent of the subject, i.e. what they want to do with the resource being requested. Some of the common actions include ‘read, ‘write’, ‘copy’, ‘edit’, and ‘delete’. In most cases, users may ask for multiple actions, such as edit and copy, or read and edit.

### 4. Environment
The environment describes the entire landscape of the access request, and it contains information like the time and location of the access request, the subject’s device, communication protocol, encryption strength, etc.

The ABAC makes use of these attributes and components to develop access control policies, which also align with the rules. The rules also define the attribute combinations that can be paired together for a subject to perform the action with an object.

## Policy evaluation

Every resource has a policy assigned to it. A policy can be thought of as a set of conditions which will determine if a resource can be accessed by an user. Every time an user makes a request to a resource, Policy evaluation happens and based on it's output, the user is either permitted or denied access to the resource. 

Multiple policies can be associated with every component of an ABAC sytem.

For example,

1. Allow doctors to view medical records only for their patients
2. Allow doctors to view medical records for other patients in medical emergencies.

The latter is sometimes called "break glass" policy. These can be thought of as overrides. 

## Changes to the Policy

As the system grows, new users & new resources will be created which would lead to creating new set of attributes which require updates to the existing policies or creating new ones. 


## Testing the system
Often times close monitoring & testing is required for keeping track of the updates to the policy.

New policies or changes to the existing policies can break the existing policies which may lead to bugs.


## Bugs in the ABAC system

Like any issues in a security system, Bugs in the ABAC system could lead to devasting outcomes. 

## Research area

Research efforts can be directed at finding an easy way to find all possible test cases. A test case would consist of a description of the test to be executed and the expected result (in our case it will be wether if an operation is permission or not permitted)

One such path is exploring & behaviour driven approaches to better understand the use cases. If there is a possible way to generalize the way we define policys through behaviour driven approaches, it may lead to predecting the output of the system. This could help us find or gather all the test cases for the ABAC system.

## NGAC - Next Generation Access Control

-  Apart from conventional access controls, the NGAC provides additional capabilities to filter or control data access at the SQL query level. It supports query altering to hide unaccessible data based on an user's role.

-  It uses associations to provide access rights

Example: alice -- r,w -- public

The above means that alice can perform read and write operations on all the public records.

-  Use of set operation for creating new object and assigning it to the existing attributes.

Creating object x in y

```
if x is not an existing object and y is an existing attribute:
{
    O' = O U {x}
    Assign' = Assign U {(x,y)}
}

```

## Resources referred

Axiomatics - demo videos & blogs:

    This gave me a clear picture about ABAC system & policy evaluation in general. 

Next generation access control - NGAC

Ontology

OWL

Protege tool

[visualize ontology](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbDA1UWFrMWkwZ19pZmdlSlN1Y045dlNPV3BZQXxBQ3Jtc0trZDl5TFZUWEdBVldOQ3hRMW9CTVBnWWVDMERFMVlIV21JUkpyTVhfMFNoTXd2eXRVRGVWVTBSWWlNeU1wQmJFZF92TzFkMFZGZTVlRzkxaDFfRHAyVjN1aUtFQ3gycE9CdXQxcFFmdDNTMmY1Q3gtTQ&q=http%3A%2F%2Fvowl.visualdataweb.org%2Fwebvowl.html&v=JiGRVIQ9rks)
This site can be used to create and visualize ontologies

Behaviour driven approaches:

     Yet to fully explore this.

## Ontology

- Address questions related to categorizing, classification and explanation of entities
- A branch of philosophy

Definition:

Ontologies are described way of showing the properties of a subject area and how they are related, by defining set of concepts and categories that represent the subject.

Components in an ontology

Concepts:
- Concepts represent a set of classes or entities within a domain, which are used to classify individuals or other classes or combination of both.

Instances:
- Instances are used to refer things that are represented by a concept

Relationship:
- Relationships specify how objects are related to one another

Note: The oncology design concepts are very much similar to an object oriented programming.

## Protege

-  Protege is an open source tool used to create, upload, modify and visualize ontologies.  

Axioms

The main component of an OWL 2 ontology is a set of axioms — statements that say what is true in the domain. OWL 2 provides an extensive set of axioms, all of which extend the Axiom class in the structural specification. Axioms in OWL 2 can be declarations, axioms about classes, axioms about object or data properties, datatype definitions, keys, assertions (sometimes also called facts), and axioms about annotations.


## Useful links and resources

1. NGAC - Next Generation Access control
[https://csrc.nist.gov/CSRC/media/Projects/Policy-Machine/documents/NGAC_Control_over-SQL_Queries_v6.pdf](https://csrc.nist.gov/CSRC/media/Projects/Policy-Machine/documents/NGAC_Control_over-SQL_Queries_v6.pdf)

2. Ontology
[https://warwick.ac.uk/fac/soc/ces/research/current/socialtheory/maps/ology/](https://warwick.ac.uk/fac/soc/ces/research/current/socialtheory/maps/ology/)

3. Stanford protege documentation
[https://protege.stanford.edu/support.php#documentationSupport](https://protege.stanford.edu/support.php#documentationSupport)


4. Wine data set - ontology - owl
[https://archivo.dbpedia.org/info?o=http://www.w3.org/TR/2003/CR-owl-guide-20030818/wine](https://archivo.dbpedia.org/info?o=http://www.w3.org/TR/2003/CR-owl-guide-20030818/wine)


5. Protege - tutorial
[https://www.youtube.com/watch?v=LQ4iW3PO36E](https://www.youtube.com/watch?v=LQ4iW3PO36E)

6. Web Ontology Language - OWL
[https://www.youtube.com/watch?v=JiGRVIQ9rks](https://www.youtube.com/watch?v=JiGRVIQ9rks)

7. Creating ontology using protege

[https://youtu.be/CduRWyyL3q8](https://youtu.be/CduRWyyL3q8)