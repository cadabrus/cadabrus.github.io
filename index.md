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
                withCredentials: true
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
        });


var http_request;
http_request = new XMLHTTPRequest();
http_request.onreadystatechange = function () { /* .. */ };
http_request.open("POST", "https://api.amunra.com/api/users/sign_in");
http_request.withCredentials = true;
http_request.setRequestHeader("Content-Type", "application/json");
http_request.send({ 'request': "authentication token" });


</script>

</body>

</html>
