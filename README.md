# Ember Cheat Sheet

## State & Reactivity

| Feature | Purpose | Notes |
|----------|----------|----------|
| `@tracked` | | |
| `@computed` | | |
| `@computed("items.[]")` | | |
| `@computed("items.@each.id")` | | |
| `@computed("object.{prop1,prop2}")` | | |
| Getter (`get`) | | |
| Setter (`set`) | | |

## Actions & Arguments

| Feature | Purpose | Notes |
|----------|----------|----------|
| `@action` | | |
| `this.args` | | |
| `...attributes` | | |

## Property Access

| Feature | Purpose | Notes |
|----------|----------|----------|
| `this.get()` | | |
| `object.get()` | | |
| `get()` | | |
| `this.set()` | | |
| `set()` | | |
| Direct assignment (`=`) | | |
| `@alias` | | |

## Lifecycle & Template Modifiers

| Feature | Purpose | Notes |
|----------|----------|----------|
| `init()` | | |
| `constructor()` | | |
| `did-insert` | | |
| `did-update` | | |
| `will-destroy` | | |
| `willDestroy()` | | |

## Data & Objects

| Feature | Purpose | Notes |
|----------|----------|----------|
| Proxy Object | | |
| `EmberObject` | | |
| `EmberObject.create()` | | |
| `A([])` | | |
| `Changeset` | | |
| `changeset.error` | | |

## Services & Dependency Injection

| Feature | Purpose | Notes |
|----------|----------|----------|
| `@service` | | |
| `getOwner()` | | |
| `setOwner()` | | |

## Runloop

| Feature | Purpose | Notes |
|----------|----------|----------|
| `scheduleOnce()` | | |
| `schedule()` | | |
| `later()` | | |

## Storage & Utilities

| Feature | Purpose | Notes |
|----------|----------|----------|
| `storageFor()` | | |
| `UUID.v4()` | | |
| `debug` | | |
| `isEmpty()` | | |

## Async

| Feature | Purpose | Notes |
|----------|----------|----------|
| `RSVP` | | |
| `RSVP.allSettled()` | | |

## Cleanup

| Feature | Purpose | Notes |
|----------|----------|----------|
| `registerDestructor()` | | |

---

# Classic → Glimmer Migration

| Classic Ember | Glimmer |
|----------|----------|
| `this.get()` | |
| `this.set()` | |
| `object.get()` | |
| `object.set()` | |
| `init()` | |
| `@computed` | |
| `this.onClose()` | |
| `@ember/component` | |
| `didInsertElement()` | |
| `willDestroyElement()` | |
