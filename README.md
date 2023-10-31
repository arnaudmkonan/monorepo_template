# monorepo_template

## This monorepo is organized into three main directories:

*Backend*: This directory contains the Python-FastAPI code for the backend API.
*Database*: This directory contains the PostgreSQL database schema and Dockerfile.
*Frontend*: This directory contains the Flutter code for the frontend web app and mobile app.
The `tests/` directory contains unit tests for the backend and frontend code.

The ```WORKSPACE``` file is a Bazel build file that defines the monorepo and its dependencies.

To build the backend API, you can run the following command:

```$bazel build backend:api```   
This will create an executable file called api in the ```backend/``` directory.

To start the backend API, you can run the following command:

```./backend/api```   
To build the frontend web app, you can run the following command:

```bazel build frontend:web```   
This will create a web app bundle in the `frontend/build/web/` directory.

To serve the frontend web app, you can run the following command:

```python -m SimpleHTTPServer 8000```   
This will start a web server on port 8000.

To build the frontend mobile app, you can run the following command:

bazel build frontend:mobile
This will create an Android app bundle (AAB) in the frontend/build/app/ directory.

To install the frontend mobile app on an Android device, you can use the following command:

```adb install frontend/build/app/app.aab```   
Once the mobile app is installed, you can launch it from the app drawer.

This is just a minimal example of a monorepo for a shopping list platform. You can add more features and functionality to your monorepo as needed.

```
└── shopping_list
    ├── backend
    │   └── python_fastapi
    │       ├── models.py
    │       ├── routers
    │       │   └── items.py
    │       └── __main__.py
    ├── database
    │   └── postgres
    │       ├── schema.sql
    │       └── Dockerfile
    ├── frontend
    │   └── flutter
    │       ├── lib
    │       │   ├── main.dart
    │       │   ├── models
    │       │   │   ├── item.dart
    │       │   │   └── user.dart
    │       │   ├── screens
    │       │   │   ├── items_list.dart
    │       │   │   └── login_screen.dart
    │       │   └── services
    │       │       └── api_service.dart
    └── tests
        ├── backend
        │   └── test_items.py
        │   └── test_users.py
        └── frontend
            └── test_items_list.dart
            └── test_login_screen.dart
```
