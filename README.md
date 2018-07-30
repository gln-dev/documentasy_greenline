# documentasy_greenline

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>Greenline Documentation</title>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato:400,700,400italic">
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="bslide.css">
  <link rel="stylesheet" href="sh.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  <link rel="canonical" href="https://nodejs.org/api/documentation.html">
  <style>
      .highlight table td { padding: 5px; }
.highlight table pre { margin: 0; }
.highlight, .highlight .w {
  color: #f8f8f2;
  background-color: #272822;
}
.highlight .err {
  color: #272822;
  background-color: #f92672;
}
.highlight .c, .highlight .cd, .highlight .cm, .highlight .c1, .highlight .cs {
  color: #75715e;
}
.highlight .cp {
  color: #f4bf75;
}
.highlight .nt {
  color: #f4bf75;
}
.highlight .o, .highlight .ow {
  color: #f8f8f2;
}
.highlight .p, .highlight .pi {
  color: #f8f8f2;
}
.highlight .gi {
  color: #a6e22e;
}
.highlight .gd {
  color: #f92672;
}
.highlight .gh {
  color: #66d9ef;
  background-color: #272822;
  font-weight: bold;
}
.highlight .k, .highlight .kn, .highlight .kp, .highlight .kr, .highlight .kv {
  color: #ae81ff;
}
.highlight .kc {
  color: #fd971f;
}
.highlight .kt {
  color: #fd971f;
}
.highlight .kd {
  color: #fd971f;
}
.highlight .s, .highlight .sb, .highlight .sc, .highlight .sd, .highlight .s2, .highlight .sh, .highlight .sx, .highlight .s1 {
  color: #a6e22e;
}
.highlight .sr {
  color: #a1efe4;
}
.highlight .si {
  color: #cc6633;
}
.highlight .se {
  color: #cc6633;
}
.highlight .nn {
  color: #f4bf75;
}
.highlight .nc {
  color: #f4bf75;
}
.highlight .no {
  color: #f4bf75;
}
.highlight .na {
  color: #66d9ef;
}
.highlight .m, .highlight .mf, .highlight .mh, .highlight .mi, .highlight .il, .highlight .mo, .highlight .mb, .highlight .mx {
  color: #a6e22e;
}
.highlight .ss {
  color: #a6e22e;
}
#myBtn {
  display: none;
  position: fixed;
  bottom: 20px;
  right: 30px;
  z-index: 99;
  font-size: 18px;
  border: none;
  outline: none;
  background-color: #555;
  color: white;
  cursor: pointer;
  padding: 15px;
  border-radius: 4px;
}

#myBtn:hover {
  background-color: #FF8C00;
}
</style>
</head>
<body class="alt apidoc" id="api-section-documentation">
  <div id="content" class="clearfix">
    <div id="column2" class="interior">
      <div id="intro" class="interior">
        <a href="index2.html" title="Go back to the home page">
         Greenline
        </a>
      </div>
      <!--introduced_in=v0.10.0-->
<ul>

</ul>
<div class="line"></div>

<ul>
<li><a class="nav-assert" href="#Introduction">Introduction</a></li>
<li><a class="nav-async_hooks" href="#Integration">Integration</a>
<ul>
  <li><a class="nav-async_hooks" href="#Development">Development</a></li>
  </ul></li>
<li><a class="nav-buffer" href="#API-Referention">API Referention</a>
<ul>
  <li><a class="nav-async_hooks" href="#Make-Transaction">Make Transaction</a></li>
  <li><a class="nav-async_hooks" href="#Create-Wallet">Create Wallet</a></li>
  <li><a class="nav-async_hooks" href="#Check-Balance">Check Balance</a></li>
  </ul></li>
<li><a class="nav-addons" href="#Response-Code">Response Code</a></li>

</ul>
<div class="line"></div>

<ul>

</ul>

    </div>

    <div id="column1" data-id="documentation" class="interior" >
      <header>
        <h1>Greenline Documentation</h1>
        
        <div id="gtoc">
          <ul>
          </ul>
        </div>
        <hr>
      </header>

      <div id="toc" >

      </div>
      <a href="javascript:"  onclick="topFunction()" id="myBtn" title="Go to top"><i class="fa fa-hand-o-up" aria-hidden="true"></i></a>

      <div id="Introduction">
        <h1>introduction<span><a class="mark" href="#documentation_about_this_documentation" id="documentation_about_this_documentation"></a></span></h1>
<!--introduced_in=v0.10.0-->
<!-- type=misc -->
<p>Welcome to Greenline. Greenline is a simple,accessed over HTTP or HTTPS from the dev.greenline.ai domain.</p>
<h2>Integration<span><a class="mark" href="#documentation_contributing" id="documentation_contributing"></a></span></h2>
<p>1. Develop (make) modul interface on your system (member) that contains of sender functions transaction request to environment development system greenline.ai based on spesification.</p>

