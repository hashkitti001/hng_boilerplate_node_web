# HNG BACKEND TASK 3 - NodeJS Boilerplate [Argo Team]
This is a sample Node js boilerplate Server based on the OpenAPI 3.0 specification.  

### Contributors (Slack Usernames)
@reneiii
@Lanfear
@Japheth Paul
@Romauld
@Hudhayfah

Some useful links:
- [The Argo team repository](https://github.com/hashkitti001/hng_boilerplate_node_web)

- [The Entity relationship diagram](httpS://)

## Version: 1.0.11

### Terms of service
http://swagger.io/terms/

**Contact information:**  
apiteam@swagger.io  

**License:** [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

[Find out more about Swagger](http://swagger.io)
### /auth/register

#### POST
##### Summary:

Register a new user

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | User registered successfully |
| 400 | Bad request |
| 409 | Conflict - User already exists |
| 500 | Internal server error |

### /auth/login

#### POST
##### Summary:

Login a user

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User logged in successfully |
| 400 | Bad request |
| 401 | Unauthorized |
| 500 | Internal server error |

### /auth/social

#### POST
##### Summary:

Social authentication

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User authenticated successfully |
| 400 | Bad request |
| 401 | Unauthorized |
| 500 | Internal server error |

### /auth/magic-link

#### POST
##### Summary:

Send magic link for authentication

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Magic link sent successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /auth/magic-link/verify

#### POST
##### Summary:

Verify magic link

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Magic link verified successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /auth/change-password

#### POST
##### Summary:

Change user password

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Password changed successfully |
| 400 | Bad request |
| 401 | Unauthorized |
| 500 | Internal server error |

### /auth/get-otp

#### POST
##### Summary:

Get OTP for authentication

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OTP sent successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /email/send

#### POST
##### Summary:

Send an email

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Email sent successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /email/templates

#### GET
##### Summary:

Get all email templates

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | List of email templates |
| 500 | Internal server error |

#### POST
##### Summary:

Create a new email template

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Email template created successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /email/templates/{id}

#### GET
##### Summary:

Get an email template by ID

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | ID of the email template | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Email template details |
| 404 | Template not found |
| 500 | Internal server error |

#### PUT
##### Summary:

Update an email template

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | ID of the email template | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Email template updated successfully |
| 400 | Bad request |
| 404 | Template not found |
| 500 | Internal server error |

#### DELETE
##### Summary:

Delete an email template

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | ID of the email template | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Email template deleted successfully |
| 404 | Template not found |
| 500 | Internal server error |

### /payments/stripe/create-payment-intent

#### POST
##### Summary:

Create Stripe payment intent

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Payment intent created successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /payments/internal/create

#### POST
##### Summary:

Create an internal payment record

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Payment record created successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /notifications/send

#### POST
##### Summary:

Send a notification

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Notification sent successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /blog/posts

#### GET
##### Summary:

Get all blog posts

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | List of blog posts |
| 500 | Internal server error |

#### POST
##### Summary:

Create a new blog post

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Blog post created successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /blog/posts/{id}

#### GET
##### Summary:

Get a blog post by ID

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Blog post details |
| 404 | Blog post not found |
| 500 | Internal server error |

#### PUT
##### Summary:

Update a blog post by ID

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Blog post updated successfully |
| 400 | Bad request |
| 404 | Blog post not found |
| 500 | Internal server error |

#### DELETE
##### Summary:

Delete a blog post by ID

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Blog post deleted successfully |
| 404 | Blog post not found |
| 500 | Internal server error |

### /invite/send

#### POST
##### Summary:

Send an invite link

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Invite link sent successfully |
| 400 | Bad request |
| 500 | Internal server error |

### /users/profile

#### GET
##### Summary:

Get users profile

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Users data |
| 500 | Internal server error |

#### PATCH
##### Summary:

Update user profile

##### Responses

| Code | Description |
| ---- | ----------- |
| 204 | Profile updated successfully |
| 422 | Validation error |
| 500 | Internal server error |

#### Link to Image Preview
![Alt text](https://imgur.com/a/wjPg3Gl)



