---
layout: default
---

# Summary

* [Introduction](index.html)
* [Highlights](highlights.html)

## GETTING FAMILIAR

* [Getting Started](getting-started-readme.html)
  * [Installation](getting-started-installation.html)
  * [Authentication](getting-started-authentication.html)
  * [Web Interface](getting-started-web-interface.html)
  * [Databases, Collections and Documents](getting-started-databases-collections-documents.html)
  * [Querying the Database](getting-started-querying-the-database.html)
  * [Coming from SQL](getting-started-coming-from-sql.html)
  * [Next Steps](getting-started-next-steps.html)
* [Tutorials](tutorials-readme.html)
  <!-- SYNC: https://@github.com/arangodb-helper/arangodb.git;arangodb;docs/Manual;;/ -->
  * [ArangoDB Starter](tutorials-starter-readme.html)
  <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
  * [Datacenter to datacenter Replication](tutorials-dc2dc-readme.html)
  <!-- SYNC: https://@github.com/arangodb/kube-arangodb.git;kube-arangodb;docs/Manual;;/ -->
  * [Kubernetes](tutorials-kubernetes-readme.html)
    * [Amazon EKS](tutorials-kubernetes-e-k-s.html)
    * [Google GKE](tutorials-kubernetes-g-k-e.html)
    * [Azure AKS](tutorials-kubernetes-a-k-s.html)
  * [DC2DC on Kubernetes](tutorials-kubernetes-dc2dc.html)
* [Programs & Tools](programs-readme.html)
  * [ArangoDB Server](programs-arangod-readme.html)
    * [Options](programs-arangod-options.html)
      * [Global](programs-arangod-global.html)
      * [Agency](programs-arangod-agency.html)
      * [ArangoSearch](programs-arangod-arangosearch.html)
      * [Audit](programs-arangod-audit.html)
      * [Cache](programs-arangod-cache.html)
      * [Cluster](programs-arangod-cluster.html)
      * [Compaction](programs-arangod-compaction.html)
      * [Database](programs-arangod-database.html)
      * [Foxx](programs-arangod-foxx.html)
      * [Frontend](programs-arangod-frontend.html)
      * [HTTP](programs-arangod-http.html)
      * [JavaScript](programs-arangod-javascript.html)
      * [LDAP](programs-arangod-ldap.html)
      * [Log](programs-arangod-log.html)
      * [Nonce](programs-arangod-nonce.html)
      * [Query](programs-arangod-query.html)
      * [Random](programs-arangod-random.html)
      * [Replication](programs-arangod-replication.html)
      * [RocksDB](programs-arangod-rocksdb.html)
      * [Server](programs-arangod-server.html)
      * [SSL](programs-arangod-ssl.html)
      * [TCP](programs-arangod-tcp.html)
      * [Temp](programs-arangod-temp.html)
      * [VST](programs-arangod-vst.html)
      * [WAL](programs-arangod-wal.html)
  * [Web Interface](programs-web-interface-readme.html)
    * [Dashboard](programs-web-interface-dashboard.html)
    * [Cluster](programs-web-interface-cluster.html)
    * [Collections](programs-web-interface-collections.html)
    * [Document](programs-web-interface-document.html)
    * [Queries](programs-web-interface-aql-editor.html)
    * [Graphs](programs-web-interface-graphs.html)
    * [Services](programs-web-interface-services.html)
    * [Users](programs-web-interface-users.html)
    * [Logs](programs-web-interface-logs.html)
  * [ArangoDB Shell](programs-arangosh-readme.html)
    * [Examples](programs-arangosh-examples.html)
    * [Details](programs-arangosh-details.html)
    * [Options](programs-arangosh-options.html)
  <!-- SYNC: https://@github.com/arangodb-helper/arangodb.git;arangodb;docs/Manual;;/ -->
  * [ArangoDB Starter](programs-starter-readme.html)
    * [Options](programs-starter-options.html)
    * [Security](programs-starter-security.html)
    * [Architecture](programs-starter-architecture.html)
  * [Arangodump](programs-arangodump-readme.html)
    * [Examples](programs-arangodump-examples.html)
    * [Options](programs-arangodump-options.html)
    * [Maskings](programs-arangodump-maskings.html)
    * [Limitations](programs-arangodump-limitations.html)
  * [Arangorestore](programs-arangorestore-readme.html)
    * [Examples](programs-arangorestore-examples.html)
    * [Fast Cluster Restore](programs-arangorestore-fast-cluster-restore.html)
    * [Options](programs-arangorestore-options.html)
  * [Arangoimport](programs-arangoimport-readme.html)
    * [Examples JSON](programs-arangoimport-examples-json.html)
    * [Examples CSV](programs-arangoimport-examples-csv.html)
    * [Details](programs-arangoimport-details.html)
    * [Options](programs-arangoimport-options.html)
  * [Arangoexport](programs-arangoexport-readme.html)
    * [Examples](programs-arangoexport-examples.html)
    * [Options](programs-arangoexport-options.html)
  * [Arangobench](programs-arangobench-readme.html)
    * [Examples](programs-arangobench-examples.html)
    * [Options](programs-arangobench-options.html)
  * [Arangoinspect](programs-arangoinspect-readme.html)
    * [Examples](programs-arangoinspect-examples.html)
    * [Options](programs-arangoinspect-options.html)
  * [Datafile Debugger](programs-arango-dfdb-readme.html)
    * [Examples](programs-arango-dfdb-examples.html)
  <!-- SYNC: https://@github.com/arangodb/foxx-cli.git;foxx-cli;docs/Manual;;/ -->
  * [Foxx CLI](programs-foxx-cli-readme.html)
    * [Details](programs-foxx-cli-details.html)

