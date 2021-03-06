## `epiviz-workspace` element

This uses firebase to setup authentication (firebase-auth) and polyfire elements to save and retrieve user and workspace data.

## Installation

Please install `bower` and `polymer`

```
    bower install epiviz/epiviz-workshop

```

To reuse this repository, clone the repository and install the dependencies.

```
    git clone http://github.com/epiviz/epiviz-workspace
    cd epiviz-workspace
    bower install
```

## Firebase configuration
To setup, Please open a firebase account and use the firebase configuration to setup epiviz-workspace

```
    auth-domain="{{authDomain}}"
    database-url="{{databaseUrl}}"
    api-key="{{apiKey}}"
    storage-bucket="{{storageBucket}}"
    messaging-sender-id="{{messagingSenderId}}"
```

## Database Structure

the firebase database linked to this project creates two documents

### `users`

The users document contains the oauth-id and all the workspace id's linked to a user.

### `workspaces`

Similarly the workspaces document contains all the workspace id's and its content.