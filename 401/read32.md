# Permissions

- Permission checks are always run at the very start of the view, before any other code is allowed to proceed.
- Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

- Permissions are used to grant or deny access for different classes of users to different parts of the API.

- The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user.

- A slightly less strict style of permission would be to allow full access to authenticated users, but allow read-only access to unauthenticated users. 

## How permissions are determined ?

- Permissions in REST framework are always defined as a list of permission classes.

- Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

- When the permissions checks fail either a “403 Forbidden” or a “401 Unauthorized” response will be returned, according to the following rules:

    - The request was successfully authenticated, but permission was denied.    
       - An HTTP 403 Forbidden response will be returned.
    - The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers.
      - An HTTP 403 Forbidden response will be returned.
    - The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers
      - An HTTP 401 Unauthorized response
      
## set permisiion
by type in setting.py

        REST_FRAMEWORK = {
            'DEFAULT_PERMISSION_CLASSES': [
                'rest_framework.permissions.IsAuthenticated',
            ]
        }

You can also set the authentication policy on a per-view, or per-viewset basis, using the `APIView` class-based views.
## API Reference

- `AllowAny` The AllowAny permission class will allow unrestricted access.

- `IsAuthenticated` the IsAuthenticated class will deny permission to any unauthenticated user, and allow permission otherwise.

- `IsAdminUser` The IsAdminUser permission class will deny permission to any user, unless user.is_staff is true 

- `IsAuthenticatedOrReadOnly` The IsAuthenticatedOrReadOnly will allow authenticated users to perform any - - request. Requests for unauthorised users will only be permitted if the request method is one of the “safe” methods; GET, HEAD or OPTIONS.

## Django Model Permissions 

- This permission class ties into Django’s standard django.contrib.auth model permissions.

- This permission must only be applied to views that have a .queryset property or get_queryset() method.

- **POST**: requests require the user to have the add permission on the model.

- **PUT**: requests require the user to have the change permission on the model.

- **DELETE**: requests require the user to have the delete permission on the model

## some Third party packages:
1. [DRF - Access Policy](https://github.com/rsinger86/drf-access-policy)
2. [Composed Permissions](https://github.com/niwibe/djangorestframework-composed-permissions)
3. [REST Condition](https://github.com/caxap/rest_condition)
4. [DRY Rest Permissions](https://github.com/FJNR-inc/dry-rest-permissions)
5. [Django Rest Framework Roles](https://github.com/computer-lab/django-rest-framework-roles)
6. [Django REST Framework API Key](https://florimondmanca.github.io/djangorestframework-api-key/)
7. [Django Rest Framework Role Filters](https://github.com/allisson/django-rest-framework-role-filters)
8. [Django Rest Framework PSQ](https://github.com/drf-psq/drf-psq)


***resources**

[permissions](https://www.django-rest-framework.org/api-guide/permissions/)