<h2>Development<span><a class="mark" href="#documentation_stability_index" id="documentation_stability_index"></a></span></h2>
<!--type=misc-->
<p>We dedicate this environmental development to ease you doing integration modul your H2H system to greenline.ai.</p>
 <p>In this phase, please make an interface modul on your system (member) who has to send the request to URL API in greenline.ai which appropriates with the spesification.</p>
                  
<h2>API Referention<span><a class="mark" href="#documentation_json_output" id="API-Referention"></a></span></h2>
<div class="api_metadata">
<span></span>
</div><!-- <div class="api_stability api_stability_1"><a href="documentation.html#documentation_stability_index">Stability: 1</a> - Experimental</div> --><p>Please use message format which is convenient for your (member), there is some format that is available, such as : JSON. </p>


            <p>You can check your current limits and usage via a POST on the following endpoint, outside of our normal coin/chain pattern:</p>

            <p> Generally, in the option JSON format , every transaction request is sent through HTTPS protocol <code style="background-color: green" class="prettyprint">HTTPS</code> to target URL API greenline.ai with condition: </p>

            <ol>
            <li>header <code style="background-color: green">Content-Type: application/json</code>  to JSON format.</li>
            <li>contains to contents request according to API greenline.ai spesification.</li>
            <li>And set <code style="background-color: green">Authorization: Bearer $api_token</code>.</li>
            </ol>
            <h3 id="target-url-api-development">Target URL API Development</h3>

            <table><thead>
            <tr>
            <th>Format</th>
            <th>Target URL</th>
            </tr>
            </thead><tbody>
            <tr>
            <td>JSON</td>
            <td><code class="prettyprint">POST https://www.greenline.ai/api</code></td>
            </tr>
            </tbody></table>
<h2>Make Transaction<span><a class="mark" href="#documentation_syscalls_and_man_pages" id="Make-Transaction"></a></span></h2>
<p>Making the latest transaction.<br>
                  first you need to provide the input password, wallet, and amount. </p>
<blockquote >
                  <p>Make Transaction Request</p>
                  </blockquote>
                  <ul>
                  <pre class="highlight json"><span class="p">curl https://www.greenline.ai/api/transac</span>
<span class="p">{</span><span class="w">
  </span><span class="nt">"password"</span><span class="p">:</span><span class="w"> </span><span class="s2">"YOUR_PASSWORD"</span><span class="p">,</span><span class="w">
  </span><span class="nt">"address"</span><span class="p">:</span><span class="w"> </span><span class="s2">"MEMBER_ADDRESS"</span><span class="p">,</span><span class="w">
  </span><span class="nt">"amount"</span><span class="p">:</span><span class="w"> </span><span class="s2">"MEMBER_AMOUNT"</span><span class="p">,</span><span class="w">
</span><span class="p">}</span><span class="w">
</span></code></pre>  </ul>

<p><strong>Request Parameters</strong></p>

 <table><thead>
              <tr>
              <th>Parameters</th>
              <th>Value</th>
              <th>Description</th>
              </tr>
              </thead><tbody>
              <tr>
              <td>password</td>
              <td>YOUR_PASSWORD</code></td>
              <td>your password</td>
              </tr>
              <tr>
              <td>address</td>
              <td>MEMBER_ADDRESS</td>
              <td>member address.</td>
              </tr>
              <tr>
              <td>amount</td>
              <td>MEMBER_AMOUNT</td>
              <td>amount member.</td>
              </tr>

              </tbody></table>

<blockquote>
<p>Make Transaction Response</p>
</blockquote>

<pre class="highlight json">

