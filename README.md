Transaction


| element_name | element_type | element_minOccurs |
| --- | --- | --- |
| TransactionRequest |  |  |
| GatewayID | xs:string | 0 |
| Name | xs:string | 0 |
| Address | xs:string | 0 |
| City | xs:string | 0 |
| State | xs:string | 0 |
| ZipCode | xs:string | 0 |
| Country | xs:string | 0 |
| Phone | xs:string | 0 |
| Email | xs:string |  |
| Products | xs:string |  |
| Token | xs:string |  |
| ApplicationID | xs:string | 0 |
| Card_Number | xs:string | 0 |
| CCMonth | xs:string | 0 |
| CCYear | xs:string |  |
| TransactionSignature | xs:string | 0 |
| CVV2 | xs:string |  |
| CVV2Indicator | xs:string |  |
| AttemptVoid | xs:string |  |
| InitialRequest | xs:string |  |
| TransType | xs:string | 0 |
| PaymentType | xs:string | 0 |
| MerchantInvoiceNumber | xs:string | 0 |
| SendCustomerEmailReceipt | xs:string | 0 |
| SendMerchantEmailReceipt | xs:string |  |
| TransactionResponse |  |  |
| GatewayID | xs:unsignedInt |  |
| ReceiptNumber | xs:string |  |
| SalesOrderNumber | xs:unsignedByte |  |
| Name | xs:string |  |
| Token | xs:string |  |
| Date | xs:string |  |
| CardType | xs:string |  |
| Page | xs:unsignedInt |  |
| ApprovalCode | xs:string |  |
| Verbiage | xs:string |  |
| TotalAmount | xs:decimal |  |
| Products |  |  |
| product |  |  |
| code | xs:unsignedByte |  |
| description | xs:string |  |
| quantity | xs:unsignedByte |  |
| price | xs:decimal |  |
| subtotal | xs:decimal |  |
| flags |  |  |
| flag | xs:string |  |
| AVSResponseCode | xs:string |  |
| CVV2ResponseCode | xs:string |  |
| GUID | xs:string |  |
| ShippingName | xs:string |  |
| ShippingCompany | xs:string |  |
| ShippingAddress | xs:string |  |
| ShippingCity | xs:string |  |
| ShippingPostal | xs:string |  |
| ShippingProvince | xs:string |  |
| ShippingCountry | xs:string |  |
| ShippingEmail | xs:string |  |
| ShippingPhone | xs:string |  |
| MerchantIPAddress | xs:string |  |
| CustomerIP | xs:string |  |
| UnixTimeStamp | xs:string |  |
| ProcessorTime | xs:string |  |
| Card_Number | xs:string |  |
| ISOCurrency | xs:unsignedShort |  |
| Company | xs:string |  |
| Address | xs:string |  |
| City | xs:string |  |
| Postal | xs:unsignedShort |  |
| Province | xs:string |  |
| Country | xs:string |  |
| Phone | xs:string |  |
| Email | xs:string |  |
| TransType | xs:unsignedByte |  |
| CardType | xs:string |  |
| Language | xs:string |  |
| Amount | xs:decimal |  |

