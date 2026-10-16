# How do I run an incremental reindex of a data source?

Open the actions menu of the data source and select **Incremental Index**. Only content that was added, changed or removed since the last successful run is processed, which is faster and cheaper than a **Full Reindex**.

Incremental indexing is supported for Git (code and FAQ), SVN, Confluence, Jira, X-ray, Azure DevOps (Work Items and Wiki), SharePoint, Google Docs and xWiki. File data sources are not incremental.

**Incremental Index** is disabled after a failed run, or when the query, space, site, filter, repository or branch was changed. In these cases, run a **Full Reindex** first.

For scheduled reindexing, enable **Run scheduled reindex incrementally** next to the schedule. It is off by default, so scheduled runs are full; Jira and X-ray scheduled runs are always incremental.

## Sources

- [Indexing Data Sources](https://docs.codemie.ai/user-guide/data-source/data-source-overview/indexing-data-sources)