## CORE TOPICS

* [Data models & modeling](data-modeling-readme.html)
  * [Concepts](data-modeling-concepts.html)
  * [Databases](data-modeling-databases-readme.html)
    * [Working with Databases](data-modeling-databases-working-with.html)
    * [Notes about Databases](data-modeling-databases-notes.html)
  * [Collections](data-modeling-collections-readme.html)
    * [Collection Methods](data-modeling-collections-collection-methods.html)
    * [Database Methods](data-modeling-collections-database-methods.html)
  * [Documents](data-modeling-documents-readme.html)
    * [Basics and Terminology](data-modeling-documents-document-address.html)
    * [Collection Methods](data-modeling-documents-document-methods.html)
    * [Database Methods](data-modeling-documents-database-methods.html)
  * [Graphs, Vertices & Edges](data-modeling-graphs-vertices-edges.html)
  * [Views](data-modeling-views-readme.html)
    * [Database Methods](data-modeling-views-database-methods.html)
    * [View Methods](data-modeling-views-view-methods.html)
  * [Naming Conventions](data-modeling-naming-conventions-readme.html)
    * [Database Names](data-modeling-naming-conventions-database-names.html)
    * [Collection and View Names](data-modeling-naming-conventions-collection-and-view-names.html)
    * [Document Keys](data-modeling-naming-conventions-document-keys.html)
    * [Attribute Names](data-modeling-naming-conventions-attribute-names.html)
  * [Operational Factors](data-modeling-operational-factors.html)
* [Indexing](indexing-readme.html)
  * [Index Basics](indexing-index-basics.html)
  * [Which index to use when](indexing-which-index.html)
  * [Index Utilization](indexing-index-utilization.html)
  * [Working with Indexes](indexing-working-with-indexes.html)
    * [Hash Indexes](indexing-hash.html)
    * [Skiplists](indexing-skiplist.html)
    * [Persistent](indexing-persistent.html)
    * [Fulltext Indexes](indexing-fulltext.html)
    * [Geo-spatial Indexes](indexing-geo.html)
    * [Vertex Centric Indexes](indexing-vertex-centric.html)
