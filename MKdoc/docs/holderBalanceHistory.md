###### Endpoint

    https://boascan.io/holder_balance_history/boa1xrval5rzmma29zh4aqgv3mvcarhwa0w8rgthy3l9vaj3fywf9894ycmjkm8/?date=1609459200&filter=D

HTTP Method: **GET**
<br/>
<br/>
Returns average transaction fee between range (date - filter)

| Parameter | Explanation  | Example                              |
| --------- | ------------ | ------------------------------------ |
| date   | start date of the range of dates to look up. | 1609459200|
| --------- | ------------ | ------------------------------------ |
| address   | The address of BOA Holder | boa1xrval5rzmma29zh4aqgv3mvcarhwa0w8rgthy3l9vaj3fywf9894ycmjkm8|

Example Response JSON:<br/>
[{"address":"boa1xrval5rzmma29zh4aqgv3mvcarhwa0w8rgthy3l9vaj3fywf9894ycmjkm8","granularity":"D","time_stamp":1609459200,"balance":20000000000000,"block_height":0}]