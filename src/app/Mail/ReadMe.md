# The `Mail` Directory
The `app/Mail` directory contains classes that send emails for Tranzakt.
It is anticipated that these will most likely be generated by Tranzakt user apps.

Mail classes can be created using the `make:mail` Artisan command.

Mail objects allow you to encapsulate all of the logic of building an email
in a single, simple class that may be sent using the `Mail::send` method.
