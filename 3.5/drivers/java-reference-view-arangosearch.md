---
layout: default
description: These functions implement the HTTP API for ArangoSearch Views
redirect_from:
  - /3.6/java-reference-view-arango-search.html # 3.4 -> 3.5
---
# ArangoSearch API

These functions implement the
[HTTP API for ArangoSearch Views](../http/views-arangosearch.html).

## ArangoDatabase.createArangoSearch

`ArangoDatabase.createArangoSearch(String name, ArangoSearchCreateOptions options) : ViewEntity`

Creates a ArangoSearch View with the given _options_, then returns
View information from the server.

**Arguments**

- **name**: `String`

  The name of the View

- **options**: `ArangoSearchCreateOptions`

  - **commitIntervalMsec**: `Long`

    Wait at least this many milliseconds between committing View data store changes
    and making documents visible to queries (default: 1000, to disable use: 0). For
    the case where there are a lot of inserts/updates, a lower value, until commit,
    will cause the index not to account for them and memory usage would continue to
    grow. For the case where there are a few inserts/updates, a higher value will
    impact performance and waste disk space for each commit call without any added
    benefits. Background: For data retrieval ArangoSearch Views follow the concept
    of "eventually-consistent", i.e. eventually all the data in ArangoDB will be
    matched by corresponding query expressions. The concept of ArangoSearch View
    "commit" operation is introduced to control the upper-bound on the time until
    document addition/removals are actually reflected by corresponding query
    expressions. Once a "commit" operation is complete all documents added/removed
    prior to the start of the "commit" operation will be reflected by queries
    invoked in subsequent ArangoDB transactions, in-progress ArangoDB transactions
    will still continue to return a repeatable-read state.

  - **consolidationIntervalMsec**: `Long`

    Wait at least this many milliseconds between committing index data changes
    and making them visible to queries (default: 60000, to disable use: 0).
    For the case where there are a lot of inserts/updates, a lower value,
    until commit, will cause the index not to account for them and memory usage
    would continue to grow. For the case where there are a few inserts/updates,
    a higher value will impact performance and waste disk space for each
    commit call without any added benefits.

  - **cleanupIntervalStep**: `Long`

    Wait at least this many commits between removing unused files in
    data directory (default: 10, to disable use: 0). For the case where the
    consolidation policies merge segments often (i.e. a lot of commit+consolidate),
    a lower value will cause a lot of disk space to be wasted. For the case
    where the consolidation policies rarely merge segments (i.e. few inserts/deletes),
    a higher value will impact performance without any added benefits.

  - **consolidationPolicy**:

    - **type**: `ConsolidationType`

      The type of the consolidation policy.

    - **threshold**: `Double`

      Select a given segment for "consolidation" if and only if the formula
      based on type (as defined above) evaluates to true, valid value range
      [0.0, 1.0] (default: 0.85)

    - **segmentThreshold**: `Long`

      Apply the "consolidation" operation if and only if (default: 300):
      `{segmentThreshold} < number_of_segments`

    - **links**: `CollectionLink[]`

      A list of linked collections

    - **primarySorts**: `CollectionLink[]`

      A list of primary sort objects. When creating an ArangoSearch View, you
      can optionally define a default sort order.

**Examples**

```Java
ArangoDB arango = new ArangoDB.Builder().build();
ArangoDatabase db = arango.db("myDB");
db.createArangoSearch("potatoes", new ArangoSearchPropertiesOptions());
// the ArangoSearch View "potatoes" now exists
```

## ArangoSearch.create

`ArangoSearch.create(ArangoSearchCreateOptions options) : ViewEntity`

Creates a ArangoSearch View with the given _options_, then returns View information from the server.

Alternative for `ArangoDatabase.createArangoSearch`.

**Arguments**

- **options**: `ArangoSearchCreateOptions`

  - **consolidationIntervalMsec**: `Long`

    Wait at least this many milliseconds between committing index data changes
    and making them visible to queries (default: 60000, to disable use: 0).
    For the case where there are a lot of inserts/updates, a lower value,
    until commit, will cause the index not to account for them and memory usage
    would continue to grow. For the case where there are a few inserts/updates,
    a higher value will impact performance and waste disk space for each
    commit call without any added benefits.

  - **cleanupIntervalStep**: `Long`

    Wait at least this many commits between removing unused files in
    data directory (default: 10, to disable use: 0). For the case where the
    consolidation policies merge segments often (i.e. a lot of commit+consolidate),
    a lower value will cause a lot of disk space to be wasted. For the case
    where the consolidation policies rarely merge segments (i.e. few inserts/deletes),
    a higher value will impact performance without any added benefits.

  - **consolidationPolicy**:

    - **type**: `ConsolidationType`

      The type of the consolidation policy.

    - **threshold**: `Double`

      Select a given segment for "consolidation" if and only if the formula
      based on type (as defined above) evaluates to true, valid value range
      [0.0, 1.0] (default: 0.85)

    - **segmentThreshold**: `Long`

      Apply the "consolidation" operation if and only if (default: 300):
      `{segmentThreshold} < number_of_segments`

    - **link**: `CollectionLink[]`

      A list of linked collections