<span class="p">{</span><span class="w">
  </span><span class="nt">"success"</span><span class="p">:</span><span class="w"> </span><span class="s2">"true"</span><span class="p">,</span><span class="w">
  </span><span class="nt">"data"</span><span class="p">:</span><span class="w"><span class="p">{</span><span class="w">
  <span class="nt">"message"</span><span class="p">:</span> </span><span class="s2">"Your transaction has ben success"</span><span class="p">,</span><span class="w"><span class="w">
  <span class="nt">"balance"</span><span class="p">:</span> </span><span class="s2">"0.000000000"</span><span class="p">,<span class="w"></span><span class="p">
  </span><span class="nt">"block"</span><span class="p">:</span><span class="w"><span class="p">{</span>
  <span class="nt">"hash"</span><span class="p">:</span><span class="w"> </span><span class="s2">"e1ec83047d0beb49ba9e2f480f206386869e81dbf461ee1c15bc7592e003453a"</span><span class="p">,</span>
  <span class="nt">"sender_id"</span><span class="p">:</span><span class="w"> </span><span class="s2">"5a16c59a402c5a04a84ea3be"</span><span class="p">,</span>
  <span class="nt">"receiver_id"</span><span class="p">:</span><span class="w"> </span><span class="s2">"5aa8b74e402c5a4ebf2cf2a2"</span><span class="p">,</span>
  <span class="nt">"data"</span><span class="p">:</span><span class="w"> </span><span class="s2">"5fd85baed63db0722d44d7063bbc154daedc38ee304e22cc23fe3bacffe9ca6a"</span><span class="p">,</span>
  <span class="nt">"value"</span><span class="p">:</span><span class="w"> </span><span class="s2">"1.0000000000"</span><span class="p">,</span>
  <span class="nt">"created_at"</span><span class="p">:</span><span class="w"> </span><span class="s2">"2018-05-01 11:20:17"</span><span class="p">,</span>
  <span class="nt">"_id"</span><span class="p">:</span><span class="w"> </span><span class="s2">"5ae83151402c5a17653f06e3"</span><span class="w">
</span><span class="p">}</span><span class="w"><span class="p">}</span>
<span class="p">}</span>
</span></code>
</pre>

</div>

<br>

<!-- The dots/circles -->




<h2 id="Create-Wallet">Create Wallet</h2>

<p></p>

<blockquote>
<p>Create Wallet Request</p>
</blockquote>
<pre class="highlight json"><span class="p">curl https://www.greenline.ai/api/new</span><br>
<span class="p">{</span><span class="w">
</span><span class="nt">"password"</span><span class="p">:</span><span class="w"> </span><span class="s2">"YOUR_PASSWORD"</span>
<span class="p">}</span><span class="w">
</span></code></pre> 
<p><strong>Parameters Request</strong></p>

<table><thead>
              <tr>
              <th>Parameters</th>
              <th>Value</th>
              <th>Description</th>
              </tr>
              </thead><tbody>
              <tr>
              <td>password</td>
              <td>YOUR_PASSWORD</code></td>
              <td>your password</td>
              </tr>

</tbody></table>
<blockquote>
<p>Create Wallet Response</p>
</blockquote>
<pre class="highlight json"><span class="p">curl https://www.greenline.ai/api/new</span>
<span class="p">{</span><span class="w">
</span><span class="nt">"success"</span><span class="p">:</span><span class="w"> </span><span class="s2">"true"</span><span class="p">,</span><span class="w">
</span><span class="nt">"data"</span><span class="p">:</span><span class="p">{</span><br>
 <span class="nt">"message"</span><span class="p">:</span> <span class="s2">"Account created"</span><span>,</span><span class="w">
 </span>
 <span class="nt">"detail"</span><span class="p">:</span><span class="p">{</span>
 <br><span class="w"> </span>
 <span class="nt"> "wallet"</span><span class="p">:</span><span class="s2">"SYrOykTM6LEL3jhCxQEXrqXMO8lhVMicoYu9owGp46YLn8PaGVNOTB5ekz54pxPGk6VAgkX9cGiYR"</span>,
 <span class="nt"> "balance"</span><span class="p">:</span><span class="s2">"0"</span>,
 <span class="nt"> "secret_key"</span><span class="p">:</span><span class="s2">"645716fb88007616783d818c9b2a7d616fc97154932757357e3e79a70363c5ee673ffce2d4453fd3de8e817eb7aa86d9b79339e850aa35c26e387c427e183485"</span>,
 <span class="nt"> "id"</span><span class="p">:</span><span class="s2">"5ae825d8402c5a230812ea73"</span>,
 <span class="nt"> "token"</span><span class="p">:</span><span class="s2">"010fa85d20fa4e586254c9a386a57a9f2ce1937ae904d22f7865aa5f09aea7626de2b22897ada7f5e4843ecdee0135281733807686dd8b3bad7efeae4e3cabd3"</span><span class="w"></span><span class="p">}</span>
 <span class="p">}</span>
 <span class="p">}</span>
 <span class="w"></span></code></pre>


          <h2 id="Check-Balance">Check Balance</h2>

<p></p>

<blockquote>
<p>Check Balance Request</p>
</blockquote>
<pre class="highlight json"><span class="p">curl https://www.greenline.ai/api/balance</span>
<span class="p">{</span><span class="w">
  </span><span class="nt">"password"</span><span class="p">:</span><span class="w"> </span><span class="s2">"YOUR_PASSWORD"</span><span class="p">,</span><span class="w">
  </span><span class="nt">"key"</span><span class="p">:</span><span class="w"> </span><span class="s2">"YOUR_SECRET_KEY"</span><span class="p"></span><span class="w">
</span><span class="p">}</span><span class="w">
</span></code></pre>
<p><strong>Parameters Request</strong></p>

