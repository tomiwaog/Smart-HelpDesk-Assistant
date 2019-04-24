<!-- ******************* For Standalone ChatBot page, Simply do the following: *******************
Step 1. Upload the "/chat/" directory (accessible via /Standalone/chat/) to your website.
Step2. Access your chat via www.yourdomain.com/chat -->


<!-- ******************* For embedding the chat widget into your preferred web page *******************

Step 1. Please copy the following code and paste it above the closing </html> tag of your website -->
<div id="chatwidget">
    <button class="open-button" onclick="openForm()">Chat</button>
    <div class="chat-popup" id="myForm">
        <iframe id="chatIframe" src="http://localhost:3000/yorao/chat"
            style="border:5px #ffffff none; position: fixed;bottom: 0; right: 0;" name="myiFrame" scrolling="no"
            frameborder="10" marginheight="0px" marginwidth="0px" height="750px" width="500px" allowfullscreen>
        </iframe>
        <button type="button" class="btn cancel" onclick="closeForm()">Close</button>
    </div>
    <script>
        function openForm() {
            document.getElementById("myForm").style.display = "block";
        }
        function closeForm() {
            document.getElementById("myForm").style.display = "none";
        }
    </script>
</div>

<!-- Step 2. Insert the following Code right above of your closing </head> tag -->
<link rel="stylesheet" type="text/css" href="iframe.css" />

<!-- Step 3. (Optional for best view) - Upload iframe.css (Acessible via /embedable/chat/iframe.ss) 
    in the same directory you've inserted the above codes -->