**Examples**

```Java
ArangoDB arango = new ArangoDB.Builder().build();
ArangoDatabase db = arango.db("myDB");
ArangoSearch view = db.arangoSearch("potatoes");

view.create(new ArangoSearchPropertiesOptions());
// the ArangoSearch View "potatoes" now exists
```

## ArangoSearch.getProperties

`ArangoSearch.getProperties() : ArangoSearchPropertiesEntity`

Reads the properties of the specified View.

**Examples**

```Java
ArangoDB arango = new ArangoDB.Builder().build();
ArangoDatabase db = arango.db("myDB");
ArangoSearch view = db.arangoSearch("potatoes");

ArangoSearchPropertiesEntity properties = view.getProperties();
```

## ArangoSearch.updateProperties

`ArangoSearch.updateProperties(ArangoSearchPropertiesOptions options) : ArangoSearchPropertiesEntity`

Partially changes properties of the View.

**Arguments**

- **options**: `ArangoSearchPropertiesOptions`

  - **consolidationIntervalMsec**: `Long`

    Wait at least this many milliseconds between committing index data changes
    and making them visible to queries (default: 60000, to disable use: 0).
    For the case where there are a lot of inserts/updates, a lower value,
    until commit, will cause the index not to account for them and memory usage
    would continue to grow. For the case where there are a few inserts/updates,
    a higher value will impact performance and waste disk space for each
    commit call without any added benefits.

  - **cleanupIntervalStep**: `Long`

    Wait at least this many commits between removing unused files in
    data directory (default: 10, to disable use: 0). For the case where the
    consolidation policies merge segments often (i.e. a lot of commit+consolidate),
    a lower value will cause a lot of disk space to be wasted. For the case
    where the consolidation policies rarely merge segments (i.e. few inserts/deletes),
    a higher value will impact performance without any added benefits.

  - **consolidationPolicy**:

    - **type**: `ConsolidationType`

      The type of the consolidation policy.

    - **threshold**: `Double`

      Select a given segment for "consolidation" if and only if the formula
      based on type (as defined above) evaluates to true, valid value range
      [0.0, 1.0] (default: 0.85)

    - **segmentThreshold**: `Long`

      Apply the "consolidation" operation if and only if (default: 300):
      `{segmentThreshold} < number_of_segments`

    - **link**: `CollectionLink[]`

      A list of linked collections

**Examples**

```Java
ArangoDB arango = new ArangoDB.Builder().build();
ArangoDatabase db = arango.db("myDB");
ArangoSearch view = db.arangoSearch("some-view");

view.updateProperties(
  new ArangoSearchPropertiesOptions()
    .link(CollectionLink.on("myCollection").fields(FieldLink.on("value").analyzers("identity")))
);
```

## ArangoSearch.replaceProperties

`ArangoSearch.replaceProperties(ArangoSearchPropertiesOptions options) : ArangoSearchPropertiesEntity`

Changes properties of the View.

**Arguments**

- **options**: `ArangoSearchPropertiesOptions`

  - **consolidationIntervalMsec**: `Long`

    Wait at least this many milliseconds between committing index data changes
    and making them visible to queries (default: 60000, to disable use: 0).
    For the case where there are a lot of inserts/updates, a lower value,
    until commit, will cause the index not to account for them and memory usage
    would continue to grow. For the case where there are a few inserts/updates,
    a higher value will impact performance and waste disk space for each
    commit call without any added benefits.

  - **cleanupIntervalStep**: `Long`

    Wait at least this many commits between removing unused files in
    data directory (default: 10, to disable use: 0). For the case where the
    consolidation policies merge segments often (i.e. a lot of commit+consolidate),
    a lower value will cause a lot of disk space to be wasted. For the case
    where the consolidation policies rarely merge segments (i.e. few inserts/deletes),
    a higher value will impact performance without any added benefits.

  - **consolidationPolicy**:

    - **type**: `ConsolidationType`

      The type of the consolidation policy.

    - **threshold**: `Double`

      Select a given segment for "consolidation" if and only if the formula
      based on type (as defined above) evaluates to true, valid value range
      [0.0, 1.0] (default: 0.85)

    - **segmentThreshold**: `Long`

      Apply the "consolidation" operation if and only if (default: 300):
      `{segmentThreshold} < number_of_segments`

    - **link**: `CollectionLink[]`

      A list of linked collections

**Examples**

```Java
ArangoDB arango = new ArangoDB.Builder().build();
ArangoDatabase db = arango.db("myDB");
ArangoSearch view = db.arangoSearch("some-view");

view.replaceProperties(
  new ArangoSearchPropertiesOptions()
    .link(CollectionLink.on("myCollection").fields(FieldLink.on("value").analyzers("identity")))
);
```
