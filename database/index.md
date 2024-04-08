---
label: Database Design (Coding)
order: 99
icon: key
---

USERS

- username
- email
- password_hash
- account_type


Profile

- firstname
- last name
- photo
- bio
- preference


Subscription

- email
- subscribed
- interest


menu group

- name
- status

menu

- name
- url
- order
- type? (sub or main)
- parent_id?
- parent_name?
- menu_group_id?

Commentary (WIP)
- id
- title
- abstract
- body
- slug
- featured
- published
- published_at
- timestamp

Library (WIP)
- id