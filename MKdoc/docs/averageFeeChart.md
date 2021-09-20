###### Endpoint

    https://boascan.io/average_fee_chart?filter=D&date=1609459200

HTTP Method: **GET**

Returns average transaction fee between range (date - filter)

| Query String | Explanation    | Example                            |
| ------------ | -------------- | ---------------------------------- |
| date         | start date of the range of dates to look up | 1609459200 |

Example Response JSON:<br/>
[{"height":0,"granularity":"D","time_stamp":1609459200,"average_tx_fee":0,"total_tx_fee":0,"total_payload_fee":0,"total_fee":0}]
