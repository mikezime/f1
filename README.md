ContactPerson


| import_schemaLocation | import_namespace | element_name | element_type | complexType_name | element_maxOccurs | element_minOccurs |
| --- | --- | --- | --- | --- | --- | --- |
| common/CommonSchema1.xsd | urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2 |  |  |  |  |  |
| common/CAC.xsd | urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2 | ContactPerson | ContactPersonType | ContactPersonType |  |  |
|  |  | ID | cbc:IDType |  | 1 | 1 |
|  |  | Name | cbc:NameType |  | 1 | 1 |
|  |  | Telephone | cbc:TelephoneType |  | unbounded | 0 |
|  |  | ElectronicMail | cbc:ElectronicMailType |  | unbounded | 0 |
|  |  | Username | cbc:ElectronicMailType |  | 1 | 1 |
|  |  | Password | cbc:TextType |  | 1 | 1 |
|  |  | Created | cbc:DateType |  | 1 | 1 |
|  |  | Role | xsd:integer |  | 1 | 0 |
|  |  | Title | cbc:TitleType |  | 1 | 0 |
|  |  | Company_No | cbc:CompanyIDType |  | 1 | 0 |
|  |  | BillingAddress | cac:AddressType |  | 1 | 1 |
|  |  | ShippingAddress | cac:AddressType |  | unbounded | 0 |
