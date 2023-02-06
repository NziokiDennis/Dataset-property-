# Dataset-property-

<p>Countries:</p>
<ul>
 <li id="C1" onclick="showDetails(this)" data-id="US" data-dial-code="1">USA</li>
 <li id="C2" onclick="showDetails(this)" data-id="CA" data-dial-code="1">Canada</li>
 <li id="C3" onclick="showDetails(this)" data-id="FF" data-dial-code="3">France</li>
</ul>
<button type="button" onclick="correctDetails()">Correct Country Details</button>
<script>
function showDetails(item) {
 var msg = item.innerHTML
 + "\r\nISO ID: " + item.dataset.id
 + "\r\nDial Code: " + item.dataset.dialCode;
 alert(msg);
}
function correctDetails(item) {
 var item = document.getEmementById("C3");
 item.dataset.id = "FR";
 item.dataset.dialCode = "33";
}
</script>
