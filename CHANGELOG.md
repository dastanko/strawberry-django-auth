CHANGELOG
=========

0.375.0 - 2023-07-10
--------------------

This release updates to the latest version of strawberry
and removes dependencies with strawberry-django-plus.

- The directive `IsVerified` is migrated to the new field
extensions API and extends the django base permission
extension.

- The Channels middleware will inject the user in `request.user`
or `request.scope["UserOrError"]`

Contributed by [ניר](https://github.com/nrbnlulu) via [PR #403](https://github.com/nrbnlulu/strawberry-django-auth/pull/403/)


0.374.6 - 2023-05-29
--------------------

This release fixes the way we call django's `send_mail()` previously
we were passing the `DjangoSetting` object directly, but now we pass its value.

fixes #387

Contributed by [ניר](https://github.com/nrbnlulu) via [PR #391](https://github.com/nrbnlulu/strawberry-django-auth/pull/391/)


0.374.5 - 2023-05-16
--------------------

Dependencies update

0.374.4 - 2023-05-07
--------------------

This is a dependencies update release.

If you use captcha validation you will need to

Contributed by [ניר](https://github.com/nrbnlulu) via [PR #377](https://github.com/nrbnlulu/strawberry-django-auth/pull/377/)


0.374.3 - 2023-04-06
--------------------

Correctly pluralizes the "UserStatus" model as "User statuses" in Django Admin.

Without this change, Django Admin automatically uses the string "User statuses" as the verbose plural name.

Achieved by overriding the `Meta` (Django model subclass) attribute `verbose_name_plural`.

Contributed by [Justin Masayda](https://github.com/keysmusician) via [PR #368](https://github.com/nrbnlulu/strawberry-django-auth/pull/368/)


0.374.2 - 2023-03-25
--------------------

This release fixes release bot.

Contributed by [ניר](https://github.com/nrbnlulu) via [PR #355](https://github.com/nrbnlulu/strawberry-django-auth/pull/355/)


0.374.1 - 2023-03-24
--------------------

This release just updates dependencies.

Contributed by [ניר](https://github.com/nrbnlulu) via [PR #354](https://github.com/nrbnlulu/strawberry-django-auth/pull/354/)
