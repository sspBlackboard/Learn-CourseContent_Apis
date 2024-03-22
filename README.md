# Learn-Placements_Apis

## Description

This project involves using Postman to obtain the access token required to authenticate the API requests for retrieving placements and a specific placement.

## Installation

### Postman

Postman is a collaboration platform for API development. It simplifies each step of building an API and streamlines collaboration, enabling you to create better APIs faster.

To install Postman, follow these steps:

1. Visit the [Postman website](https://www.postman.com/downloads/).
2. Download the version suitable for your platform.
3. Run the installer.

## API List

The `Api_Export.json` file contains the following APIs:

- `GET /learn/api/public/v1/lti/placements`: Returns a list of LTI placements.
- `POST /learn/api/public/v1/lti/placements`: Creates an LTI placement.
- `GET /learn/api/public/v1/lti/placements/{placementId}`: Returns the LTI placement with the specified Id.
- `DELETE /learn/api/public/v1/lti/placements/{placementId}`: Deletes an LTI placement with the specified Id.
- `PATCH /learn/api/public/v1/lti/placements/{placementId}`: Updates an LTI placement with the given Id.

## Usage

After importing the `Api_Export.json` file into Postman, you can use the APIs by sending requests to them. Ensure to set up the environment variables correctly:

- `$LEARN_DOMAIN`: Learn Server FQDN
- `$APP_KEY`: Your application key here
- `$APP_SECRET`: Your application secret here
- `$ACCESSTOKEN`: Obtain the access token from the API request '/learn/api/public/v1/oauth2/token' using the above values and replace the variable
- `$PLACEMENT_ID_GET`: Id of the placement to be searched
- `$PLACEMENT_ID_DEL`: Id of the placement to be deleted
