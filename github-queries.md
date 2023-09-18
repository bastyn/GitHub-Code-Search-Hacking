# Queries

## Scope

```text
repo:<your-repo> <dork>
org:<your-org> <dork>
```

## Show files that are most likely related to production environment

```text
<dork> NOT path:*tst* NOT path:*test* NOT path:*dev* NOT path:*development* NOT path:*local* NOT path:*acc* NOT path:*acceptance* NOT path:*staging*
```
