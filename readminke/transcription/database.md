---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 2
    isHidden: false
    sortIndex: -1
    width: 177
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
  date:
    input: calendar
    accessorKey: date
    key: date
    id: date
    label: date
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 101
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  language:
    input: select
    accessorKey: language
    key: language
    id: language
    label: language
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "南四縣", value: "南四縣", color: "hsl(54, 95%, 90%)"}
      - { label: "大埔", value: "大埔", color: "hsl(69, 95%, 90%)"}
      - { label: "四縣", value: "四縣", color: "hsl(95, 95%, 90%)"}
      - { label: "海陸", value: "海陸", color: "hsl(249, 95%, 90%)"}
      - { label: "詔安", value: "詔安", color: "hsl(330, 95%, 90%)"}
      - { label: "饒平", value: "饒平", color: "hsl(137, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  issue:
    input: number
    accessorKey: issue
    key: issue
    id: issue
    label: issue
    position: 1
    skipPersist: false
    isHidden: false
    sortIndex: 1
    width: -23
    isSorted: true
    isSortedDesc: false
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  author:
    input: text
    accessorKey: author
    key: author
    id: author
    label: author
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 78
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  wikidata:
    input: text
    accessorKey: wikidata
    key: wikidata
    id: wikidata
    label: wikidata
    position: 9
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  wikidata_link:
    input: formula
    accessorKey: wikidata_link
    key: wikidata_link
    id: wikidata_link
    label: wikidata link
    position: 10
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      formula_query: "https://www.wikidata.org/wiki/${row.wikidata}"
      formula_persist_type: text
  topic:
    input: text
    accessorKey: topic
    key: topic
    id: topic
    label: topic
    position: 7
    skipPersist: false
    isHidden: true
    sortIndex: -1
    width: 68
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  difficulty:
    input: number
    accessorKey: difficulty
    key: difficulty
    id: difficulty
    label: difficulty
    position: 8
    skipPersist: false
    isHidden: true
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  title:
    input: text
    accessorKey: title
    key: title
    id: title
    label: title
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 179
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      wrap_content: true
      content_alignment: text-align-left
  author_wikidata:
    input: text
    accessorKey: author_wikidata
    key: author_wikidata
    id: author_wikidata
    label: author_wikidata
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  author_wikidata_link:
    input: formula
    accessorKey: author_wikidata_link
    key: author_wikidata_link
    id: author_wikidata_link
    label: author_wikidata_link
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: true
      formula_query: "https://www.wikidata.org/wiki/${row.author_wikidata}"
      formula_persist_type: text
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 50
  font_size: 13
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
```