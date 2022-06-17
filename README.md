# hello world
## hello
sdkjfhdskjfh
**kdsjflksdjflk**
*sdkjfklsdjfs*
list:
 * jsdfhdjs
 * ksjkdsf
   * dsfjsdhfj

```javascript
$("#rndActBtn").click(function() { 
        let params = $("#filters").serialize();
        console.log(params);
        $.ajax({
            url: `https://www.boredapi.com/api/activity/?${params}`,
            success: function (response) {
                console.log(response);
                $("#activity").html(`
                    <p>Activity: ${response.activity}</p>
                    <p>Price: ${response.price}</p>
                    <p>Type: ${response.type}</p>
                `);
            }
        });
        $("#activity").show();
        $("#rndActBtn").html("Randimize Again")       
    });
```
