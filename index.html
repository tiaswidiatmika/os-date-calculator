<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="https://code.jquery.com/jquery-3.5.1.min.js" integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>
    
    <link rel="stylesheet" type="text/css" href="http://ajax.googleapis.com/ajax/libs/jqueryui/1.8.23/themes/south-street/jquery-ui.css"> 
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.8.3/jquery.min.js"></script> 
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jqueryui/1.8.23/jquery-ui.min.js"></script>
    <script src="https://momentjs.com/downloads/moment.js"></script>
    <script src="js/cleave.js-1.6.0/dist/cleave.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body{ 
            background-color: #222; 
            color: #ccc;
            font-family: 'Open Sans';
            font-weight: 400;
            font-stretch: normal;
            font-size: 13.3333px;
        } 

        #days_here{
            width: 40px;
        }        

        p{ 
        color: #ccc; 
        } 
        input { 
            background-color: #333333; 
            border: 1px solid #555; 
            border-radius: 5%;
            font: 400 13.3333px Helvetica;
            color: #e6e6e6;
            font-style: normal;
            font-variant-ligatures: normal;
            font-variant-caps: normal;
            font-variant-numeric: normal;
            font-variant-east-asian: normal;
            font-weight: 400;
            font-stretch: normal;
            font-size: 13.3333px;
            line-height: normal;
            font-family: Helvetica;
        } 
        .change { 
            cursor: pointer; 
             
            width: 20px; 
            text-align: center; 
            padding: 5px; 
            margin-left: 8px; 
        } 
        .dark{ 
            
        } 
    </style>
    
</head>
<body>
    <h4><p>Input date in either arrival date, visa validity, or in any extension expiry date</p></h4>
    <h4><p>Input must be inserted in format "DD/MM/YYYY" or "DD-MM-YYYY"</p></h4>
    
    <table>
        <tr>
            <td>visa length:</td>
            <td><input type="text" name="" id="visa_length"></td>
        </tr>
        <tr>
            <td>arrival date:</td>
            <td><input type="text" name="" id="arrival_date" class="date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
        <tr><td></td></tr>
        <tr>
            <td>visa validity:</td>
            <td><input type="text" name="" id="valid_until" class="cls_input date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
    </table>
    <br>
    <table>
        <tr>
            <td>first ext expired on:</td>
            <td><input type="text" name="" id="first_ext" class="date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
        <tr>
            <td>second ext expired on:</td>
            <td><input type="text" name="" id="second_ext" class="date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
        <tr>
            <td>third ext expired on:</td>
            <td><input type="text" name="" id="third_ext" class="date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
        <tr>
            <td>fourth ext expired on:</td>
            <td><input type="text" name="" id="fourth_ext" class="date_format" placeholder="DD/MM/YYYY"></td>
        </tr>
    </table>
    <h4>Or <b><strong>paste</strong></b>  days after stay permit expires</h4>
   <!-- <h4>Or <strong>paste</strong></h4><h4> days after stay permit expires</h4> -->
   <input type="text" name="" id="permit_dies" class="date_format" placeholder="DD/MM/YYYY"> is <span id="overstays">... </span> day(s) over
   <h4>Or <b><strong>insert</strong></b> how many days been staying</h4>
   <input type="text" name="" id="days_here"> days. <span id="get_arrival_date"></span>

    
