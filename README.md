# Ember Cheat Sheet

## State & Reactivity

| Feature | Purpose | Notes |
|----------|----------|----------|
| `@tracked` | Tells Ember to update the UI when this property changes | `@tracked isLoading = true`<br>`this.isLoading = false` |
| `@computed` | A classic Ember property that updates when its dependencies change. | 🔴 `classic Ember pattern` <br>`@computed("firstName", "lastName")` |
| `@computed("items.[]")` | Watches array add/remove changes. | 🔴 `classic Ember pattern` |
| `@computed("items.@each.id")` | Watches a property inside each array item. | 🔴 `classic Ember pattern` |
| `@computed("object.{prop1,prop2}")` | Watches multiple properties on the same object. | 🔴 `classic Ember pattern` |
| Getter (`get`) | Read a property value. | `get fullName() { return ... }`<br>Use: `this.fullName` |
| Setter (`set`) | Assign a property. | `set fullName(value) { ... }`<br>Use: `this.fullName = value` |

## Actions & Arguments

| Feature | Purpose | Notes |
|----------|----------|----------|
| `@action` | Handle user actions from the template, such as click, submit, or change. | `@action`<br>`save() {}` |
| `this.args` | Read values passed from the parent component. | Parent: `<UserCard @name={{this.userName}} />`<br>Child: `this.args.name` |
| `...attributes` | Pass HTML attributes (class, id, href, ...) from parent to child element. | Parent: `<MyButton id="" class="primary" />`<br>Child: `<button ...attributes>Save</button>` |

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
