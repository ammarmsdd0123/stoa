<h6>Endpoint</h6>

<p id="endpoint"></p>

HTTP Method: **GET**
Returns transactions of block.
<input class="md-input" placeholder="Enter Page" id="page" width="100"></input><br/>
<input class="md-input" placeholder="Enter Limit" id="limit"></input><br/>
<input class="md-input" placeholder="Enter Height" id="height"></input><br/><br/>
<button class="md-button" onclick="tryNow()">Try Now</button>
<script>
   document.getElementById("endpoint").innerHTML =`http://3.38.34.30:3836/block-transactions?page=${document.getElementById("page").value || "1"}&limit=${document.getElementById("limit").value || "10"}&height=${document.getElementById("height").value || "0"}`
    function tryNow(){
        document.getElementById("showResult").innerHTML =""
        document.getElementById("endpoint").innerHTML =""
        fetch(`http://3.38.34.30:3836/block-transactions?page=${document.getElementById("page").value || "1"}&limit=${document.getElementById("limit").value || "10"}&height=${document.getElementById("height").value || "0"}`).then((res) => {
            res.json().then((res) => {
                document.getElementById("showResult").innerHTML = JSON.stringify(res[0])
                document.getElementById("endpoint").innerHTML =`http://3.38.34.30:3836/holder_balance_history?page=${document.getElementById("page").value || "1"}&limit=${document.getElementById("limit").value || "10"}&height=${document.getElementById("height").value || "0"}`
                })
        }).catch((err) => {
            console.log(err)
        })
    }
</script>
<p id="showResult"></p>

| Query String | Explanation    | Example                            |
| ------------ | -------------- | ---------------------------------- |
| page      | page number | 1 |
| limit      | Number of records at a time | 10 |
| height      | block Height | 0 |

Example Response JSON:<br/>
[{"height":"0","tx_hash":"0x26866bb263593d024a92103646c48cf35a2b1bfcc49b087915b85db14a432b373569d56f576242354328a31bf0102a0a78cb806cf6e25d88d7981367833631b7","amount":"4880000000000000","fee":0,"size":368,"time":1609459200,"sender_address":null,"receiver":[{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"},{"type":0,"amount":610000000000000,"address":"boa1xzgenes5cf8xel37fz79gzs49v56znllk7jw7qscjwl5p6a9zxk8zaygm67"}],"full_count":2},{"height":"0","tx_hash":"0xeb5e0004d046422c84ddb7b9d54a0eba484a41b5179beda0b3dd7c54c3fca609437a9c8ef16b5bfc2335d9b258eb68908757e0f1a4c725752598aaa962924551","amount":"120000000000000","fee":0,"size":278,"time":1609459200,"sender_address":null,"receiver":[{"type":1,"amount":20000000000000,"address":"boa1xzval2a3cdxv28n6slr62wlczslk3juvk7cu05qt3z55ty2rlfqfc6egsh2"},{"type":1,"amount":20000000000000,"address":"boa1xzval3ah8z7ewhuzx6mywveyr79f24w49rdypwgurhjkr8z2ke2mycftv9n"},{"type":1,"amount":20000000000000,"address":"boa1xzval4nvru2ej9m0rptq7hatukkavemryvct4f8smyy3ky9ct5u0s8w6gfy"},{"type":1,"amount":20000000000000,"address":"boa1xrval5rzmma29zh4aqgv3mvcarhwa0w8rgthy3l9vaj3fywf9894ycmjkm8"},{"type":1,"amount":20000000000000,"address":"boa1xrval6hd8szdektyz69fnqjwqfejhu4rvrpwlahh9rhaazzpvs5g6lh34l5"},{"type":1,"amount":20000000000000,"address":"boa1xrval7gwhjz4k9raqukcnv2n4rl4fxt74m2y9eay6l5mqdf4gntnzhhscrh"}],"full_count":2}]