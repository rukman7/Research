### Project idea

## Attribute based access control

Attribute based access control is one of the ways to manage & control access to data in a system. A set of attributes shall be assigned to every user based on the resources that they shall access. 

## Policy evaluation

Every resource has a policy assigned to it. A policy can be thought of as a set of conditions which will determine if a resource can be accessed by an user. Every time an user makes a request to a resource, Policy evaluation happens and based on it's output, the user is either permitted or denied access to the resource. 

## Changes to the Policy

As the system grows, new users & new resources will be created which would leads to creating new set of attributes which require updates to the existing policies or creating new ones. 


## Testing the system
Often times close monitoring & testing is required for keeping track of the updates to the policy.

New policies or changes to the existing policies can break the existing policies which may lead to bugs.


## Bugs in the ABAC system

Like any issues in a security system, Bugs in the ABAC system could lead to devasting outcomes. 

## Research area

Research efforts can be directed at finding an easy way to find all possible test cases. A test case would consist of a description of the test to be executed and the expected result (in our case it will be wether if an operation is permission or not permitted)

One such path is exploring & behaviour driven approaches to better understand the use cases. If there is a possible way to generalize the way we define policys through behaviour driven approaches, it may lead to predecting the output of the system. This could help us find or gather all the test cases for the ABAC system.

## Resources referred

Axiomatics - demo videos & blogs:

    This gave me a clear picture about ABAC system & policy evaluation in general. 

Behaviour driven approaches:

     Yet to fully explore this.