New, updated, and deprecated options in Newton for Identity service
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

..
  Warning: Do not edit this file. It is automatically generated and your
  changes will be overwritten. The tool to do so lives in the
  openstack-doc-tools repository.


.. list-table:: New options
   :header-rows: 1
   :class: config-ref-table

   * - Option = default value
     - (Type) Help string
   * - ``[security_compliance] disable_user_account_days_inactive =``
     - (IntOpt) The maximum number of days a user can go without authenticating before being considered "inactive" and automatically disabled (locked).
   * - ``[security_compliance] lockout_failure_attempts =``
     - (IntOpt) The maximum number of times that a user can fail to authenticate before the user account is locked.
   * - ``[security_compliance] lockout_duration = 1800``
     - (IntOpt) The number of seconds a user account will be locked when the maximum number of failed authentication attempts is exceeded.
   * - ``[security_compliance] password_expires_days = <None>``
     - (IntOpt) The number of days for which a password will be considered valid before requiring it to be changed.
   * - ``[security_compliance] password_expires_ignore_user_ids =``
     - (StrOpt) User IDs to be ignored when checking if a password is expired.
   * - ``[security_compliance] unique_last_password_count = 1``
     - (IntOpt) Controls the number of previous user password iterations to keep in history, in order to enforce that newly created passwords are unique.
   * - ``[security_compliance] minimum_password_age = 0``
     - (IntOpt）The number of days that a password must be used before the user can change it.
   * - ``[security_compliance] password_regex = <None>``
     - (StrOpt) Validate password strength requirements.
   * - ``[security_compliance] password_regex_description = <None>``
     - (StrOpt) Humans language to describe password regular expression.
   * - ``[token] cache_on_issue = false``
     - (BoolOpt) Enable storing issued token data to token validation cache so that first token validation doesn't actually cause full validation cycle.


.. list-table:: Deprecated options
   :header-rows: 1
   :class: config-ref-table

   * - Deprecated option
     - New Option
   * - ``[DEFAULT] use_syslog``
     - ``None``
   * - ``[endpoint_policy] enabled``
     - ``None``
   * - ``[token] hash_algorithm``
     - ``None``
   * - ``[os_inherit]``
     - ``None``

