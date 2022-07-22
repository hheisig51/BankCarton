# BankCarton

This is a sandbox for messing around with Github features!

<html>
<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>

<script src="/mrjsontable/scripts/mrjsontable.js"></script>

<link href="/mrjsontable/css/mrjsontable.css" rel="stylesheet" />

<div id="mydiv"></div>

<script>
    $(function () {
        $("#mydiv").mrjsontable({
            columns: [
                {
                    heading: "Can be any text for the heading of this column",
                    data: "json_data_field_name", // see how this links to the json object further down
                    type: "string", // can be string, int, float, datetime
                    sortable: true, // is the field sortable (optional defaults to false)
                    starthidden: true // should the field be hidden when loaded (optional defaults to false)
                },
            ],
            data: [
                {
                    yourdata: yourvalue,
                    json_data_field_name: value //in this example the first column is looking for this field specified in the data property,
                    name: name_value // in this example the second column is looking for this value
                },
            ],
        });
    });
</script>

</html>
