<h6>Endpoint</h6>

<p id="endpoint"></p>
HTTP Method: **GET**

Returns validator uptime of the ledger.
<input class="md-input" placeholder="Enter Address" id="address" width="100"></input><br/><br/>
<button class="md-button" onclick="tryNow()">Try Now</button>
<script>
   document.getElementById("endpoint").innerHTML =`http://3.38.34.30:3836/validator/uptime/${document.getElementById("address").value || "boa1xzval2a3cdxv28n6slr62wlczslk3juvk7cu05qt3z55ty2rlfqfc6egsh2"}`
    function tryNow(){
        document.getElementById("showResult").innerHTML =""
        document.getElementById("endpoint").innerHTML =""
        fetch(`http://3.38.34.30:3836/validator/uptime/${document.getElementById("address").value || "boa1xzval2a3cdxv28n6slr62wlczslk3juvk7cu05qt3z55ty2rlfqfc6egsh2"}`).then((res) => {
            res.json().then((res) => {
                document.getElementById("showResult").innerHTML = JSON.stringify(res)
                document.getElementById("endpoint").innerHTML =`http://3.38.34.30:3836/validator/uptime/${document.getElementById("address").value || "boa1xzval2a3cdxv28n6slr62wlczslk3juvk7cu05qt3z55ty2rlfqfc6egsh2"}`
                })
        }).catch((err) => {
            console.log(err)
        })
    }
</script>
<p id="showResult"></p>
| Query String | Explanation    | Example                            |
| ------------ | -------------- | ---------------------------------- |
| address      | The address of the validator | boa1xzval2a3cdxv28n6slr62wlczslk3juvk7cu05qt3z55ty2rlfqfc6egsh2 |


Example Response JSON:<br/>
1187