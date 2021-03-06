..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _ceilometer-events:

.. list-table:: Description of events configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[event]**
     -
   * - ``definitions_cfg_file`` = ``event_definitions.yaml``
     - (String) Configuration file for event definitions.
   * - ``drop_unmatched_notifications`` = ``False``
     - (Boolean) Drop notifications if no event definition matches. (Otherwise, we convert them with just the default traits)
   * - ``store_raw`` = ``[]``
     - (Multi-valued) Store the raw notification for select priority levels (info and/or error). By default, raw details are not captured.
   * - **[notification]**
     -
   * - ``ack_on_event_error`` = ``True``
     - (Boolean) Acknowledge message when event persistence fails.
   * - ``workers`` = ``1``
     - (Integer) Number of workers for notification service, default value is 1.
   * - ``workload_partitioning`` = ``False``
     - (Boolean) Enable workload partitioning, allowing multiple notification agents to be run simultaneously.
