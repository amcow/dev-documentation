---
label: Database Design (Coding)
order: 99
icon: key
---

### case studies

- id
- publish_at
- photo
- author_id
- embedding
- slug
- view_count
- title_en (title english)
- content_en
- title_ar  (title arabic)
- content_ar
- title_pt (title portuguese)
- content_pt
- title_fr (title french)
- content_fr



### press

- id
- publish_at
- embedding (this can be ignored for now)
- slug
- view_count
- title_en (title english)
- link_en
- title_ar  (title arabic)
- link_ar
- title_pt (title portuguese)
- link_pt
- title_fr (title french)
- link_fr

### users

- username
- email
- password_hash
- account_type
- more fields ...

###  profile

- firstname
- last name
- photo
- bio
- preference
- more fields ...


### library (WIP)

- id
- pages
- view_count
- published_at
- category
- sub_category
- tags
- embedding
- slug
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


### categories/subjects
(Is there a possibilty of a resources having being in multiple categories/subjects)

- id
- name


### sub categories 
(Could this be embedded or tags)

- id
- name
- subcategory_id


###  videos

- title
- link
- views
- length
- summary
- embedding
- transcription?


###  subscription

- email
- subscribed
- interest
- more fields ...

### menu group

- name
- status

### menu

- name
- url
- order
- type? (sub or main)
- parent_id?
- parent_name?
- menu_group_id?