* [Transactions](transactions-readme.html)
  * [Transaction invocation](transactions-transaction-invocation.html)
  * [Passing parameters](transactions-passing.html)
  * [Locking and isolation](transactions-locking-and-isolation.html)
  * [Durability](transactions-durability.html)
  * [Limitations](transactions-limitations.html)
* [Graphs](graphs-readme.html)
  * [General Graphs](graphs-general-graphs-readme.html)
    * [Graph Management](graphs-general-graphs-management.html)
    * [Graph Functions](graphs-general-graphs-functions.html)
  * [SmartGraphs](graphs-smart-graphs-readme.html)
    * [SmartGraph Management](graphs-smart-graphs-management.html)
  * [Traversals](graphs-traversals-readme.html)
    * [Using Traversal Objects](graphs-traversals-using-traversal-objects.html)
    * [Example Data](graphs-traversals-example-data.html)
  * [Working with Edges](graphs-edges-readme.html)
  * [Pregel](graphs-pregel-readme.html)
* [ArangoSearch Views](views-arango-search-readme.html)
  * [Getting Started](views-arango-search-getting-started.html)
  * [Detailed Overview](views-arango-search-detailed-overview.html)
  * [Analyzers](views-arango-search-analyzers.html)
  * [Scorers](views-arango-search-scorers.html)

## ADVANCED TOPICS

* [Architecture](architecture-readme.html)
  * [ArangoDB Deployment Modes](architecture-deployment-modes-readme.html)
    * [Single Instance](architecture-deployment-modes-single-instance-readme.html)
    * [Master/Slave](architecture-deployment-modes-master-slave-readme.html)
      * [Architecture](architecture-deployment-modes-master-slave-architecture.html)
      * [Limitations](architecture-deployment-modes-master-slave-limitations.html)
    * [Active Failover](architecture-deployment-modes-active-failover-readme.html)
      * [Architecture](architecture-deployment-modes-active-failover-architecture.html)
      * [Limitations](architecture-deployment-modes-active-failover-limitations.html)
    * [Cluster](architecture-deployment-modes-cluster-readme.html)
      * [Architecture](architecture-deployment-modes-cluster-architecture.html)
      * [Data models](architecture-deployment-modes-cluster-data-models.html)
      * [Limitations](architecture-deployment-modes-cluster-limitations.html)
    <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
    * [Datacenter to datacenter replication](architecture-deployment-modes-dc2dc-readme.html)
      * [Introduction](architecture-deployment-modes-dc2dc-introduction.html)
      * [Applicability](architecture-deployment-modes-dc2dc-applicability.html)
      * [Requirements](architecture-deployment-modes-dc2dc-requirements.html)
      * [Limitations](architecture-deployment-modes-dc2dc-limitations.html)
  * [Single Instance vs. Cluster](architecture-single-instance-vs-cluster.html)
  * [Storage Engines](architecture-storage-engines.html)
  * [Replication](architecture-replication-readme.html)
  * [Write-ahead log](architecture-write-ahead-log.html)
