<!DOCTYPE HTML>
<html>

    <head>
        <title>Select a timer</title>
        <meta name="description" content="website description" />
        <meta name="keywords" content="website keywords, website keywords" />
        <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
        <link href="https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.3/css/select2.min.css" rel="stylesheet" />
        <link rel="stylesheet" type="text/css" href="../style/lowRated.css" title="style" />
        <link href="https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.3/css/select2.min.css" rel="stylesheet" />
        <link rel="stylesheet" type="text/css" href="../style/jquery.simple-dtpicker.css" />
        <script src="https://code.jquery.com/jquery-1.12.4.js"></script>
        <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
        <link rel="stylesheet" href="//code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css">
        <script src="https://cdnjs.cloudflare.com/ajax/libs/select2/4.0.3/js/select2.min.js"></script>
    </head>
    <body>


        <select class="taglist" id="typeselector" style="width: 100%">
            <option value=1>Deletion</option>
            <option value=2>Ban</option>
            <option value=3>Generic</option>
        </select>
        <hr/>
        <p id="results">
        </p>
        <div id="dspHolder" style="visibility:hidden; dsiplay: none;">
            <div class="displayblock" style="float: top;">
                <div class="caption">
                    When do I start the timer?
                </div>
                <div class="radio">  
                    <input id="yes" type="radio" name="noworlater" value="now"/>  
                    <label for="yes">Now</label>  
                    <input id="no" type="radio" name="noworlater" value="later"/>  
                    <label for="no">Later</label>  
                </div> 
            </div>
            <div id="midblock" class="displayblock" style=" display: none;
                                                           visibility: hidden;">
                <div class="caption">
                    Date and Time
                </div>
                <input type="text" id="datepicker">
                <div id="time" style="display: inline-block">

                    <select id="hours"style="width: 45%; display: inline-block">";

                        <option >00</option>
                        <option >01</option>
                        <option >02</option>
                        <option >03</option>
                        <option >04</option>
                        <option >05</option>
                        <option >06</option>
                        <option >07</option>
                        <option >08</option>
                        <option >09</option>
                        <option >10</option>
                        <option >11</option>
                        <option >12</option>
                        <option >13</option>
                        <option >14</option>
                        <option >15</option>
                        <option >16</option>
                        <option >17</option>
                        <option >18</option>
                        <option >19</option>
                        <option >20</option>
                        <option >21</option>
                        <option >22</option>
                        <option >23</option>
                    </select>
                    <select id="minutes" style="width: 45%; display:inline-block">";
                        <option >00</option>
                        <option >01</option>
                        <option >02</option>
                        <option >03</option>
                        <option >04</option>
                        <option >05</option>
                        <option >06</option>
                        <option >07</option>
                        <option >08</option>
                        <option >09</option>
                        <option >10</option>
                        <option >11</option>
                        <option >12</option>
                        <option >13</option>
                        <option >14</option>
                        <option >15</option>
                        <option >16</option>
                        <option >17</option>
                        <option >18</option>
                        <option >19</option>
                        <option >20</option>
                        <option >21</option>
                        <option >22</option>
                        <option >23</option>
                        <option >24</option>
                        <option >25</option>
                        <option >26</option>
                        <option >27</option>
                        <option >28</option>
                        <option >29</option>
                        <option >30</option>
                        <option >31</option>
                        <option >32</option>
                        <option >33</option>
                        <option >34</option>
                        <option >35</option>
                        <option >36</option>
                        <option >37</option>
                        <option >38</option>
                        <option >39</option>
                        <option >40</option>
                        <option >41</option>
                        <option >42</option>
                        <option >43</option>
                        <option >44</option>
                        <option >45</option>
                        <option >46</option>
                        <option >47</option>
                        <option >48</option>
                        <option >49</option>
                        <option >50</option>
                        <option >51</option>
                        <option >52</option>
                        <option >53</option>
                        <option >54</option>
                        <option >55</option>
                        <option >56</option>
                        <option >57</option>
                        <option >58</option>
                        <option >59</option>
                    </select>
                </div>
            </div>

            <div class="displayblock" id="duration" style="float: top;">
                <div class="caption">
                    Duration
                </div>
                <div class="radio">  
                    <input id="1hr" type="radio" name="duration" value="1h"/>  
                    <label for="1hr">One Hour</label>  
                    <input id="24hrs" type="radio" name="duration" value="24h"/>  
                    <label for="24hrs">24 Hours</label>  
                    <input id="48hrs" type="radio" name="duration" value="48h"/>  
                    <label for="48hrs">48 Hours</label>  
                    <input id="72hrs" type="radio" name="duration" value="72h"/>  
                    <label for="72hrs">72 Hours</label>  
                    <input id="1wk" type="radio" name="duration" value="1wk"/>  
                    <label for="1wk">One week</label>  
                    <input id="custom" type="radio" name="duration" value="custom"/>  
                    <label for="custom">Custom</label>  
                </div> 
            </div>

            <div id="endblock" class="displayblock" style=" display: none;
                                                           visibility: hidden;">
                <div class="caption">
                    When should it end?
                </div>
                <input type="text" id="customamount" style="width: 40%; display:inline-block">


                <select id="durationtype"style="width: 30%%; display: inline-block">";
                    <option value="hours">Hours</option>
                    <option value="days">Days</option>
                    <option value="weeks">Weeks</option>
                    <option value="months">Months</option>
                    <option value="years">Years</option>

                </select>


            </div>
            <div id="displayblock">
                <button type="button" class="button" id="submitBan">Get Timer Code</button>
            </div>
            <p id="banCode"></p>
        </div>
        <div id="genericHolder" style="visibility:hidden; dsiplay: none;">
            <div class="displayblock" style="float: top;">
                <div class="caption">
                    When do I start the timer?
                </div>
                Text to display: <input name="customTimerText" id="customTimerText" type="text" size="25" maxlength="150" value="This timer expires in">
                <div class="radio">  
                    <input id="genericYes" type="radio" name="noworlater" value="now"/>  
                    <label for="genericYes">Now</label>  
                    <input id="genericNo" type="radio" name="noworlater" value="later"/>  
                    <label for="genericNo">Later</label>  
                </div> 
            </div>
            <div id="genericMidblock" class="displayblock" style=" display: none;
                                                           visibility: hidden;">
                <div class="caption">
                    Date and Time
                </div>
                <input type="text" id="genericdatepicker">
                <div id="genericTime" style="display: inline-block">

                    <select id="genericHours"style="width: 45%; display: inline-block">";

                        <option >00</option>
                        <option >01</option>
                        <option >02</option>
                        <option >03</option>
                        <option >04</option>
                        <option >05</option>
                        <option >06</option>
                        <option >07</option>
                        <option >08</option>
                        <option >09</option>
                        <option >10</option>
                        <option >11</option>
                        <option >12</option>
                        <option >13</option>
                        <option >14</option>
                        <option >15</option>
                        <option >16</option>
                        <option >17</option>
                        <option >18</option>
                        <option >19</option>
                        <option >20</option>
                        <option >21</option>
                        <option >22</option>
                        <option >23</option>
                    </select>
                    <select id="genericMinutes" style="width: 45%; display:inline-block">";
                        <option >00</option>
                        <option >01</option>
                        <option >02</option>
                        <option >03</option>
                        <option >04</option>
                        <option >05</option>
                        <option >06</option>
                        <option >07</option>
                        <option >08</option>
                        <option >09</option>
                        <option >10</option>
                        <option >11</option>
                        <option >12</option>
                        <option >13</option>
                        <option >14</option>
                        <option >15</option>
                        <option >16</option>
                        <option >17</option>
                        <option >18</option>
                        <option >19</option>
                        <option >20</option>
                        <option >21</option>
                        <option >22</option>
                        <option >23</option>
                        <option >24</option>
                        <option >25</option>
                        <option >26</option>
                        <option >27</option>
                        <option >28</option>
                        <option >29</option>
                        <option >30</option>
                        <option >31</option>
                        <option >32</option>
                        <option >33</option>
                        <option >34</option>
                        <option >35</option>
                        <option >36</option>
                        <option >37</option>
                        <option >38</option>
                        <option >39</option>
                        <option >40</option>
                        <option >41</option>
                        <option >42</option>
                        <option >43</option>
                        <option >44</option>
                        <option >45</option>
                        <option >46</option>
                        <option >47</option>
                        <option >48</option>
                        <option >49</option>
                        <option >50</option>
                        <option >51</option>
                        <option >52</option>
                        <option >53</option>
                        <option >54</option>
                        <option >55</option>
                        <option >56</option>
                        <option >57</option>
                        <option >58</option>
                        <option >59</option>
                    </select>
                </div>
            </div>

            <div class="displayblock" id="duration" style="float: top;">
                <div class="caption">
                    Duration
                </div>
                <div class="radio">  
                    <input id="generic1hr" type="radio" name="duration" value="1h"/>  
                    <label for="generic1hr">One Hour</label>  
                    <input id="generic24hrs" type="radio" name="duration" value="24h"/>  
                    <label for="generic24hrs">24 Hours</label>  
                    <input id="generic48hrs" type="radio" name="duration" value="48h"/>  
                    <label for="generic48hrs">48 Hours</label>  
                    <input id="generic72hrs" type="radio" name="duration" value="72h"/>  
                    <label for="generic72hrs">72 Hours</label>  
                    <input id="generic1wk" type="radio" name="duration" value="1wk"/>  
                    <label for="generic1wk">One week</label>  
                    <input id="genericcustom" type="radio" name="duration" value="custom"/>  
                    <label for="genericcustom">Custom</label>  
                </div> 
            </div>

            <div id="genericEndblock" class="displayblock" style=" display: none;
                                                           visibility: hidden;">
                <div class="caption">
                    When should it end?
                </div>
                <input type="text" id="genericcustomamount" style="width: 40%; display:inline-block">


                <select id="genericdurationtype"style="width: 30%%; display: inline-block">";
                    <option value="hours">Hours</option>
                    <option value="days">Days</option>
                    <option value="weeks">Weeks</option>
                    <option value="months">Months</option>
                    <option value="years">Years</option>

                </select>


            </div>
            <div id="displayblock">
                <button type="button" class="button" id="genericsubmit">Get Timer Code</button>
            </div>
            <p id="genericcode"></p>
        </div>


        <script type="text/javascript">
            $('select').select2({
                placeholder: "Timer Type"
            });

            $(document).on('click', '.clicker', function(e)  { 
                var params="";  
                console.log("hurr");

                var type = $('.taglist').val().toString();
                if(type == '1'){
                    var code = "<p><strong>Post title:</strong><br><br><i>Staff Post - Deletion Vote</i></p><p><strong>Post content:</strong></p><p><i>Beginning deletion vote at "+this.value+".</i></p><p><i>[[iframe https://home.helenbot.com/tools/timer.html?time=" + (new Date().getTime() + 86400000)  +"&amp;type=del style=\"width: 500px; height: 250px; border: 0;\"]]</i></p><p><i>**If you are not the author and you want to rewrite this article, you may reply to this post asking for the opportunity to do so. Please obtain permission from the author (or the Rewrite Team if this article is older than 6 months) and make sure you copy the page source to your sandbox. Please do __not__ reply to this post for any other reason unless you are staff.**</i></p>"

                    document.getElementById('code').style.visibility = 'visible';
                    $("#code").html(code);
                }else{

                }
            });

            $(document).on('click', '#submitBan', function(){
                var startTime = Date.now();

                if(document.getElementById('no').checked ){
                    if(document.getElementById('datepicker').value != "" ){
                        startTime = Date.parse($("#datepicker").val());
                        startTime = startTime + (60 * 60 * 1000 * parseInt($("#hours").val()));
                        startTime = startTime + (60 * 1000 * parseInt($("#minutes").val()));
                    }
                }

                var endTime = startTime;

                if(document.getElementById('1hr').checked){
                    endTime = endTime + (60 * 60 * 1000);
                }else if(document.getElementById('24hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 24)
                }else if(document.getElementById('48hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 48)
                }else if(document.getElementById('72hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 72)
                }else if(document.getElementById('1wk').checked){
                    endTime = endTime + (60 * 60 * 1000 * 24 * 7)
                }else if(document.getElementById('custom').checked){
                    var durationtype = $("#customamount").val();
                    if(durationtype == 'hours'){
                        endTime = endTime + (60 * 60 * 1000 * parseInt($("#customamount")))
                    }else if (durationtype == 'days'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * parseInt($("#customamount")))
                    }else if (durationtype == 'weeks'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * 7 * parseInt($("#customamount")))
                    }else if (durationtype == 'months'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * 30 * parseInt($("#customamount")))
                    }else if (durationtype == 'years'){
                        endTime = endTime + (60 * 60 * 24 * 365 *  1000 * parseInt($("#customamount")))
                    }
                }








                var code = "<p><strong>Post title:</strong><br><br><i>Staff Post - Timer</i></p><p><strong>Post content:</strong></p><p>" +
                    "<i>Beginning deletion vote at -10.</i></p><p><i>[[iframe https://home.helenbot.com/tools/timer.html?time="
                    + parseFloat(startTime + (endTime - startTime))  +"&amp;type="+encodeURI($('#customTimerText').val())+
                    " style=\"width: 500px; height: 250px; border: 0;\"]]</i></p><p><i> **If this article is over a year old," +
                    " you are not the author, and you want to rewrite this article, request to do so in the [http://scp-wik" +
                    "i.wikidot.com/forum/t-14018096/rewrite-request-thread#post-4916192 Rewrite Request Thread]. Please request permission " +
                    "from the author and make sure you copy the page source to your sandbox. Do not reply to this post unless you are staff.**</i></p>"


                $('#banCode').html(code);

            });
            $(document).on('click', '#genericsubmit', function(){
                var startTime = Date.now();

                if(document.getElementById('genericNo').checked ){
                    if(document.getElementById('genericdatepicker').value != "" ){
                        startTime = Date.parse($("#genericdatepicker").val());
                        startTime = startTime + (60 * 60 * 1000 * parseInt($("#hours").val()));
                        startTime = startTime + (60 * 1000 * parseInt($("#minutes").val()));
                    }
                }

                var endTime = startTime;

                if(document.getElementById('generic1hr').checked){
                    endTime = endTime + (60 * 60 * 1000);
                }else if(document.getElementById('generic24hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 24)
                }else if(document.getElementById('generic48hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 48)
                }else if(document.getElementById('generic72hrs').checked){
                    endTime = endTime + (60 * 60 * 1000 * 72)
                }else if(document.getElementById('generic1wk').checked){
                    endTime = endTime + (60 * 60 * 1000 * 24 * 7)
                }else if(document.getElementById('genericcustom').checked){
                    var durationtype = $("#genericdurationtype").val();
                    if(durationtype == 'hours'){
                        endTime = endTime + (60 * 60 * 1000 * parseInt($("#genericcustomamount").val()))
                    }else if (durationtype == 'days'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * parseInt($("#genericcustomamount").val()))
                    }else if (durationtype == 'weeks'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * 7 * parseInt($("#genericcustomamount").val()))
                    }else if (durationtype == 'months'){
                        endTime = endTime + (60 * 60 * 1000 * 24 * 30 * parseInt($("#genericcustomamount").val()))
                    }else if (durationtype == 'years'){
                        endTime = endTime + (60 * 60 * 24 * 365 *  1000 * parseInt($("#genericcustomamount").val()))
                    }
                }








                var code = "<p><strong>Post title:</strong><br><br><i>Staff Post - Timer</i></p><p><strong>Post content:</strong></p><p>" +
                    "<i>Beginning deletion vote at -10.</i></p><p><i>[[iframe https://home.helenbot.com/tools/timer.html?time="
                    + parseFloat(startTime + (endTime - startTime))  +"&amp;type="+encodeURI($('#customTimerText').val())+
                    " style=\"width: 500px; height: 250px; border: 0;\"]]</i></p><p><i> **If this article is over a year old," +
                    " you are not the author, and you want to rewrite this article, request to do so in the [http://scp-wik" +
                    "i.wikidot.com/forum/t-14018096/rewrite-request-thread#post-4916192 Rewrite Request Thread]. Please request permission " +
                    "from the author and make sure you copy the page source to your sandbox. Do not reply to this post unless you are staff.**</i></p>"

//console.log(code);
                $('#genericcode').html(code);

            });
            jQuery(document).ready(function($){
               document.getElementById("results").style.visibility = 'visible';
                    document.getElementById("results").style.display = '';
                    document.getElementById("dspHolder").style.visibility = 'hidden';
                    document.getElementById("dspHolder").style.display = 'none';
                    $.ajax({type: "POST",
                            url: '/tools/getLowPages.php',
                            data: {tags: $('.taglist').val().toString()},
                            success: function(result){
                                $("#results").html(result);
                            }
                           });
            });


            document.getElementById("typeselector").onchange = function () { 
                var type = $('.taglist').val();
                if(type == "1" || type == "0"){
                    document.getElementById("results").style.visibility = 'visible';
                    document.getElementById("results").style.display = '';
                    
                    document.getElementById("dspHolder").style.visibility = 'hidden';
                    document.getElementById("dspHolder").style.display = 'none';
                    
                    document.getElementById("genericHolder").style.visibility = 'hidden';
                    document.getElementById("genericHolder").style.display = 'none';
                    
                    
                    $.ajax({type: "POST",
                            url: '/tools/getLowPages.php',
                            data: {tags: $('.taglist').val().toString()},
                            success: function(result){
                                $("#results").html(result);
                            }
                           });
                }else if(type == "2"){
                    document.getElementById("results").style.visibility = 'hidden';
                    document.getElementById("results").style.display = 'none';
                    
                    document.getElementById("genericHolder").style.visibility = 'hidden';
                    document.getElementById("genericHolder").style.display = 'none';
                    
                    
                    document.getElementById("dspHolder").style.visibility = 'visible';
                    document.getElementById("dspHolder").style.display = '';
                } else {
                     document.getElementById("genericHolder").style.visibility = 'visible';
                    document.getElementById("genericHolder").style.display = '';
                    
                    
                    document.getElementById("results").style.visibility = 'hidden';
                    document.getElementById("results").style.display = 'none';
                    document.getElementById("dspHolder").style.visibility = 'hidden';
                    document.getElementById("dspHolder").style.display = 'none';
                }
            };	

            document.getElementById("no").onclick = function(){
                document.getElementById("midblock").style.display = 'inline-block';
                document.getElementById("midblock").style.visibility = 'visible';
            }

            document.getElementById("yes").onclick = function(){
                document.getElementById("midblock").style.display = 'none';
                document.getElementById("midblock").style.visibility = 'hidden';
            }

            document.getElementById("custom").onclick = function(){
                document.getElementById("endblock").style.display = 'inline-block';
                document.getElementById("endblock").style.visibility = 'visible';
            }

            $('#1hr, #24hrs, #48hrs, #72hrs, #1wk').on('click', function(){
                document.getElementById("endblock").style.display = 'none';
                document.getElementById("endblock").style.visibility = 'hidden';
            });
            
             document.getElementById("genericNo").onclick = function(){
                document.getElementById("genericMidblock").style.display = 'inline-block';
                document.getElementById("genericMidblock").style.visibility = 'visible';
            }

            document.getElementById("genericYes").onclick = function(){
                document.getElementById("genericMidblock").style.display = 'none';
                document.getElementById("genericMidblock").style.visibility = 'hidden';
            }

            document.getElementById("genericcustom").onclick = function(){
                document.getElementById("genericEndblock").style.display = 'inline-block';
                document.getElementById("genericEndblock").style.visibility = 'visible';
            }

            $('#1hr, #24hrs, #48hrs, #72hrs, #1wk').on('click', function(){
                document.getElementById("genericEndblock").style.display = 'none';
                document.getElementById("genericEndblock").style.visibility = 'hidden';
            });

            $('select').select2({
                placeholder: 'Select an option'
            });

            $( function() {
                $( "#datepicker" ).datepicker();
            } );
            $( function() {
                $( "#genericdatepicker" ).datepicker();
            } );
        </script>
    </body>
</html>
