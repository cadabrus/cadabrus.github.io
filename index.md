<html>

<head></head>

<body>


<h1>amunra</h1>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>

<script>
  
          $.ajax({
            url: 'https://api.amunra.com/api/users/sign_in',
            data : '{"user" : {"email":"qwerty@gmail.com", "password":"Qwerty12345"}}',
            contentType : 'application/json',
            type : 'POST',
            xhrFields: {
                withCredentials: false
            },
            headers: {
                "Accept": "application/vnd.softswiss.v1+json"
            },
            success: function(data) {
                console.log(data);
            },
            error: function(data) {
                console.log(data);
            }
        })


</script>

</body>

</html>
