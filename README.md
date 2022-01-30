node-red-contrib-swagger-petstore
================

Node-RED node for swagger-petstore

This is a sample server Petstore server.  You can find out more about Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).  For this sample, you can use the api key `special-key` to test the authorization filters.

## Install

To install the stable version use the `Menu - Manage palette - Install` 
option and search for node-red-contrib-swagger-petstore, or run the following 
command in your Node-RED user directory, typically `~/.node-red`

    npm install node-red-contrib-swagger-petstore

## Usage

### Methods

#### POST /pet/{petId}/uploadImage

uploads an image

    petId : integer
    additionalMetadata : string
    file : file
     
    Accept : 'application/json'
    Content-Type : 'multipart/form-data'

#### POST /pet

Add a new pet to the store

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### PUT /pet

Update an existing pet

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### GET /pet/findByStatus

Multiple status values can be provided with comma separated strings

    status : array
     
    Accept : 'application/json'

#### GET /pet/findByTags

Multiple tags can be provided with comma separated strings. Use tag1, tag2, tag3 for testing.

    tags : array
     
    Accept : 'application/json'

#### GET /pet/{petId}

Returns a single pet

    petId : integer
     
    Accept : 'application/json'

#### POST /pet/{petId}

Updates a pet in the store with form data

    petId : integer
    name : string
    status : string
     
    Accept : 'application/json'

#### DELETE /pet/{petId}

Deletes a pet

    api_key : string
    petId : integer
     
    Accept : 'application/json'

#### POST /store/order

Place an order for a pet

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### GET /store/order/{orderId}

For valid response try integer IDs with value >= 1 and <= 10. Other values will generated exceptions

    orderId : integer
     
    Accept : 'application/json'

#### DELETE /store/order/{orderId}

For valid response try integer IDs with positive integer value. Negative or non-integer values will generate API errors

    orderId : integer
     
    Accept : 'application/json'

#### GET /store/inventory

Returns a map of status codes to quantities

     
    Accept : 'application/json'

#### POST /user/createWithArray

Creates list of users with given input array

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### POST /user/createWithList

Creates list of users with given input array

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### GET /user/{username}

Get user by user name

    username : string
     
    Accept : 'application/json'

#### PUT /user/{username}

This can only be done by the logged in user.

    username : string
    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'

#### DELETE /user/{username}

This can only be done by the logged in user.

    username : string
     
    Accept : 'application/json'

#### GET /user/login

Logs user into the system

    username : string
    password : string
     
    Accept : 'application/json'

#### GET /user/logout

Logs out current logged in user session

     
    Accept : 'application/json'

#### POST /user

This can only be done by the logged in user.

    body : 
     
    Accept : 'application/json'
    Content-Type : 'application/json'


## License

#### Apache 2.0

http://www.apache.org/licenses/LICENSE-2.0.html