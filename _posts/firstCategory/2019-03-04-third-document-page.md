---
layout: post
title:  "Third Document Page"
date:   2019-03-04 08:00:00
categories: ['First Category']
permalink: /firstCategory/third-document-page/
---

[My PDF Document](../../../MyCreds.PDF)
### Sprint Lifecycle

- [Sprint Lifecycle1](#sprint-lifecycle)
- [Sprint Lifecycle2](#sprint-lifecycle)
- [Sprint Lifecycle3](#sprint-lifecycle)

# This is a H1 header
## This is a H2 header
### This is a H3 header
#### This is a H4 header
##### This is a H5 header  

> Single line quote
>> Nested quote
>> multiple line
>> quote
 
Add line below  

----

Use _emphasis_ in comments to express **strong** opinions and point out ~~corrections~~  
**_Bold, italicized text_**  
**~~Bold, strike-through text~~**

#### Code sample below

```
sudo npm install vsoagent-installer -g  
```

#### Sample of a table

| Heading 1 | Heading 2 | Heading 3 |  
|-----------|:-----------:|-----------:|  
| Cell A1 | Cell A2 | Cell A3 |  
| Cell B1 | Cell B2 | Cell B3<br/>second line of text |

#### List
1. First item.
1. Second item.
1. Third item.

#### Bulleted Lists
- Item 1
- Item 2
- Item 3

#### Nested Lists
1. First item.
   - Item 1
   - Item 2
   - Item 3
1. Second item.
   - Nested item 1
      - Further nested item 1
      - Further nested item 2
      - Further nested item 3
   - Nested item 2
   - Nested item 3

#### Link Sample
[Azure Wiki Documentation](https://learn.microsoft.com/en-us/azure/devops/project/wiki/markdown-guidance?view=azure-devops)

[Link to the top of the page](#sprint-lifecycle)

![Illustration to use for new users](./images/doubles_img_1.png)

Format a list as a task list

- [ ] A  
- [ ] B  
- [ ] C  
- [x] A  
- [x] B  
- [x] C  

$
\alpha, \beta, \gamma, \delta, \epsilon, \zeta, \eta, \theta, \kappa, \lambda, \mu, \nu, \omicron, \pi, \rho, \sigma, \tau, \upsilon, \phi, ...
$  


$\Gamma,  \Delta,  \Theta, \Lambda, \Xi, \Pi, \Sigma, \Upsilon, \Phi, \Psi, \Omega$

Area of a circle is $\pi r^2$

And, the area of a triangle is:

$$
A_{triangle}=\frac{1}{2}({b}\cdot{h})
$$

$$
\sum_{i=1}^{10} t_i
$$


$$
\int_0^\infty \mathrm{e}^{-x}\,\mathrm{d}x
$$     

#### Sequence diagram

::: mermaid
sequenceDiagram
    Christie->>Josh: Hello Josh, how are you?
    Josh-->>Christie: Great!
    Christie->>Josh: See you later!
:::

#
A Gantt Chart below:

::: mermaid
gantt
    title A Gantt chart
    dateFormat YYYY-MM-DD
    excludes 2022-03-16,2022-03-18,2022-03-19
    section Section

    A task          :a1, 2022-03-07, 7d
    Another task    :after a1 , 5d
:::

#
A FlowChart diagram below:
:::mermaid
graph LR;
    A[Hard edge] -->|Link text| B(Round edge) --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
:::

# A Class Diagram below:

:::mermaid
classDiagram
    Creature <|-- Superman
    Creature <|-- Vampire
    Creature <|-- Diavolo
    Creature: +int size
    Creature: +int weight
    Creature: +isBenign()
    Creature: +power()
    class Superman{
        +String currentName
        +fly()
        +heal()
    }
    class Vampire{
        -int age
        -canBite()
    }
    class Diavolo{
        +bool is_serving
        +heat()
    }
:::

#
A State Diagram below:
:::mermaid
stateDiagram-v2
    [*] --> Active
    state Active {
        [*] --> NumLockOff
        NumLockOff --> NumLockOn : EvNumLockPressed
        NumLockOn --> NumLockOff : EvNumLockPressed
        --
        [*] --> CapsLockOff
        CapsLockOff --> CapsLockOn : EvCapsLockPressed
        CapsLockOn --> CapsLockOff : EvCapsLockPressed
        --
        [*] --> ScrollLockOff
        ScrollLockOff --> ScrollLockOn : EvScrollLockPressed
        ScrollLockOn --> ScrollLockOff : EvScrollLockPressed
    }
:::

# 
A Requirement Diagram below:
:::mermaid
requirementDiagram
    requirement development_req {
    id: 1
    text: requirements spec.
    risk: medium
    verifymethod: test
    }
    element test_suite {
    type: manual test
    }
    test_suite - verifies -> development_req
:::

::: video
<iframe width="560" height="315" src="https://www.youtube.com/embed/OtqFyBA6Dbk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
:::

#
A Journey Example below:
:::mermaid
journey
    title Home office day
    section Go to work
      Wake up: 1: Me, Dog
      Take shower: 2: Me
      Go downstairs: 3: Me, Dog
      Make coffee: 4: Me
      Have a breakfast: 5: Me, Dog
      Go upstairs: 3: Me, Dog
      Do work: 1: Me, Dog
    section Go home
      Go downstairs: 3: Me, Dog
      Sit down: 5: Me
:::

# Swagger Petstore YAML
This is a sample server Petstore server.  You can find out more about Swagger at <a href="<http://swagger.io>">http://swagger.io</a> or on irc.freenode.net, #swagger.  For this sample, you can use the api key "special-key" to test the authorization filters

## Version: 1.0.0

### Terms of service
<http://swagger.io/terms/>

**Contact information:**  
apiteam@swagger.io  

**License:** [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

[Find out more about Swagger](http://swagger.io)

### Security
**petstore_auth**  

| oauth2 | *OAuth 2.0* |
| ------ | ----------- |
| Authorization URL | <http://petstore.swagger.io/api/oauth/dialog> |
| Flow | implicit |
| **Scopes** |  |
| write:pets | modify pets in your account |
| read:pets | read your pets |

**api_key**  

| apiKey | *API Key* |
| ------ | --------- |
| Name | api_key |
| In | header |

## pet
Everything about your Pets
[Find out more](http://swagger.io)

### /pet

#### POST
##### Summary

Add a new pet to the store

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | Pet object that needs to be added to the store | No | [Pet](#pet) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 405 | Invalid input |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

#### PUT
##### Summary

Update an existing pet

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | Pet object that needs to be added to the store | No | [Pet](#pet) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Invalid ID supplied |
| 404 | Pet not found |
| 405 | Validation exception |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

### /pet/findByStatus

#### GET
##### Summary

Finds Pets by status

##### Description

Multiple status values can be provided with comma separated strings

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| status | query | Status values that need to be considered for filter | No | [ string ] |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [ [Pet](#pet) ] |
| 400 | Invalid status value |  |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

### /pet/findByTags

#### GET
##### Summary

Finds Pets by tags

##### Description

Multiple tags can be provided with comma separated strings. Use tag1, tag2, tag3 for testing.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| tags | query | Tags to filter by | No | [ string ] |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [ [Pet](#pet) ] |
| 400 | Invalid tag value |  |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

### /pet/{petId}

#### GET
##### Summary

Find pet by ID

##### Description

Returns a single pet

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| petId | path | ID of pet to return | Yes | long |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [Pet](#pet) |
| 400 | Invalid ID supplied |  |
| 404 | Pet not found |  |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| api_key |  |  |
| petstore_auth | write:pets | read:pets |

#### POST
##### Summary

Updates a pet in the store with form data

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| petId | path | ID of pet that needs to be updated | Yes | string |
| name | formData | Updated name of the pet | No | string |
| status | formData | Updated status of the pet | No | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 405 | Invalid input |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

#### DELETE
##### Summary

Deletes a pet

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| api_key | header |  | No | string |
| petId | path | Pet id to delete | Yes | long |

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Invalid pet value |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

### /pet/{petId}/uploadImage

#### POST
##### Summary

uploads an image

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| petId | path | ID of pet to update | Yes | long |
| additionalMetadata | formData | Additional data to pass to server | No | string |
| file | formData | file to upload | No | file |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [ApiResponse](#apiresponse) |

##### Security

| Security Schema | Scopes |  |
| --------------- | ------ | --- |
| petstore_auth | write:pets | read:pets |

## store
Operations about user

### /store/inventory

#### GET
##### Summary

Returns pet inventories by status

##### Description

Returns a map of status codes to quantities

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | object |

##### Security

| Security Schema | Scopes |
| --------------- | ------ |
| api_key |  |

### /store/order

#### POST
##### Summary

Place an order for a pet

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | order placed for purchasing the pet | No | [Order](#order) |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [Order](#order) |
| 400 | Invalid Order |  |

### /store/order/{orderId}

#### GET
##### Summary

Find purchase order by ID

##### Description

For valid response try integer IDs with value <= 5 or > 10. Other values will generated exceptions

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| orderId | path | ID of pet that needs to be fetched | Yes | string |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [Order](#order) |
| 400 | Invalid ID supplied |  |
| 404 | Order not found |  |

#### DELETE
##### Summary

Delete purchase order by ID

##### Description

For valid response try integer IDs with value < 1000. Anything above 1000 or nonintegers will generate API errors

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| orderId | path | ID of the order that needs to be deleted | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Invalid ID supplied |
| 404 | Order not found |

## user
Access to Petstore orders
[Find out more about our store](http://swagger.io)

### /user

#### POST
##### Summary

Create user

##### Description

This can only be done by the logged in user.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | Created user object | No | [User](#user) |

##### Responses

| Code | Description |
| ---- | ----------- |
| default | successful operation |

### /user/createWithArray

#### POST
##### Summary

Creates list of users with given input array

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | List of user object | No | [ [User](#user) ] |

##### Responses

| Code | Description |
| ---- | ----------- |
| default | successful operation |

### /user/createWithList

#### POST
##### Summary

Creates list of users with given input array

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| body | body | List of user object | No | [ [User](#user) ] |

##### Responses

| Code | Description |
| ---- | ----------- |
| default | successful operation |

### /user/login

#### GET
##### Summary

Logs user into the system

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| username | query | The user name for login | No | string |
| password | query | The password for login in clear text | No | string |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | string |
| 400 | Invalid username/password supplied |  |

### /user/logout

#### GET
##### Summary

Logs out current logged in user session

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |

##### Responses

| Code | Description |
| ---- | ----------- |
| default | successful operation |

### /user/{username}

#### GET
##### Summary

Get user by user name

##### Description

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| username | path | The name that needs to be fetched. Use user1 for testing.  | Yes | string |

##### Responses

| Code | Description | Schema |
| ---- | ----------- | ------ |
| 200 | successful operation | [User](#user) |
| 400 | Invalid username supplied |  |
| 404 | User not found |  |

#### PUT
##### Summary

Updated user

##### Description

This can only be done by the logged in user.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| username | path | name that need to be deleted | Yes | string |
| body | body | Updated user object | No | [User](#user) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Invalid user supplied |
| 404 | User not found |

#### DELETE
##### Summary

Delete user

##### Description

This can only be done by the logged in user.

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ------ |
| username | path | The name that needs to be deleted | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Invalid username supplied |
| 404 | User not found |

### Models

#### Order

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| id | long |  | No |
| petId | long |  | No |
| quantity | integer |  | No |
| shipDate | dateTime |  | No |
| status | string | Order Status<br>*Enum:* `"placed"`, `"approved"`, `"delivered"` | No |
| complete | boolean |  | No |

#### Category

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| id | long |  | No |
| name | string |  | No |

#### User

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| id | long |  | No |
| username | string |  | No |
| firstName | string |  | No |
| lastName | string |  | No |
| email | string |  | No |
| password | string |  | No |
| phone | string |  | No |
| userStatus | integer | User Status | No |

#### Tag

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| id | long |  | No |
| name | string |  | No |

#### Pet

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| id | long |  | No |
| category | [Category](#category) |  | No |
| name | string | *Example:* `"doggie"` | Yes |
| photoUrls | [ string ] |  | Yes |
| tags | [ [Tag](#tag) ] |  | No |
| status | string | pet status in the store<br>*Enum:* `"available"`, `"pending"`, `"sold"` | No |

#### ApiResponse

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| code | integer |  | No |
| type | string |  | No |
| message | string |  | No |

[My PDF Document](MyCreds.PDF)