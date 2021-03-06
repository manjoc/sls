# How do I configure an index for a historical log? {#concept_pc5_kzb_kgb .concept}

Log Service cannot configure indexes for historical logs directly. However, you can rewrite the logs into a new Logstore through DataWorks or use CLI commands to configure indexes as needed.

Indexes are valid only for the logs that are collected after index configuration, and historical logs cannot be queried or analyzed. If you want to configure indexes for historical logs, use either of the following methods:

-   **Rewrite data into a new Logstore through DataWorks and then configure indexes**.

    After configuring an index for the new Logstore, use DataWorks to export historical logs from the old Logstore and then import them to the new Logstore. By dong so, you can query and analyze historical logs.

-   **Rewrite data into the Logstore through CLI commands and then configure indexes**.

    Use a command-line tool to rewrite logs into the Logstore to configure indexes.

    For more information, see [Aliyun Log Service CLI](https://aliyun-log-cli.readthedocs.io/en/latest/README.html).


**Note:** Both the methods achieve index configuration through data duplication and import, which does not change or delete existing historical logs.

