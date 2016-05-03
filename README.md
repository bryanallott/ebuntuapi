# ebuntuapi

```
<div id="_ebuntu" style="top:0;left:0;"></div>

<script>
      $j(document).ready(function(){ 
        $j.ajax({cache:false, 
                 async:true, 
                 url:'https://api.ebuntu.co/embed', 
                 success: function(data) { 
                  $j('#_ebuntu').html(data);
                  $j('#_ebuntu').insertBefore('.topbar');
                   }
        }); 
      });
</script>
```
