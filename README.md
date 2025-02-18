# SimplyFI Hyperledger Task
## ABAC-Based Asset Management System

## Overview
This project is a Hyperledger Fabric blockchain application for managing assets securely. It includes functionalities for creating, reading, updating, and deleting assets, with role-based access control (RBAC) ensuring that only authorized users can perform specific actions.

## Features
- Admin: Can create, update, and delete assets.
- User: Can read assets they own.
- Auditor: Can view all assets.
- Chaincode: Implements business logic for asset transactions.
- Blockchain Network: Built on Hyperledger Fabric.

## Prerequisites

- Node.js (v16+ recommended)
- npm
- Docker & Docker Compose
- Hyperledger Fabric (v2.2 or later)
- Fabric Samples & CLI Tools

## Setup & Installation
1. Clone the Repository

```
git clone https://github.com/Sneha-p1/SimplyFI_Task_Hyperledger
cd SimplyFI_Task_Hyperledger
```
2. Install Dependencies
```
npm install
```
3. Start the Hyperledger Fabric Network
```
cd Network/
./startNetwork.sh
```
4. Run the Client Application
```
cd Client/
node index.js
```

### Create an Asset
```
node CreateAsset.js
```

### Read an Asset
```
node ReadAsset.js
```

### Update an Asset
```
node UpdateAsset.js
```
### Delete an Asset
```
node DeleteAsset.js
```

### Get All Assets (Auditor Only)
```
node GetAllAssets.js
```

