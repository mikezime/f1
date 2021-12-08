States


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| StateName | TEXT | No | No | Contains State Name |
| StateCode | TEXT | No | No | Contains State Code |
| Region | TEXT | No | No | Contains Region |
| SubRegion | TEXT | No | No | Contains Sub Region |

address


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| FirstName | TEXT | No | No | Contains First Name |
| LastName1 | TEXT | No | No | Contains Last Name1 |
| Organization | TEXT | No | No | Contains Organization |
| JobTitle | TEXT | No | No | Contains Job Title |
| StreetAddress | TEXT | No | No | Contains Street Address |
| Zip | TEXT | No | No | Contains Zip |
| City | TEXT | No | No | Contains City |
| CountryName | TEXT | No | No | Contains Country Name |
| Phone | TEXT | No | No | Contains Phone |
| Mobile | TEXT | No | No | Contains Mobile |
| Email | TEXT | No | No | Contains Email |
| HomePage | TEXT | No | No | Contains Home Page |

moz_anno_attributes


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| name | VARCHAR(32) | No | Yes | Contains name |

moz_annos


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| place_id | INTEGER | No | Yes | Contains place_id |
| anno_attribute_id | INTEGER | No | No | Contains anno_attribute_id |
| mime_type | VARCHAR(32) | No | No | Contains mime_type |
| content | LONGVARCHAR | No | No | Contains content |
| flags | INTEGER | No | No | Contains flags |
| expiration | INTEGER | No | No | Contains expiration |
| type | INTEGER | No | No | Contains type |
| dateAdded | INTEGER | No | No | Contains date Added |
| lastModified | INTEGER | No | No | Contains last Modified |

moz_bookmarks


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| type | INTEGER | No | No | Contains type |
| fk | INTEGER | No | No | Contains fk |
| parent | INTEGER | No | No | Contains parent |
| position | INTEGER | No | No | Contains position |
| title | LONGVARCHAR | No | No | Contains title |
| keyword_id | INTEGER | No | No | Contains keyword_id |
| folder_type | TEXT | No | No | Contains folder_type |
| dateAdded | INTEGER | No | No | Contains date Added |
| lastModified | INTEGER | No | No | Contains last Modified |
| guid | TEXT | No | No | Contains guid |
| syncStatus | INTEGER | No | Yes | Contains sync Status |
| syncChangeCounter | INTEGER | No | Yes | Contains sync Change Counter |

moz_bookmarks_deleted


moz_favicons


moz_historyvisits


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| from_visit | INTEGER | No | No | Contains from_visit |
| place_id | INTEGER | No | No | Contains place_id |
| visit_date | INTEGER | No | No | Contains visit_date |
| visit_type | INTEGER | No | No | Contains visit_type |
| session | INTEGER | No | No | Contains session |

moz_hosts


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| host | TEXT | No | Yes | Contains host |
| frecency | INTEGER | No | No | Contains frecency |
| typed | INTEGER | No | Yes | Contains typed |
| prefix | TEXT | No | No | Contains prefix |

moz_inputhistory


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| place_id | INTEGER | Yes | Yes | Contains place_id |
| input | LONGVARCHAR | No | Yes | Contains input |
| use_count | INTEGER | No | No | Contains use_count |

moz_items_annos


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| item_id | INTEGER | No | Yes | Contains item_id |
| anno_attribute_id | INTEGER | No | No | Contains anno_attribute_id |
| mime_type | VARCHAR(32) | No | No | Contains mime_type |
| content | LONGVARCHAR | No | No | Contains content |
| flags | INTEGER | No | No | Contains flags |
| expiration | INTEGER | No | No | Contains expiration |
| type | INTEGER | No | No | Contains type |
| dateAdded | INTEGER | No | No | Contains date Added |
| lastModified | INTEGER | No | No | Contains last Modified |

moz_keywords


moz_places


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| id | INTEGER | Yes | No | Contains id |
| url | LONGVARCHAR | No | No | Contains url |
| title | LONGVARCHAR | No | No | Contains title |
| rev_host | LONGVARCHAR | No | No | Contains rev_host |
| visit_count | INTEGER | No | No | Contains visit_count |
| hidden | INTEGER | No | Yes | Contains hidden |
| typed | INTEGER | No | Yes | Contains typed |
| favicon_id | INTEGER | No | No | Contains favicon_id |
| frecency | INTEGER | No | Yes | Contains frecency |
| last_visit_date | INTEGER | No | No | Contains last_visit_date |
| guid | TEXT | No | No | Contains guid |
| foreign_count | INTEGER | No | Yes | Contains foreign_count |
| url_hash | INTEGER | No | Yes | Contains url_hash |
| description | TEXT | No | No | Contains description |
| preview_image_url | TEXT | No | No | Contains preview_image_url |

sqlite_sequence


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| name | String | No | No | Contains name |
| seq | Object | No | No | Contains seq |

sqlite_stat1


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| tbl | String | No | No | Contains tbl |
| idx | String | No | No | Contains idx |
| stat | String | No | No | Contains stat |
