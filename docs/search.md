###### Endpoint

    https://boascan.io//search/hash/0xE8DBDEB515CF835F515355045EC1AF6CB141F9690FB85B01294FE1985E84A37BD78F0100AF5E1847A881D04DA033E1A84C903F81BD05E52CADC534518F4011FF

HTTP Method: **GET**
<br/>
<br/>
Returns block as true if hash matches block hash or transaction as true if hash matches tx_hash 
* otherwise it will respond with no data found.

| Parameter | Explanation  | Example                              |
| --------- | ------------ | ------------------------------------ |
| hash   | hash of block or transaction | 0xE8DBDEB515CF835F515355045EC1AF6CB141F9690FB85B01294FE1985E84A37BD78F0100AF5E1847A881D04DA033E1A84C903F81BD05E52CADC534518F4011FF|

Example Response JSON:<br/>
{"block":1,"transaction":0}