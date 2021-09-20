###### Endpoint

    https://boascan.io/wallet/transactions/history/boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67

HTTP Method: **GET**
<br/>
<br/>
Returns a set of transactions history of the addresses.

| Parameter | Explanation  | Example                              |
| --------- | ------------ | ------------------------------------ |
| address   | address to query. | boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67|

Example Response JSON:<br/>
[{"display_tx_type":"inbound","address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67","peer":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67","peer_count":0,"height":"0","time":1609459200,"tx_hash":"0x26866bb263593d024a92103646c48cf35a2b1bfcc49b087915b85db14a432b373569d56f576242354328a31bf0102a0a78cb806cf6e25d88d7981367833631b7","tx_type":"payment","amount":"4880000000000000","unlock_height":"1","unlock_time":1609459800}]