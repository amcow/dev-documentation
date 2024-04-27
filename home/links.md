---
label: Navigation Menu (Coding)
order: 995
icon: key
---

The menu is dynamic, with fields and URLs stored in the database. However, it will only load the menu from DB once on application startup and subsequently loads from an ETS cache.

The cache is updated through the menu manager when the menu is changed.

The existing hub has an implementation of this dynamic menu; We will migrate and improve on it.