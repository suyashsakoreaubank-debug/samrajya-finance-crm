<!DOCTYPE html>
<html lang="mr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SAMRAJYA FINANCE CRM</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#f2f5fa;color:#172033}
header{background:#10284b;color:white;padding:20px}
header h1{margin:0;font-size:24px}
header p{margin:6px 0 0;color:#d5e4ff}
.container{max-width:1100px;margin:25px auto;padding:15px}
.card{background:white;padding:22px;border-radius:12px;box-shadow:0 3px 14px #00000010;margin-bottom:20px}
input,select,button{padding:12px;margin:6px 0;border-radius:7px;border:1px solid #ccd5e3;width:100%;font-size:15px}
button{background:#123d73;color:white;border:0;cursor:pointer;font-weight:bold}
button:hover{background:#19569c}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:15px}
.stat{background:white;padding:20px;border-radius:10px;border-left:5px solid #164b87}
.stat strong{font-size:27px;display:block;margin-top:8px}
.small{color:#667085;font-size:13px}
#dashboard{display:none}
</style>
</head>
<body>
<header>
  <h1>🏦 SAMRAJYA FINANCE</h1>
  <p>Online CRM | Loan Lead Management System</p>
</header>

<div class="container">
  <section class="card" id="login">
    <h2>Admin / Team Login</h2>
    <p class="small">आपल्या अधिकृत खात्याने Login करा.</p>
    <form id="loginForm">
      <label>Email ID / ईमेल</label>
      <input id="email" type="email" required placeholder="Enter your email">
      <label>Password / पासवर्ड</label>
      <input id="password" type="password" required placeholder="Enter password">
      <button type="submit">Login / लॉगिन</button>
    </form>
    <p id="message" role="status"></p>
  </section>

  <section id="dashboard">
    <div class="card">
      <h2>Dashboard / डॅशबोर्ड</h2>
      <p id="welcome"></p>
      <button id="logout">Logout / बाहेर पडा</button>
    </div>
    <div class="grid">
      <div class="stat">New Leads<strong id="newCount">0</strong></div>
      <div class="stat">Login<strong id="loginCount">0</strong></div>
      <div class="stat">Approval<strong id="approvalCount">0</strong></div>
      <div class="stat">Disbursement<strong id="disbursementCount">0</strong></div>
      <div class="stat">Rejected<strong id="rejectedCount">0</strong></div>
    </div>
    <div class="card">
      <h3>Lead Management / लीड व्यवस्थापन</h3>
      <p>Database Connection झाल्यावर येथे नवीन Lead, Search, Edit आणि Follow-up सुविधा जोडल्या जातील.</p>
    </div>
  </section>
</div>
</body>
</html>