</body>
<script>
    $(document).ready(function () {
        
        $('#permit_dies').val("Paste one of date shown above");
        
        $('.date_format').toArray().forEach(function(field){
            new Cleave(field, {
                date: true,
                datePattern: ['d','m', 'Y']
            });
        });

        $('#permit_dies').focus(function (e) { 
            e.preventDefault();
            $(this).val("");
        });

        var visa_length;
        var arrival_date, valid_until, first_ext_validity, second_ext_validity, third_ext_validity, fourth_ext_validity;
        function isvaliddate(str_date){
            str_date
        }
        
        function isNotValid(value){
            if (! $('#visa_length').val()) {
                alert('visa length is empty');
                $('#visa_length').focus();
                // $('.date_format').val('');
                return true;
            }
            if (! moment(value).isValid()) {
                alert('invalid date');
                return true;
            }
            visa_length = +$('#visa_length').val()-1;
            return false;
        }
        //  ARRIVAL DATE INPUT
        $('#arrival_date').change( function (e) {
            e.preventDefault();
            arrival_date = String ($(this).val());
            arrival_date = moment(arrival_date, "DD/MM/YYYY");
            if (isNotValid(arrival_date)) {
                return;
            }
            $('#valid_until').val(moment(arrival_date).add(visa_length, 'days').format('DD/MM/YYYY'));
            $('#first_ext').val(moment(arrival_date).add(visa_length+30, 'days').format('DD/MM/YYYY'));
            $('#second_ext').val(moment(arrival_date).add(visa_length+60, 'days').format('DD/MM/YYYY'));
            $('#third_ext').val(moment(arrival_date).add(visa_length+90, 'days').format('DD/MM/YYYY'));
            $('#fourth_ext').val(moment(arrival_date).add(visa_length+120, 'days').format('DD/MM/YYYY'));
        });

        // VISA LENGTH INPUT
        $('#visa_length').change(function (e) { 
            e.preventDefault();
            visa_validity = $(this).val()-1;
            
            // check if arrival date is inserted
            arrival_date = String ($('#arrival_date').val());
            arrival_date = moment(arrival_date, "DD/MM/YYYY");
            if (arrival_date.isValid()){
                $('#arrival_date').trigger('change');
                return;
            }

            // check if visa validity is inserted
            valid_until = String ($('#valid_until').val());
            valid_until = moment(valid_until, "DD/MM/YYYY");
            if (valid_until.isValid()){
                $('#valid_until').trigger('change');
                return;
            }

            // check if first expired date is inserted
            first_ext_validity = String ($('#first_ext').val());
            first_ext_validity = moment(first_ext_validity, "DD/MM/YYYY");
            if (first_ext_validity.isValid()){
                $('#first_ext').trigger('change');
                return;
            }

            // check if second expired date is inserted
            second_ext_validity = String ($('#second_ext').val());
            second_ext_validity = moment(second_ext_validity, "DD/MM/YYYY");
            if (second_ext_validity.isValid()){
                $('#second_ext').trigger('change');
                return;
            }
            // check if third expired date is inserted
            third_ext_validity = String ($('#third_ext').val());
            third_ext_validity = moment(third_ext_validity, "DD/MM/YYYY");
            if (third_ext_validity.isValid()){
                $('#third_ext').trigger('change');
                return;
            }

            // check if fourth expired date is inserted
            fourth_ext_validity = String ($('#fourth_ext').val());
            fourth_ext_validity = moment(fourth_ext_validity, "DD/MM/YYYY");
            if (fourth_ext_validity.isValid()){
                $('#fourth_ext').trigger('change');
                return;
            }

            
        });

        
        //VISA VALIDITY INPUT
        $('#valid_until').change(function (e) { 
            e.preventDefault();
            arrival_date = moment(String($(this).val()), "DD/MM/YYYY");
            if (isNotValid(arrival_date)){
                return
            }
            $('#arrival_date').val(moment(arrival_date).subtract(visa_length, 'day').format('DD/MM/YYYY'));
            // $('#arrival_date').val( moment(arrival_date, "DD/MM/YYYY")).subtract(visa_validity, 'day').format('DD/MM/YYYY'));
            $('#first_ext').val(moment(arrival_date).add(30, 'day').format('DD/MM/YYYY'));
            $('#second_ext').val(moment(arrival_date).add(60, 'days').format('DD/MM/YYYY'));
            $('#third_ext').val(moment(arrival_date).add(90, 'days').format('DD/MM/YYYY'));
            $('#fourth_ext').val(moment(arrival_date).add(120, 'days').format('DD/MM/YYYY'));
            
        });

        // FIRST EXT INPUT
        $('#first_ext').change(function (e) { 
            e.preventDefault();
            first_ext_validity = moment($(this).val(), 'DD/MM/YYYY');
            if (isNotValid(first_ext_validity)) return;
            valid_until = moment(first_ext_validity, 'DD/MM/YYYY').subtract(30, 'days');
            $('#valid_until').val(moment(valid_until).format('DD/MM/YYYY'));
            $('#arrival_date').val(moment(first_ext_validity, 'DD/MM/YYYY').subtract(visa_length+30, 'days').format('DD/MM/YYYY'));
            $('#second_ext').val(moment(first_ext_validity, 'DD/MM/YYYY').add(30, 'days').format('DD/MM/YYYY'));
            $('#third_ext').val(moment(first_ext_validity, 'DD/MM/YYYY').add(60, 'days').format('DD/MM/YYYY'));
            $('#fourth_ext').val(moment(first_ext_validity, 'DD/MM/YYYY').add(90, 'days').format('DD/MM/YYYY'));
        });
        
        // SECOND EXT INPUT
        $('#second_ext').change(function (e) { 
            e.preventDefault();
            second_ext_validity = String($(this).val());
            second_ext_validity = moment(second_ext_validity, 'DD/MM/YYYY');
            if(isNotValid(second_ext_validity)) return;
            first_ext_validity = moment(second_ext_validity).subtract(30, 'days');

            $('#first_ext').val(first_ext_validity.format('DD/MM/YYYY'));
            $('#arrival_date').val(first_ext_validity.subtract(visa_length+30, 'days').format('DD/MM/YYYY'));
            $('#valid_until').val(first_ext_validity.add(visa_length, 'days').format('DD/MM/YYYY'));
            $('#third_ext').val(second_ext_validity.add(30, 'days').format('DD/MM/YYYY'));
            $('#fourth_ext').val(second_ext_validity.add(30, 'days').format('DD/MM/YYYY'));

        });

        // THIRD EXT INPUT

        $('#third_ext').change(function (e) { 
            e.preventDefault();
            
            third_ext_validity = moment($(this).val(), 'DD/MM/YYYY');
            if(isNotValid(third_ext_validity)) return;
            second_ext_validity = moment(third_ext_validity).subtract(30, 'days');
            $('#second_ext').val(second_ext_validity.format('DD/MM/YYYY'));
            $('#first_ext').val(second_ext_validity.subtract(30, 'days').format('DD/MM/YYYY'));
            $('#arrival_date').val(second_ext_validity.subtract(visa_length+30, 'days').format('DD/MM/YYYY'));
            $('#valid_until').val(second_ext_validity.add(visa_length, 'days').format('DD/MM/YYYY'));
            
            
            $('#fourth_ext').val(third_ext_validity.add(30, 'days').format('DD/MM/YYYY'));
        });

        // FOURTH EXT INPUT
        $('#fourth_ext').change(function (e) { 
            e.preventDefault();
            fourth_ext_validity = moment(String($(this).val()),'DD/MM/YYYY');
            if(isNotValid(fourth_ext_validity)) return;
            $('#third_ext').val(fourth_ext_validity.subtract(30, 'days').format('DD/MM/YYYY'));
            $('#second_ext').val(fourth_ext_validity.subtract(30, 'days').format('DD/MM/YYYY'));
            $('#first_ext').val(fourth_ext_validity.subtract(30, 'days').format('DD/MM/YYYY'));
            $('#valid_until').val(fourth_ext_validity.subtract(30, 'days').format('DD/MM/YYYY'));
            $('#arrival_date').val(fourth_ext_validity.subtract(visa_length, 'days').format('DD/MM/YYYY'));
        });

        $('#permit_dies').change(function (e) { 
            e.preventDefault();
            var permit_dies = moment( $(this).val(), "DD/MM/YYYY" ).format("DD/MM/YYYY");
            var os = moment().diff(moment($('#permit_dies').val(), "DD/MM/YYYY"),'days');
            if (isNaN(os)){
                $(this).val("Invalid date");
                $(this).select();
                $('#overstays').html('... ');
            } else {
                $('#overstays').html(os);
            }
                   
        }); 

        $('#days_here').change(function (e) { 
            e.preventDefault();
            
            arrival_date = moment().subtract($(this).val(), 'days').format("DD/MM/YYYY");
            $('#arrival_date').val(arrival_date).trigger('change');

        });

    });
</script>
</html>
