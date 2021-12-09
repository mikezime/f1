
Category


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| CategoryName | VARCHAR(8000) | No | No | Contains Category Name |
| Description | VARCHAR(8000) | No | No | Contains Description |

Customer


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | VARCHAR(8000) | Yes | No | Contains Id |
| CompanyName | VARCHAR(8000) | No | No | Contains Company Name |
| ContactName | VARCHAR(8000) | No | No | Contains Contact Name |
| ContactTitle | VARCHAR(8000) | No | No | Contains Contact Title |
| Address | VARCHAR(8000) | No | No | Contains Address |
| City | VARCHAR(8000) | No | No | Contains City |
| Region | VARCHAR(8000) | No | No | Contains Region |
| PostalCode | VARCHAR(8000) | No | No | Contains Postal Code |
| Country | VARCHAR(8000) | No | No | Contains Country |
| Phone | VARCHAR(8000) | No | No | Contains Phone |
| Fax | VARCHAR(8000) | No | No | Contains Fax |

CustomerCustomerDemo


CustomerDemographic


Employee


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| LastName | VARCHAR(8000) | No | No | Contains Last Name |
| FirstName | VARCHAR(8000) | No | No | Contains First Name |
| Title | VARCHAR(8000) | No | No | Contains Title |
| TitleOfCourtesy | VARCHAR(8000) | No | No | Contains Title Of Courtesy |
| BirthDate | VARCHAR(8000) | No | No | Contains Birth Date |
| HireDate | VARCHAR(8000) | No | No | Contains Hire Date |
| Address | VARCHAR(8000) | No | No | Contains Address |
| City | VARCHAR(8000) | No | No | Contains City |
| Region | VARCHAR(8000) | No | No | Contains Region |
| PostalCode | VARCHAR(8000) | No | No | Contains Postal Code |
| Country | VARCHAR(8000) | No | No | Contains Country |
| HomePhone | VARCHAR(8000) | No | No | Contains Home Phone |
| Extension | VARCHAR(8000) | No | No | Contains Extension |
| Photo | BLOB | No | No | Contains Photo |
| Notes | VARCHAR(8000) | No | No | Contains Notes |
| ReportsTo | INTEGER | No | No | Contains Reports To |
| PhotoPath | VARCHAR(8000) | No | No | Contains Photo Path |

EmployeeTerritory


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | VARCHAR(8000) | Yes | No | Contains Id |
| EmployeeId | INTEGER | No | Yes | Contains Employee Id |
| TerritoryId | VARCHAR(8000) | No | No | Contains Territory Id |

Order


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| CustomerId | VARCHAR(8000) | No | No | Contains Customer Id |
| EmployeeId | INTEGER | No | Yes | Contains Employee Id |
| OrderDate | VARCHAR(8000) | No | No | Contains Order Date |
| RequiredDate | VARCHAR(8000) | No | No | Contains Required Date |
| ShippedDate | VARCHAR(8000) | No | No | Contains Shipped Date |
| ShipVia | INTEGER | No | No | Contains Ship Via |
| Freight | DECIMAL | No | Yes | Contains Freight |
| ShipName | VARCHAR(8000) | No | No | Contains Ship Name |
| ShipAddress | VARCHAR(8000) | No | No | Contains Ship Address |
| ShipCity | VARCHAR(8000) | No | No | Contains Ship City |
| ShipRegion | VARCHAR(8000) | No | No | Contains Ship Region |
| ShipPostalCode | VARCHAR(8000) | No | No | Contains Ship Postal Code |
| ShipCountry | VARCHAR(8000) | No | No | Contains Ship Country |

OrderDetail


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | VARCHAR(8000) | Yes | No | Contains Id |
| OrderId | INTEGER | No | Yes | Contains Order Id |
| ProductId | INTEGER | No | Yes | Contains Product Id |
| UnitPrice | DECIMAL | No | Yes | Contains Unit Price |
| Quantity | INTEGER | No | Yes | Contains Quantity |
| Discount | DOUBLE | No | Yes | Contains Discount |

Product


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| ProductName | VARCHAR(8000) | No | No | Contains Product Name |
| SupplierId | INTEGER | No | Yes | Contains Supplier Id |
| CategoryId | INTEGER | No | Yes | Contains Category Id |
| QuantityPerUnit | VARCHAR(8000) | No | No | Contains Quantity Per Unit |
| UnitPrice | DECIMAL | No | Yes | Contains Unit Price |
| UnitsInStock | INTEGER | No | Yes | Contains Units In Stock |
| UnitsOnOrder | INTEGER | No | Yes | Contains Units On Order |
| ReorderLevel | INTEGER | No | Yes | Contains Reorder Level |
| Discontinued | INTEGER | No | Yes | Contains Discontinued |

Region


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| RegionDescription | VARCHAR(8000) | No | No | Contains Region Description |

Shipper


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| CompanyName | VARCHAR(8000) | No | No | Contains Company Name |
| Phone | VARCHAR(8000) | No | No | Contains Phone |

Supplier


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | INTEGER | Yes | No | Contains Id |
| CompanyName | VARCHAR(8000) | No | No | Contains Company Name |
| ContactName | VARCHAR(8000) | No | No | Contains Contact Name |
| ContactTitle | VARCHAR(8000) | No | No | Contains Contact Title |
| Address | VARCHAR(8000) | No | No | Contains Address |
| City | VARCHAR(8000) | No | No | Contains City |
| Region | VARCHAR(8000) | No | No | Contains Region |
| PostalCode | VARCHAR(8000) | No | No | Contains Postal Code |
| Country | VARCHAR(8000) | No | No | Contains Country |
| Phone | VARCHAR(8000) | No | No | Contains Phone |
| Fax | VARCHAR(8000) | No | No | Contains Fax |
| HomePage | VARCHAR(8000) | No | No | Contains Home Page |

Territory


| FieldName | FieldType | PrimaryKey | NotNull | Description |
| --- | --- | --- | --- | --- |
| Id | VARCHAR(8000) | Yes | No | Contains Id |
| TerritoryDescription | VARCHAR(8000) | No | No | Contains Territory Description |
| RegionId | INTEGER | No | Yes | Contains Region Id |

