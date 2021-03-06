..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _murano-api:

.. list-table:: Description of API configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[DEFAULT]**
     -
   * - ``admin_role`` = ``admin``
     - (String) Role used to identify an authenticated user as administrator.
   * - ``max_header_line`` = ``16384``
     - (Integer) Maximum line size of message headers to be accepted. max_header_line may need to be increased when using large tokens (typically those generated by the Keystone v3 API with big service catalogs).
   * - ``secure_proxy_ssl_header`` = ``X-Forwarded-Proto``
     - (String) The HTTP Header that will be used to determine which the original request protocol scheme was, even if it was removed by an SSL terminator proxy.
   * - **[oslo_middleware]**
     -
   * - ``enable_proxy_headers_parsing`` = ``False``
     - (Boolean) Whether the application is behind a proxy or not. This determines if the middleware should parse the headers or not.
   * - ``max_request_body_size`` = ``114688``
     - (Integer) The maximum body size for each request, in bytes.
   * - ``secure_proxy_ssl_header`` = ``X-Forwarded-Proto``
     - (String) DEPRECATED: The HTTP Header that will be used to determine what the original request protocol scheme was, even if it was hidden by a SSL termination proxy.
   * - **[oslo_policy]**
     -
   * - ``policy_default_rule`` = ``default``
     - (String) Default rule. Enforced when a requested rule is not found.
   * - ``policy_dirs`` = ``['policy.d']``
     - (Multi-valued) Directories where policy configuration files are stored. They can be relative to any directory in the search path defined by the config_dir option, or absolute paths. The file defined by policy_file must exist for these directories to be searched. Missing or empty directories are ignored.
   * - ``policy_file`` = ``policy.json``
     - (String) The file that defines policies.
   * - **[paste_deploy]**
     -
   * - ``config_file`` = ``None``
     - (String) Path to Paste config file
   * - ``flavor`` = ``None``
     - (String) Paste flavor
