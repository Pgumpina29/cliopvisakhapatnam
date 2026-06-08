<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Electrical OP</title>

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Montserrat',sans-serif;
}

body{
    background:linear-gradient(135deg,#0f172a,#1e3a8a);
    min-height:100vh;
    padding:30px;
}

.container{
    max-width:1200px;
    margin:auto;
    background:#fff;
    border-radius:15px;
    overflow:hidden;
    box-shadow:0 10px 30px rgba(0,0,0,.25);
}

.header{
    background:linear-gradient(135deg,#003566,#00509d);
    color:#fff;
    text-align:center;
    padding:25px;
}

.header h1{
    font-size:32px;
    margin-bottom:5px;
}

.header h2{
    font-size:18px;
    font-weight:500;
}

.form-section{
    padding:30px;
}

.form-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.field{
    display:flex;
    flex-direction:column;
}

label{
    margin-bottom:8px;
    font-weight:600;
    color:#003566;
}

input,
select,
textarea{
    padding:12px;
    border:1px solid #d1d5db;
    border-radius:8px;
    font-size:14px;
}

input:focus,
select:focus,
textarea:focus{
    outline:none;
    border-color:#00509d;
}

.employee-box{
    margin-top:20px;
    background:#eef6ff;
    border-left:5px solid #00509d;
    padding:15px;
    border-radius:8px;
}

.employee-name{
    font-size:18px;
    font-weight:700;
    color:#003566;
}

.dynamic-section{
    margin-top:25px;
    background:#f8fafc;
    border:1px solid #e5e7eb;
    border-radius:10px;
    padding:20px;
}

.section-title{
    font-size:20px;
    color:#003566;
    margin-bottom:20px;
    font-weight:700;
}

.submit-btn{
    margin-top:25px;
    background:#00509d;
    color:#fff;
    border:none;
    padding:14px 40px;
    border-radius:8px;
    font-size:16px;
    font-weight:600;
    cursor:pointer;
}

.submit-btn:hover{
    background:#003566;
}

/* ===== MOBILE RESPONSIVE ===== */
@media screen and (max-width:768px){
body{padding:10px;}
.container{width:100%;border-radius:10px;}
.header{padding:15px;}
.header h1{font-size:22px;line-height:1.3;}
.header h2{font-size:14px;}
.form-section{padding:15px;}
.form-grid{grid-template-columns:1fr !important;gap:15px;}
input,select,textarea{width:100%;font-size:16px;}
.employee-name{font-size:16px;}
.dynamic-section{padding:15px;}
.submit-btn{width:100%;}
.field[style*="grid-column"]{grid-column:auto !important;}
}
@media screen and (max-width:480px){
.header h1{font-size:18px;}
.header h2{font-size:12px;}
.section-title{font-size:16px;}
}

</style>
</head>
<body>

<div class="container">

    <div class="header">
        <h1>ELECTRIC-OPERATIONS</h1>
        <h2>Visakhapatnam - South Coast Railway</h2>
    </div>

    <div class="form-section">

        <div class="form-grid">

            <div class="field">
                <label>CMS ID</label>
                <select id="cmsid" onchange="showName()">
                    <option value="">Select CMS ID</option>
                    <option value="VSKP0074">VSKP0074</option>
<option value="VSKP0014">VSKP0014</option>
<option value="VSKP0019">VSKP0019</option>
<option value="VSKP0042">VSKP0042</option>
<option value="VSKP0080">VSKP0080</option>
<option value="VSKP0058">VSKP0058</option>
<option value="VSKP0048">VSKP0048</option>
<option value="VSKP0085">VSKP0085</option>
<option value="VSKP0050">VSKP0050</option>
<option value="VSKP0078">VSKP0078</option>
<option value="VSKP0018">VSKP0018</option>
<option value="VSKP0006">VSKP0006</option>
<option value="VSKP0084">VSKP0084</option>
<option value="VSKP0037">VSKP0037</option>
<option value="VSKP0028">VSKP0028</option>
<option value="VSKP0057">VSKP0057</option>
<option value="VSKP0033">VSKP0033</option>
<option value="VSKP0060">VSKP0060</option>
<option value="VSKP0073">VSKP0073</option>
<option value="VSKP0043">VSKP0043</option>
<option value="VSKP0051">VSKP0051</option>
<option value="VSKP0072">VSKP0072</option>
<option value="VSKP0069">VSKP0069</option>
<option value="VSKP0009">VSKP0009</option>
<option value="VSKP0079">VSKP0079</option>
<option value="VSKP0064">VSKP0064</option>
<option value="VSKP0066">VSKP0066</option>
<option value="VSKP0053">VSKP0053</option>
<option value="VSKP0071">VSKP0071</option>
<option value="VSKP0012">VSKP0012</option>
<option value="VSKP0047">VSKP0047</option>
<option value="VSKP0044">VSKP0044</option>
<option value="VSKP0067">VSKP0067</option>
<option value="VSKP0039">VSKP0039</option>
<option value="VSKP0021">VSKP0021</option>
<option value="VSKP0063">VSKP0063</option>
<option value="VSKP0003">VSKP0003</option>
<option value="VSKP0031">VSKP0031</option>
<option value="VSKP0038">VSKP0038</option>
<option value="VSKP0040">VSKP0040</option>
<option value="VSKP0049">VSKP0049</option>
<option value="VSKP0075">VSKP0075</option>
<option value="VSKP0052">VSKP0052</option>
<option value="VSKP0055">VSKP0055</option>
<option value="VSKP0061">VSKP0061</option>
<option value="VSKP0046">VSKP0046</option>
<option value="VSKP0099">VSKP0099</option>
<option value="VSKP0001">VSKP0001</option>
<option value="VSKP0054">VSKP0054</option>
<option value="VSKP0002">VSKP0002</option>
<option value="VSKP0022">VSKP0022</option>
<option value="VSKP0062">VSKP0062</option>
<option value="VSKP0065">VSKP0065</option>
<option value="VSKP0010">VSKP0010</option>
<option value="VSKP0045">VSKP0045</option>











                </select>
            </div>

            <div class="field">
                <label>Type of Duty</label>
                <select id="dutyType" onchange="loadForm()">
                    <option value="">Select Duty</option>
                    <option value="RS Valve Test">RS Valve Test</option>
                    <option value="Counselling">Counselling</option>
                    <option value="BA Ambush">BA Ambush</option>
                    <option value="Mobile Ambush">Mobile Ambush</option>
                    <option value="Speed Gun">Speed Gun</option>
                    <option value="Shunting Ambush">Shunting Ambush</option>
                    <option value="Casuality">Casuality</option>
                </select>
            </div>

        </div>

        <div class="employee-box">
            <strong>Employee Name</strong>
            <div id="empName" class="employee-name">Not Selected</div>
        </div>

        <div id="dynamicFields"></div>

        <button type="button" class="submit-btn">Submit</button>

    </div>

</div>

<script>

const employees = {
   "VSKP0074":"SIMMA CHINNARAO",
"VSKP0014":"D.V.LPRASAD",
"VSKP0019":"DEBABRATA MANNA",
"VSKP0042":"G PRAKASA RAO",
"VSKP0080":"E.Venkateswarlu",
"VSKP0058":"TEMBA NARAYANA RAO",
"VSKP0048":"T V V PRASAD",
"VSKP0085":"Tatipudi Govinda Rao",
"VSKP0050":"S P RAVI KUMAR",
"VSKP0078":"M.Srinivasa Rao",
"VSKP0018":"M.KURUKSHETRA",
"VSKP0006":"P.V.APPARAO",
"VSKP0084":"A.Uday Kumar Dath",
"VSKP0037":"T. RAMA MOHANA  RAO",
"VSKP0028":"A.N.NAIDU",
"VSKP0057":"N ESWRA RAO",
"VSKP0033":"SANGANNA",
"VSKP0060":"G. LEELA KRISHNA",
"VSKP0073":"p govind achari",
"VSKP0043":"P PRAKASHA RAO",
"VSKP0051":"CH.NARASIMHA ACHARI",
"VSKP0072":"V NAGESH KUMAR",
"VSKP0069":"R.RAVIKUMAR",
"VSKP0009":"K.S.RAO",
"VSKP0079":"Y.Rama Krishna",
"VSKP0064":"CH SRIHARI",
"VSKP0066":"M V RAMANA",
"VSKP0053":"G RAMA MOHAN",
"VSKP0071":"LABUDU BHOJA RAJU",
"VSKP0012":"M.APPALANAIDU",
"VSKP0047":"K ANANTHA RAO",
"VSKP0044":"P.P.SANKAR",
"VSKP0067":"CH.SRIDHARARAO",
"VSKP0039":"B MANI BABU",
"VSKP0021":"Dhananjaya Sirugudi",
"VSKP0063":"Y  RAMESH BABU",
"VSKP0003":"K SHAJI",
"VSKP0031":"M.P REDDY",
"VSKP0038":"TRP VERMA",
"VSKP0040":"M RAVI KUMAR",
"VSKP0049":"G KRISHNA",
"VSKP0075":"T NARAYANA",
"VSKP0052":"G CHINNAJI",
"VSKP0055":"R M S RAO",
"VSKP0061":"Y.Mohana Babu",
"VSKP0046":"D ANANDA RAO",
"VSKP0099":"R.V.S.S.RAO",
"VSKP0001":"H.DAS",
"VSKP0054":"M A V S  NARAYANA",
"VSKP0002":"CHT SWAMY",
"VSKP0022":"D.V.ANNAJI RAO",
"VSKP0062":"S BANGARU BABU",
"VSKP0065":"G.JAGANNADHAM",
"VSKP0010":"L.K.PANDA",
"VSKP0045":"PILLALA SRINIVASA RAO"

};

function showName(){
    let id = document.getElementById("cmsid").value;
    document.getElementById("empName").innerHTML =
        employees[id] || "Not Found";
}

function loadForm(){

let duty = document.getElementById("dutyType").value;
let html = "";

if(duty==="RS Valve Test"){

html = `
<div class="dynamic-section">
<div class="section-title">RS Valve Test Details</div>

<div class="form-grid">
<div class="field">
<label>Date</label>
<input type="date">
</div>

<div class="field">
<label>CMS ID</label>
<input type="text">
</div>

<div class="field">
<label>Train No</label>
<input type="text">
</div>

<div class="field">
<label>Time</label>
<input type="time">
</div>

<div class="field">
<label>Location</label>
<input type="text">
</div>
</div>
</div>`;
}

else if(duty==="Counselling"){

html = `
<div class="dynamic-section">
<div class="section-title">Counselling Details</div>

<div class="form-grid">

<div class="field">
<label>Date</label>
<input type="date">
</div>

<div class="field">
<label>No of LP</label>
<input type="number">
</div>

<div class="field">
<label>No of ALP</label>
<input type="number">
</div>

<div class="field" style="grid-column:1/-1;">
<label>LP / ALP IDs</label>
<textarea rows="4" placeholder="VSKP1234, VSKP2345"></textarea>
</div>

</div>
</div>`;
}

else if(duty==="BA Ambush"){

html = `
<div class="dynamic-section">
<div class="section-title">BA Ambush Details</div>

<div class="form-grid">
<div class="field">
<label>Date</label>
<input type="date">
</div>

<div class="field">
<label>Station / Place</label>
<input type="text">
</div>

<div class="field">
<label>No of Staff Done</label>
<input type="number">
</div>
</div>
</div>`;
}

else if(duty==="Mobile Ambush"){

html = `
<div class="dynamic-section">
<div class="section-title">Mobile Ambush Details</div>

<div class="form-grid">
<div class="field">
<label>Date</label>
<input type="date">
</div>

<div class="field">
<label>Station / Place</label>
<input type="text">
</div>

<div class="field">
<label>No of Staff</label>
<input type="number">
</div>
</div>
</div>`;
}

else if(duty==="Speed Gun"){

html = `
<div class="dynamic-section">
<div class="section-title">Speed Gun Details</div>

<div class="form-grid">

<div class="field">
<label>Section</label>
<input type="text">
</div>

<div class="field">
<label>KM No</label>
<input type="text">
</div>

<div class="field">
<label>OHE Mast No</label>
<input type="text">
</div>

<div class="field">
<label>From Time</label>
<input type="time">
</div>

<div class="field">
<label>To Time</label>
<input type="time">
</div>

<div class="field">
<label>No of Trains</label>
<input type="number">
</div>

<div class="field" style="grid-column:1/-1;">
<label>Remarks</label>
<textarea rows="3"></textarea>
</div>

</div>
</div>`;
}

else if(duty==="Shunting Ambush"){

html = `
<div class="dynamic-section">
<div class="section-title">Shunting Ambush Details</div>

<div class="form-grid">

<div class="field">
<label>Station Name</label>
<input type="text">
</div>

<div class="field">
<label>From Time</label>
<input type="time">
</div>

<div class="field">
<label>To Time</label>
<input type="time">
</div>

<div class="field">
<label>No of Trains / Shunts Observed</label>
<input type="number">
</div>

</div>
</div>`;
}

else if(duty==="Casuality"){

html = `
<div class="dynamic-section">
<div class="section-title">Casuality Details</div>

<div class="form-grid">

<div class="field">
<label>Date</label>
<input type="date">
</div>

<div class="field">
<label>Type of Casuality</label>
<select>
<option value="">Select Type</option>
<option>LAP</option>
<option>CL</option>
<option>RMC</option>
<option>PMC</option>
<option>SCL</option>
<option>Others</option>
</select>
</div>

<div class="field">
<label>From Date</label>
<input type="date">
</div>

<div class="field">
<label>To Date</label>
<input type="date">
</div>

<div class="field">
<label>No. of Days</label>
<input type="number">
</div>

<div class="field" style="grid-column:1/-1;">
<label>Remarks</label>
<textarea rows="4"></textarea>
</div>

</div>
</div>`;
}

document.getElementById("dynamicFields").innerHTML = html;
}
</script>

</body>
</html>