* [Foxx Microservices](foxx-readme.html)
  * [Getting started](foxx-getting-started.html)
  * [Guides](foxx-guides-readme.html)
    * [Working with routers](foxx-guides-routing.html)
    * [Working with collections](foxx-guides-collections.html)
    * [Writing queries](foxx-guides-queries.html)
    * [Development mode](foxx-guides-development-mode.html)
    * [Testing Foxx services](foxx-guides-testing.html)
    * [Foxx in a cluster](foxx-guides-cluster.html)
    * [Scripts and scheduling](foxx-guides-scripts.html)
    * [Using Node modules](foxx-guides-bundled-node-modules.html)
    * [Using Webpack with Foxx](foxx-guides-webpack.html)
    * [Authentication and sessions](foxx-guides-auth.html)
    * [Linking services together](foxx-guides-dependencies.html)
    * [Working with files](foxx-guides-files.html)
    * [Making requests](foxx-guides-making-requests.html)
    * [Access from the browser](foxx-guides-browser.html)
    * [Working with 2.x services](foxx-guides-legacy-mode.html)
  * [Reference](foxx-reference-readme.html)
    * [Service manifest](foxx-reference-manifest.html)
    * [Service context](foxx-reference-context.html)
    * [Configuration](foxx-reference-configuration.html)
    * [Routers](foxx-reference-routers-readme.html)
      * [Endpoints](foxx-reference-routers-endpoints.html)
      * [Middleware](foxx-reference-routers-middleware.html)
      * [Request](foxx-reference-routers-request.html)
      * [Response](foxx-reference-routers-response.html)
    * [Sessions middleware](foxx-reference-sessions-readme.html)
      * [Session storages](foxx-reference-sessions-storages-readme.html)
        * [Collection storage](foxx-reference-sessions-storages-collection.html)
        * [JWT storage](foxx-reference-sessions-storages-j-w-t.html)
      * [Session transports](foxx-reference-sessions-transports-readme.html)
        * [Cookie transport](foxx-reference-sessions-transports-cookie.html)
        * [Header transport](foxx-reference-sessions-transports-header.html)
    * [Related modules](foxx-reference-modules-readme.html)
      * [Authentication](foxx-reference-modules-auth.html)
      * [OAuth 1.0a](foxx-reference-modules-o-auth1.html)
      * [OAuth 2.0](foxx-reference-modules-o-auth2.html)
      * [GraphQL](foxx-reference-modules-graph-q-l.html)
      * [Queues](foxx-reference-modules-queues.html)
  * [Deployment](foxx-deployment.html)
  * [Migrating 2.x services](foxx-migrating2x-readme.html)
    * [Migrating from pre-2.8](foxx-migrating2x-wayback.html)
    * [manifest.json](foxx-migrating2x-manifest.html)
    * [applicationContext](foxx-migrating2x-context.html)
    * [Repositories and Models](foxx-migrating2x-repositories.html)
    * [Controllers](foxx-migrating2x-controllers-readme.html)
      * [Request context](foxx-migrating2x-controllers-endpoints.html)
      * [Error handling](foxx-migrating2x-controllers-errors.html)
      * [Before/After/Around](foxx-migrating2x-controllers-middleware.html)
      * [Request object](foxx-migrating2x-controllers-request.html)
      * [Response object](foxx-migrating2x-controllers-response.html)
      * [Dependency Injection](foxx-migrating2x-controllers-io-c.html)
    * [Sessions](foxx-migrating2x-sessions.html)
    * [Auth and OAuth2](foxx-migrating2x-auth.html)
    * [Foxx Queries](foxx-migrating2x-queries.html)
* [Satellite Collections](satellites.html)
* [Smart Joins](smart-joins.html)

## OPERATIONS

* [Installation](installation-readme.html)
  * [Linux](installation-linux.html)
    * [Operating System Configuration](installation-linux-os-configuration.html)
    * [Linux OS Tuning Script Examples](installation-linux-os-tuning-scripts.html)    
  * [macOS](installation-macos-x.html)
  * [Windows](installation-windows.html)
  * [Compiling](installation-compiling.html)
