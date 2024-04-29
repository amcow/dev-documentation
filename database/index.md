---
label: Database Design (Coding)
order: 99
icon: key
---


CASE STUDIES

- username
- email
- password_hash
- account_type

USERS

- publish_date
- photo
- authour_id
- account_type
- embedding
- title_en (title english)
- content_en
- title_ar  (title arabic)
- content_ar
- title_pt (title portuguese)
- content_pt
- title_fr (title french)
- content_fr

Profile

- firstname
- last name
- photo
- bio
- preference


Library (WIP)
- id
- pages
- view_count
- published_at
- category
- sub_category
- tags
- embedding
- title_ar
- summary_ar
- link_ar
- title_en
- summary_en
- link_en
- title_fr
- summary_fr
- link_fr
- title_pt
- summary_pt
- link_pt


Categories/Subject (Is there a possibilty of a resources having being in multiple areas)
- id
- name


sub categogories (Could this be embedded or tags)
- id
- name
- subcategory_id


Videos

- title
- link
- views
- length
- summary
- embedding
- transcription?


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
