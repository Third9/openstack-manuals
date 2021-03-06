..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _nova-conductor:

.. list-table:: Description of conductor configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[DEFAULT]**
     -
   * - ``migrate_max_retries`` = ``-1``
     - (Integer) Number of times to retry live-migration before failing.

       Possible values:

       * If == -1, try until out of hosts (default)

       * If == 0, only try once, no retries

       * Integer greater than 0
   * - **[conductor]**
     -
   * - ``manager`` = ``nova.conductor.manager.ConductorManager``
     - (String) DEPRECATED: Full class name for the Manager for conductor.

       Removal in 14.0
   * - ``topic`` = ``conductor``
     - (String) Topic exchange name on which conductor nodes listen.
   * - ``use_local`` = ``False``
     - (Boolean) DEPRECATED: Perform nova-conductor operations locally. This legacy mode was introduced to bridge a gap during the transition to the conductor service. It no longer represents a reasonable alternative for deployers.

       Removal may be as early as 14.0.
   * - ``workers`` = ``None``
     - (Integer) Number of workers for OpenStack Conductor service. The default will be the number of CPUs available.
