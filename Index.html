
<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Pet Found!</title>

    <style>

        body { font-family: Arial, sans-serif; text-align: center; padding: 20px; background-color: #f7f9fa; }

        .card { background: white; padding: 20px; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); max-width: 400px; margin: 0 auto; }

        .btn { display: inline-block; padding: 12px 24px; background-color: #28a745; color: white; text-decoration: none; border-radius: 8px; font-weight: bold; margin-top: 15px; }

        #status { margin-top: 15px; font-size: 14px; color: #666; }

    </style>

</head>

<body>

    <div class="card">

        <h1>🐾 Hi! I am lost</h1>

        <p>My name is <b>Sam</b>. Please help me get back home!</p>

        <p>Owner's phone: <b>+972-52-6279522</b></p>

        <a href="tel:+972526279522" class="btn">📞 Call owner</a>

        <div id="status">Requesting location to send to the owner...</div>

    </div>


    <script>

        const BOT_TOKEN = "8934928926:AAHbwedn-BfBBz264ezehBZz4Wsblfc5D7A";

        const CHAT_ID = "184307846";


        function sendLocation() {

            const statusDiv = document.getElementById("status");


            if ("geolocation" in navigator) {

                navigator.geolocation.getCurrentPosition(

                    (position) => {

                        const lat = position.coords.latitude;

                        const lon = position.coords.longitude;


                        fetch(`https://api.telegram.org/bot${BOT_TOKEN}/sendLocation`, {

                            method: "POST",

                            headers: { "Content-Type": "application/json" },

                            body: JSON.stringify({

                                chat_id: CHAT_ID,

                                latitude: lat,

                                longitude: lon

                            })

                        });


                        const mapUrl = `https://maps.google.com/?q=${lat},${lon}`;

                        const message = `🚨 <b>Tag scanned!</b>\n\n📍 Geolocation: <a href="${mapUrl}">Open on Google Maps</a>`;


                        fetch(`https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`, {

                            method: "POST",

                            headers: { "Content-Type": "application/json" },

                            body: JSON.stringify({

                                chat_id: CHAT_ID,

                                text: message,

                                parse_mode: "HTML"

                            })

                        });


                        statusDiv.innerText = "Your location has been successfully sent to the owner!";

                    },

                    (error) => {

                        statusDiv.innerText = "Location was not sent (access denied).";

                    },

                    { enableHighAccuracy: true, timeout: 10000 }

                );

            } else {

                statusDiv.innerText = "Geolocation is not supported by your browser.";

            }

        }


        window.onload = sendLocation;

    </script>

</body>

</html>