<table><thead>
              <tr>
              <th>Parameters</th>
              <th>Value</th>
              <th>Description</th>
              </tr>
              </thead><tbody>
              <tr>
              <td>password</td>
              <td>YOUR_PASSWORD</code></td>
              <td>your password</td>
              </tr>
              <tr>
              <td>key</td>
              <td>SECRET_KEY</code></td>
              <td>your key</td>
              </tr>

              </tbody></table>


<blockquote>
<p>Check Balance Response</p>
</blockquote>
<pre class="highlight json"><span class="p">curl https://www.greenline.ai/api/new</span>
<span class="p">{</span><span class="w">
</span><span class="nt">"success"</span><span class="p">:</span><span class="w"> </span><span class="s2">"true"</span><span class="p">,</span><span class="w">
</span><span class="nt">"data"</span><span class="p">:</span><span class="p">{</span><br>
 <span class="nt">"message"</span><span class="p">:</span> <span class="s2">"Account created"</span><span>,</span><span class="w">
 </span>
 <span class="nt">"detail"</span><span class="p">:</span><span class="p">{</span>
 <br><span class="w"> </span>
 <span class="nt"> "wallet"</span><span class="p">:</span><span class="s2">"SYrOykTM6LEL3jhCxQEXrqXMO8lhVMicoYu9owGp46YLn8PaGVNOTB5ekz54pxPGk6VAgkX9cGiYR"</span>,
 <span class="nt"> "balance"</span><span class="p">:</span><span class="s2">"0"</span>,
 <span class="nt"> "secret_key"</span><span class="p">:</span><span class="s2">"645716fb88007616783d818c9b2a7d616fc97154932757357e3e79a70363c5ee673ffce2d4453fd3de8e817eb7aa86d9b79339e850aa35c26e387c427e183485"</span>,
 <span class="nt"> "id"</span><span class="p">:</span><span class="s2">"5ae825d8402c5a230812ea73"</span>,
 <span class="nt"> "token"</span><span class="p">:</span><span class="s2">"010fa85d20fa4e586254c9a386a57a9f2ce1937ae904d22f7865aa5f09aea7626de2b22897ada7f5e4843ecdee0135281733807686dd8b3bad7efeae4e3cabd3"</span><span class="w"></span><span class="p">}</span>
 <span class="p">}</span>
 <span class="w"></span></code></pre>
<h1 id="Response-Code">Response Code</h1>

<p>Response Code is a respond code that is given by greenline.ai system as status from every transaction request which is sent by member system (CA).</p>

<p>Based on the outline, the following are response code less:</p>

<table><thead>
<tr>
<th>Status Code</th>
<th>Description</th>
</tr>
</thead><tbody>

<tr>
<td>200</td>
<td>Your transaction has been success</td>
</tr>

<tr>
<td>200</td>
<td>Account created</td>
</tr>

<tr>
<td>500</td>
<td>Unauthenticated</td>
</tr>

<tr>
<td>500</td>
<td>The given data was invalid.</td>
</tr>

<tr>
<td>200</td>
<td>Something wrong.</td>
</tr>

<tr>
<td>405</td>
<td>method not allowed.</td>
</tr>

<tr>
<td>404</td>
<td>page not found.</td>
</tr>


</tbody></table>

<div class="api_stability api_stability_2"><a href="documentation.html#documentation_stability_index"></a> The list of code response can change along with the increase of
    product scope which is supported by greenline.ai.</div>


      </div>
    </div>
  </div>
  <script src="assets/sh_main.js"></script>
  <script src="assets/sh_javascript.min.js"></script>
  <script>highlight(undefined, undefined, 'pre');</script>
  
    <script src="assets/dnt_helper.js"></script>
    <script>
      if (!_dntEnabled()) {
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;
        i[r]=i[r]||function(){(i[r].q=i[r].q||[]).push(arguments)},
        i[r].l=1*new Date();a=s.createElement(o),m=s.getElementsByTagName(o)[0];
        a.async=1;a.src=g;m.parentNode.insertBefore(a,m)})(window,document,
        'script','//www.google-analytics.com/analytics.js','ga');
        ga('create', 'UA-67020396-1', 'auto');
        ga('send', 'pageview');
      }

    </script>
    <script>
// When the user scrolls down 20px from the top of the document, show the button
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
    if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
        document.getElementById("myBtn").style.display = "block";
    } else {
        document.getElementById("myBtn").style.display = "none";
    }
}

// When the user clicks on the button, scroll to the top of the document
function topFunction() {
    document.body.scrollTop = 0;
    document.documentElement.scrollTop = 0;
}
</script>

 <!-- slide -->
  <script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
}
</script>

</body>
</html>

