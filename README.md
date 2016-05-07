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
Sample page: http://www.babygroup.co.za/Special-Pages/MenuContainer.aspx

You can also pass querystring parameters to the embed endpoint to control
* which banner leads the menu
* how far left the banner can be indented

For example, in the ajax call above, the url: https://api.ebuntu.co/embed?lead=babygroup&offset=60 will position the BabyGroup banner first and pad the menu with 60px from the edge of screen
