sentry-quotas
===============

An extension for Sentry which allows setting hard limits.

Install
-------

Install the package via ``pip``::

    pip install sentry-quotas


Configure ``SENTRY_QUOTAS`` in your ``sentry.conf.py``::

    SENTRY_QUOTAS = {
        'redis': {
            'hosts' = {
                # for more information on configuration hosts, see the documentation for the
                # Nydus python package
                0: {
                    'host': 'localhost',
                    'port': 6379
                }
            }
        }
        'default_events_per_minute': 100,
    }