* [Uninstallation](uninstallation-readme.html)
* [Deployment](deployment-readme.html)
  * [By ArangoDB Deployment Modes](deployment-modes.html)
    * [Single Instance](deployment-single-instance-readme.html)
      * [Using the ArangoDB Starter](deployment-single-instance-using-the-starter.html)
      * [Manual Start](deployment-single-instance-manual-start.html)
    * [Master/Slave](deployment-master-slave-readme.html)
      * [Manual Start](deployment-master-slave-manual-start.html)
    * [Active Failover](deployment-active-failover-readme.html)
      * [Using the ArangoDB Starter](deployment-active-failover-using-the-starter.html)
      * [Manual Start](deployment-active-failover-manual-start.html)
    * [Cluster](deployment-cluster-readme.html)  
      * [Preliminary Information](deployment-cluster-preliminary-information.html)	
      * [Using the ArangoDB Starter](deployment-cluster-using-the-starter.html)
      * [Manual Start](deployment-cluster-manual-start.html)
      * [Kubernetes](deployment-cluster-kubernetes.html)	
      * [Mesos, DC/OS](deployment-cluster-mesos.html)	
    <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
    * [Multiple Datacenters](deployment-dc2dc-readme.html)
      * [Cluster](deployment-dc2dc-cluster.html) 
      * [ArangoSync Master](deployment-dc2dc-arango-sync-master.html)
      * [ArangoSync Workers](deployment-dc2dc-arango-sync-workers.html)
      * [Prometheus & Grafana](deployment-dc2dc-prometheus-grafana.html)
      * [Kafka & Zookeeper](deployment-dc2dc-kafka-zookeeper.html)
    * [Standalone Agency](deployment-standalone-agency-readme.html) 
  * [By Technology](deployment-technology.html)
    * [Manually](deployment-manually-readme.html)
    * [ArangoDB Starter](deployment-arango-db-starter-readme.html)
    * [Docker](deployment-docker-readme.html)
    <!-- SYNC: https://@github.com/arangodb/kube-arangodb.git;kube-arangodb;docs/Manual;;/ -->
    * [Kubernetes](deployment-kubernetes-readme.html)
      * [Using the Operator](deployment-kubernetes-usage.html)
      * [Dashboards](deployment-kubernetes-dashboards.html)
      * [Deployment Resource Reference](deployment-kubernetes-deployment-resource.html)
      * [Driver Configuration](deployment-kubernetes-driver-configuration.html)
      * [Helm](deployment-kubernetes-helm.html)
      * [Authentication](deployment-kubernetes-authentication.html)
      * [Scaling](deployment-kubernetes-scaling.html)
      * [Draining Nodes](deployment-kubernetes-drain.html)
      * [Upgrading](deployment-kubernetes-upgrading.html)
      * [ArangoDB Configuration & Secrets](deployment-kubernetes-config-and-secrets.html)
      * [Metrics](deployment-kubernetes-metrics.html)
      * [Services & Load balancer](deployment-kubernetes-services-and-load-balancer.html)
      * [Deployment Replication Resource Reference](deployment-kubernetes-deployment-replication-resource.html)
      * [Storage](deployment-kubernetes-storage.html)
      * [Storage Resource](deployment-kubernetes-storage-resource.html)
      * [TLS](deployment-kubernetes-tls.html)
      * [Troubleshooting](deployment-kubernetes-troubleshooting.html)
    * [Mesos, DC/OS](deployment-dcos-readme.html)
      * [Cluster Deployments](deployment-dcos-cluster-mesos.html)
        * [Choosing Container Engine](deployment-dcos-mesos-containers.html)
  * [In the Cloud](deployment-cloud-readme.html)
    * [AWS](deployment-cloud-aws.html)
    * [Azure](deployment-cloud-azure.html)
  * [Production Checklist](deployment-production-checklist.html)
  * [Migrating Single Instance to Cluster](deployment-migrating-single-instance-cluster.html)
* [Backup & Restore](backup-restore-readme.html)
* [Upgrading](upgrading-readme.html)
  * [General Upgrade Information](upgrading-general-info-readme.html)
  * [Community to Enterprise Upgrade](upgrading-community-to-enterprise.html)
  * [OS-specific Information](upgrading-os-specific-info-readme.html)
    * [Upgrading on Linux](upgrading-os-specific-info-linux.html)
    * [Upgrading on macOS](upgrading-os-specific-info-macos.html)
    * [Upgrading on Windows](upgrading-os-specific-info-windows.html)    
  * [Upgrading _Starter_ Deployments](upgrading-starter-readme.html)  
  * [Upgrading Manual Deployments](upgrading-manually-readme.html)
    * [Upgrading an Active Failover deployment](upgrading-manually-active-failover.html)	
    * [Upgrading a Cluster](upgrading-manually-cluster.html)
  * [Upgrading Kubernetes Deployments](upgrading-kubernetes-readme.html)
  * [Version Specific Upgrade Information](upgrading-version-specific-readme.html)
    * [Upgrading to 3.4](upgrading-version-specific-upgrading34.html)
    * [Upgrading to 3.3](upgrading-version-specific-upgrading33.html)
    * [Upgrading to 3.2](upgrading-version-specific-upgrading32.html)
    * [Upgrading to 3.1](upgrading-version-specific-upgrading31.html)
    * [Upgrading to 3.0](upgrading-version-specific-upgrading30.html)
    * [Upgrading to 2.8](upgrading-version-specific-upgrading28.html)
    * [Upgrading to 2.6](upgrading-version-specific-upgrading26.html)
    * [Upgrading to 2.5](upgrading-version-specific-upgrading25.html)
    * [Upgrading to 2.4](upgrading-version-specific-upgrading24.html)
    * [Upgrading to 2.3](upgrading-version-specific-upgrading23.html)
    * [Upgrading to 2.2](upgrading-version-specific-upgrading22.html)
