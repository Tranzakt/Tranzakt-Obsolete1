# The `Storage` Directory
The Laravel storage directory contains:
* logs
* compiled Blade templates
* file based sessions
* file caches
* other files generated by the framework.

This Laravel directory is usually segregated into `app`, `framework`, and `logs` sub-directories.

The `app` sub-directory may be used to store any files generated by your application.

The `framework` directory is used to store framework generated files and caches.

Finally, the `logs` directory contains your application's log files.

For Tranzakt Runtime, `storage` will be used for most of the above rather than `core/storage`,
however logs detailing Tranzakt Runtime internal issues will be stored here,
whilst logs detailing Runtime issues with the Tranzakt developed app will be stored in `storage`

A `storage/app/public` directory is also recommended by standard Laravel
to store user-generated files (such as profile avatars) that should be publicly accessible,
with a symbolic link at `public/storage` which points to this directory.
However this is **not** recommended for Tranzakt,
and instead such files should be stored directly in a sub-directory of `public`.
