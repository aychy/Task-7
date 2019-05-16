# Task-7

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Index Page</title>


    <script src="https://code.jquery.com/jquery-3.4.0.min.js"
            integrity="sha256-BJeo0qm959uMBGb65z40ejJYGSgR7REI4+CW1fNKwOg="
            crossorigin="anonymous"></script>

    <link rel="stylesheet"
          href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
          integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm"
          crossorigin="anonymous">
</head>
<body>


<div class="container-fluid">
    <b>Task 7</b>

    <div class="row mt-2">
        <div class="col-3">
            <form>
                <input type="text" class="form-control form-control-sm" id="inputText" placeholder="Type and Submit...">
                <input type="button" class="btn btn-sm mt-2 btn-primary" value="Submit" id="submitButton"/>
                <div id="task"></div>
            </form>
        </div>
    </div>
</div>
</body>
</html>

<script>
    $(document).ready(function () {
        $('#submitButton').on('click', function input() {
            var inputText = $('#inputText').val().trim();
            if(inputText != ""){
                $('div#task').append('<p>' + inputText + '</p>');
            }
        });
    });
</script>