* [Downgrading](downgrading-readme.html)
* [Scaling](scaling-readme.html)
* [Administration](administration-readme.html)
  * [Configuration](administration-configuration-readme.html)
  * [Import & Export](administration-import-export.html)
  * [User Management](administration-managing-users-readme.html)
    * [In Arangosh](administration-managing-users-in-arangosh.html)
  * [Switch Storage Engine](administration-engine-switch-engine.html)
  * [Master/Slave](administration-master-slave-readme.html)
    * [Setting up](administration-master-slave-setting-up.html)
      * [Replication Applier](administration-master-slave-replication-applier.html)
      * [Per-Database Setup](administration-master-slave-database-setup.html)
      * [Server-Level Setup](administration-master-slave-server-level-setup.html)
    * [Syncing Collections](administration-master-slave-syncing-collections.html)
  * [Active Failover](administration-active-failover-readme.html)
  * [Cluster](administration-cluster-readme.html)
  <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
  * [Datacenter to datacenter replication](administration-dc2dc-readme.html)
  <!-- SYNC: https://@github.com/arangodb-helper/arangodb.git;arangodb;docs/Manual;;/ -->
  * [ArangoDB Starter Administration](administration-starter-readme.html)
    * [ArangoDB Starter Removal Procedure](administration-starter-removal.html)
    * [ArangoDB Starter Recovery Procedure](administration-starter-recovery.html)
* [Security](security-readme.html)
  * [Change Root Password](security-change-root-password.html)
  * [Encryption at Rest](security-encryption-readme.html)
  * [Auditing](security-auditing-readme.html)
    * [Configuration](security-auditing-audit-configuration.html)
    * [Events](security-auditing-audit-events.html)
  <!-- SYNC: https://@github.com/arangodb-helper/arangodb.git;arangodb;docs/Manual;;/ -->
  * [Securing Starter Deployments](security-starter-readme.html)
  <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
  * [Datacenter to datacenter replication](security-dc2dc-readme.html)
* [Monitoring](monitoring-readme.html)
  * [Log Levels](monitoring-log-levels.html)
  <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
  * [Datacenter to datacenter replication](monitoring-dc2dc-readme.html)
* [Troubleshooting](troubleshooting-readme.html)
  * [arangod](troubleshooting-arangod.html)
  * [Emergency Console](troubleshooting-emergency-console.html)
  * [Cluster](troubleshooting-cluster-readme.html)
    * [Agency Dump](troubleshooting-cluster-agency-dump.html)
  <!-- SYNC: https://@github.com/arangodb/arangosync.git;arangosync;docs/Manual;;/ -->
  * [Datacenter to datacenter replication](troubleshooting-dc2dc-readme.html)

---

* [Release Notes](release-notes-readme.html)
  * [Version 3.4](release-notes-34.html)
    * [What's New in 3.4](release-notes-new-features34.html)
    * [Known Issues in 3.4](release-notes-known-issues34.html)
    * [Incompatible changes in 3.4](release-notes-upgrading-changes34.html)
  * [Version 3.3](release-notes-33.html)
    * [What's New in 3.3](release-notes-new-features33.html)
    * [Known Issues in 3.3](release-notes-known-issues33.html)
    * [Incompatible changes in 3.3](release-notes-upgrading-changes33.html)
  * [Version 3.2](release-notes-32.html)
    * [What's New in 3.2](release-notes-new-features32.html)
    * [Known Issues in 3.2](release-notes-known-issues32.html)
    * [Incompatible changes in 3.2](release-notes-upgrading-changes32.html)
  * [Version 3.1](release-notes-31.html)
    * [What's New in 3.1](release-notes-new-features31.html)
    * [Incompatible changes in 3.1](release-notes-upgrading-changes31.html)
  * [Version 3.0](release-notes-30.html)
    * [What's New in 3.0](release-notes-new-features30.html)
    * [Incompatible changes in 3.0](release-notes-upgrading-changes30.html)
  * [Version 2.8](release-notes-28.html)
    * [What's New in 2.8](release-notes-new-features28.html)
    * [Incompatible changes in 2.8](release-notes-upgrading-changes28.html)
  * [Version 2.7](release-notes-27.html)
    * [What's New in 2.7](release-notes-new-features27.html)
    * [Incompatible changes in 2.7](release-notes-upgrading-changes27.html)
  * [Version 2.6](release-notes-26.html)
    * [What's New in 2.6](release-notes-new-features26.html)
    * [Incompatible changes in 2.6](release-notes-upgrading-changes26.html)
  * [Version 2.5](release-notes-25.html)
    * [What's New in 2.5](release-notes-new-features25.html)
    * [Incompatible changes in 2.5](release-notes-upgrading-changes25.html)
  * [Version 2.4](release-notes-24.html)
    * [What's New in 2.4](release-notes-new-features24.html)
    * [Incompatible changes in 2.4](release-notes-upgrading-changes24.html)
  * [Version 2.3](release-notes-23.html)
    * [What's New in 2.3](release-notes-new-features23.html)
    * [Incompatible changes in 2.3](release-notes-upgrading-changes23.html)
  * [Version 2.2](release-notes-22.html)
    * [What's New in 2.2](release-notes-new-features22.html)
  * [Version 2.1](release-notes-21.html)
    * [What's New in 2.1](release-notes-new-features21.html)
* [Appendix](appendix-readme.html)
  * [References](appendix-references-readme.html)
    * [db](appendix-references-db-object.html)
    * [collection](appendix-references-collection-object.html)
    * [cursor](appendix-references-cursor-object.html)
  * [JavaScript Modules](appendix-java-script-modules-readme.html)
    * [@arangodb](appendix-java-script-modules-arango-db.html)
    * [console](appendix-java-script-modules-console.html)
    * [crypto](appendix-java-script-modules-crypto.html)
    * [fs](appendix-java-script-modules-file-system.html)
    * [request](appendix-java-script-modules-request.html)
    * [actions](appendix-java-script-modules-actions.html)
    * [queries](appendix-java-script-modules-queries.html)
    * [Write-ahead log](appendix-java-script-modules-wal.html)
    * [Task Management](appendix-java-script-modules-tasks.html)
  * [Deprecated](appendix-deprecated-readme.html)
      * [Simple Queries](appendix-deprecated-simple-queries-readme.html)
        * [Pagination](appendix-deprecated-simple-queries-pagination.html)
        * [Modification Queries](appendix-deprecated-simple-queries-modification-queries.html)
        * [Geo Queries](appendix-deprecated-simple-queries-geo-queries.html)
        * [Fulltext Queries](appendix-deprecated-simple-queries-fulltext-queries.html)
      * [Actions](appendix-deprecated-actions-readme.html)
        * [Delivering HTML Pages](appendix-deprecated-actions-html-example.html)
        * [Json Objects](appendix-deprecated-actions-json-example.html)
        * [Modifying](appendix-deprecated-actions-modifying.html)
  * [Error codes and meanings](appendix-error-codes.html)
  * [Glossary](appendix-glossary.html)